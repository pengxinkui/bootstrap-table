# 表格参数 []({{ site.repo }}/blob/master/docs/_i18n/{{ site.lang }}/documentation/table-options.md)

---

表格的参数定义在 `jQuery.fn.bootstrapTable.defaults`。

<table class="table"
       id="t"
       data-search="true"
       data-show-toggle="true"
       data-show-columns="true"
       data-mobile-responsive="true">
    <thead>
    <tr>
        <th>名称</th>
        <th>标签</th>
        <th>类型</th>
        <th>默认</th>
        <th>描述</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td>-</td>
        <td>data-toggle</td>
        <td>String</td>
        <td>'table'</td>
        <td>不用写 JavaScript 直接启用表格。</td>
    </tr>
    <tr>
        <td>classes</td>
        <td>data-classes</td>
        <td>String</td>
        <td>'table table-hover'</td>
        <td>表格的类名称。默认情况下，表格是有边框的，你可以添加 'table-no-bordered' 来删除表格的边框样式。</td>
    </tr>
    <tr>
        <td>height</td>
        <td>data-height</td>
        <td>Number</td>
        <td>undefined</td>
        <td>定义表格的高度。</td>
    </tr>
    <tr>
        <td>undefinedText</td>
        <td>data-undefined-text</td>
        <td>String</td>
        <td>'-'</td>
        <td>定义默认的未定义的文本。</td>
    </tr>
    <tr>
        <td>striped</td>
        <td>data-striped</td>
        <td>Boolean</td>
        <td>false</td>
        <td>True 表示 以条纹色显示每行数据（隔行换色）。</td>
    </tr>
    <tr>
        <td>sortName</td>
        <td>data-sort-name</td>
        <td>String</td>
        <td>undefined</td>
        <td>定义哪些列可以进行排序。</td>
    </tr>
    <tr>
        <td>sortOrder</td>
        <td>data-sort-order</td>
        <td>String</td>
        <td>'asc'</td>
        <td>定义了列的排序顺序, 智能是 'asc' 或 'desc'。</td>
    </tr>
    <tr>
        <td>iconsPrefix</td>
        <td>data-icons-prefix</td>
        <td>String</td>
        <td>'glyphicon'</td>
        <td>定义图标组名称 ('glyphicon' 或 FontAwesome的'fa' ). 在默认情况下使用 'glyphicon' 。</td>
    </tr>
    <tr>
        <td>icons</td>
        <td>data-icons</td>
        <td>Object</td>
        <td>{<br/>
        &nbsp;&nbsp;refresh: 'glyphicon-refresh icon-refresh',<br/>
        &nbsp;&nbsp;toggle: 'glyphicon-list-alt icon-list-alt',<br/>
        &nbsp;&nbsp;columns: 'glyphicon-th icon-th'<br/>
        }</td>
        <td>定义刷新、切换、列三个按钮的图标</td>
    </tr>
    <tr>
        <td>columns</td>
        <td>-</td>
        <td>Array</td>
        <td>[]</td>
        <td>表格的列的配置对象, 请查看 列配置 获取更多信息.
        </td>
    </tr>
    <tr>
        <td>data</td>
        <td>-</td>
        <td>Array</td>
        <td>[]</td>
        <td>需要加载的数据.</td>
    </tr>
    <tr>
        <td>ajax</td>
        <td>data-ajax</td>
        <td>Function</td>
        <td>undefined</td>
        <td>一个取代ajax调用的方法. 需要实现和jQuery ajax 方法相同的API。</td>
    </tr>
    <tr>
        <td>method</td>
        <td>data-method</td>
        <td>String</td>
        <td>'get'</td>
        <td>请求远程数据的方法类型。</td>
    </tr>
    <tr>
        <td>url</td>
        <td>data-url</td>
        <td>String</td>
        <td>undefined</td>
        <td>从远程站点请求数据的 URL 。</td>
    </tr>
    <tr>
        <td>cache</td>
        <td>data-cache</td>
        <td>Boolean</td>
        <td>true</td>
        <td>False 表示 禁用AJAX请求的缓存。</td>
    </tr>
    <tr>
        <td>contentType</td>
        <td>data-content-type</td>
        <td>String</td>
        <td>'application/json'</td>
        <td>The contentType of request remote data.</td>
    </tr>
    <tr>
        <td>dataType</td>
        <td>data-data-type</td>
        <td>String</td>
        <td>'json'</td>
        <td>您期望从服务器返回的数据的类型。</td>
    </tr>
    <tr>
        <td>ajaxOptions</td>
        <td>data-ajax-options</td>
        <td>Object</td>
        <td>{}</td>
        <td>提交ajax请求的附加选项。 选项列表: <a href="http://api.jquery.com/jQuery.ajax">http://api.jquery.com/jQuery.ajax</a>.</td>
    </tr>
    <tr>
        <td>queryParams</td>
        <td>data-query-params</td>
        <td>Function</td>
        <td>function(params) {<br>return params;<br>}</td>
        <td>
        当请求远程数据时,您可以通过修改queryParams发送额外的参数。
        If queryParamsType = 'limit', the params object contains: <br>
        limit, offset, search, sort, order
        Else, it contains: <br>
        pageSize, pageNumber, searchText, sortName, sortOrder. <br>
        Return false to stop request.
        </td>
    </tr>
    <tr>
        <td>queryParamsType</td>
        <td>data-query-params-type</td>
        <td>String</td>
        <td>'limit'</td>
        <td>Set 'limit' to send query params width RESTFul type.</td>
    </tr>
    <tr>
        <td>responseHandler</td>
        <td>data-response-handler</td>
        <td>Function</td>
        <td>function(res) {<br>return res;<br>}</td>
        <td>
        Before load remote data, handler the response data format, the parameters object contains: <br>
        res: the response data.
        </td>
    </tr>
    <tr>
        <td>pagination</td>
        <td>data-pagination</td>
        <td>Boolean</td>
        <td>false</td>
        <td>True to show a pagination toolbar on table bottom.</td>
    </tr>
    <tr>
        <td>onlyInfoPagination</td>
        <td>data-only-info-pagination</td>
        <td>Boolean</td>
        <td>false</td>
        <td>True to show only the quantity of the data that is showing in the table. It needs the pagination table options is set to true.</td>
    </tr>
    <tr>
        <td>sidePagination</td>
        <td>data-side-pagination</td>
        <td>String</td>
        <td>'client'</td>
        <td>Defines the side pagination of table, can only be 'client' or 'server'. Using 'server' side requires either setting the 'url' or 'ajax' option</td>
    </tr>
    <tr>
        <td>pageNumber</td>
        <td>data-page-number</td>
        <td>Number</td>
        <td>1</td>
        <td>When set pagination property, initialize the page number.</td>
    </tr>
    <tr>
        <td>pageSize</td>
        <td>data-page-size</td>
        <td>Number</td>
        <td>10</td>
        <td>When set pagination property, initialize the page size.</td>
    </tr>
    <tr>
        <td>pageList</td>
        <td>data-page-list</td>
        <td>Array</td>
        <td>[10, 25, 50, 100, All]</td>
        <td>When set pagination property, initialize the page size selecting list. If you include the 'All' option, all the records will be shown in your table</td>
    </tr>
    <tr>
        <td>selectItemName</td>
        <td>data-select-item-name</td>
        <td>String</td>
        <td>'btSelectItem'</td>
        <td>The name of radio or checkbox input.</td>
    </tr>
    <tr>
        <td>smartDisplay</td>
        <td>data-smart-display</td>
        <td>Boolean</td>
        <td>true</td>
        <td>True to display pagination or card view smartly.</td>
    </tr>
    <tr>
        <td>escape</td>
        <td>data-escape</td>
        <td>Boolean</td>
        <td>false</td>
        <td>转义HTML字符串，替换 <code>&</code>, <code><</code>,
        <code>></code>, <code>"</code>, <code>`</code>, 和 <code>'</code> 字符.</td>
    </tr>
    <tr>
        <td>search</td>
        <td>data-search</td>
        <td>Boolean</td>
        <td>false</td>
        <td>Enable the search input.</td>
    </tr>
    <tr>
        <td>searchOnEnterKey</td>
        <td>data-search-on-enter-key</td>
        <td>Boolean</td>
        <td>false</td>
        <td>The search method will be executed until the Enter key is pressed.</td>
    </tr>
    <tr>
        <td>strictSearch</td>
        <td>data-strict-search</td>
        <td>Boolean</td>
        <td>false</td>
        <td>Enable the strict search.</td>
    </tr>
	<tr>
        <td>searchText</td>
        <td>data-search-text</td>
        <td>String</td>
        <td>''</td>
        <td>When set search property, initialize the search text.</td>
    </tr>
    <tr>
        <td>searchTimeOut</td>
        <td>data-search-time-out</td>
        <td>Number</td>
        <td>500</td>
        <td>Set timeout for search fire.</td>
    </tr>
    <tr>
        <td>trimOnSearch</td>
        <td>data-trim-on-search</td>
        <td>Boolean</td>
        <td>true</td>
        <td>True to trim spaces in search field.</td>
    </tr
    <tr>
        <td>showHeader</td>
        <td>data-show-header</td>
        <td>Boolean</td>
        <td>true</td>
        <td>False to hide the table header.</td>
    </tr>
    <tr>
        <td>showFooter</td>
        <td>data-show-footer</td>
        <td>Boolean</td>
        <td>false</td>
        <td>If true shows summary footer row</td>
    </tr>
    <tr>
        <td>showColumns</td>
        <td>data-show-columns</td>
        <td>Boolean</td>
        <td>false</td>
        <td>True to show the columns drop down list.</td>
    </tr>
    <tr>
        <td>showRefresh</td>
        <td>data-show-refresh</td>
        <td>Boolean</td>
        <td>false</td>
        <td>True to show the refresh button.</td>
    </tr>
    <tr>
        <td>showToggle</td>
        <td>data-show-toggle</td>
        <td>Boolean</td>
        <td>false</td>
        <td>True to show the toggle button to toggle table / card view.
        </td>
    </tr>
    <tr>
        <td>showPaginationSwitch</td>
        <td>data-show-pagination-switch</td>
        <td>Boolean</td>
        <td>false</td>
        <td>True to show the pagination switch button.</td>
    </tr>
    <tr>
        <td>minimumCountColumns</td>
        <td>data-minimum-count-columns</td>
        <td>Number</td>
        <td>1</td>
        <td>The minimum count columns to hide of the columns drop down list.
        </td>
    </tr>
    <tr>
        <td>idField</td>
        <td>data-id-field</td>
        <td>String</td>
        <td>undefined</td>
        <td>Indicate which field is an identity field.</td>
    </tr>
    <tr>
        <td>uniqueId</td>
        <td>data-unique-id</td>
        <td>String</td>
        <td>undefined</td>
        <td>Indicate an unique identifier for each row.</td>
    </tr>
    <tr>
        <td>cardView</td>
        <td>data-card-view</td>
        <td>Boolean</td>
        <td>false</td>
        <td>True to show card view table, for example mobile view.</td>
    </tr>
    <tr>
        <td>detailView</td>
        <td>data-detail-view</td>
        <td>Boolean</td>
        <td>false</td>
        <td>设置为 True 可以显示详细页面模式。</td>
    </tr>
    <tr>
        <td>detailFormatter</td>
        <td>data-detail-formatter</td>
        <td>Function</td>
        <td>function(index, row) {<br>return '';<br>}</td>
        <td>格式化详细页面模式的视图。</td>
    </tr>
    <tr>
        <td>searchAlign</td>
        <td>data-search-align</td>
        <td>String</td>
        <td>'right'</td>
        <td>Indicate how to align the search input. 'left', 'right' can be used.</td>
    </tr>
    <tr>
        <td>buttonsAlign</td>
        <td>data-buttons-align</td>
        <td>String</td>
        <td>'right'</td>
        <td>Indicate how to align the toolbar buttons. 'left', 'right' can be used.</td>
    </tr>
    <tr>
        <td>toolbarAlign</td>
        <td>data-toolbar-align</td>
        <td>String</td>
        <td>'left'</td>
        <td>Indicate how to align the custom toolbar. 'left', 'right' can be used.</td>
    </tr>
    <tr>
        <td>paginationVAlign</td>
        <td>data-pagination-v-align</td>
        <td>String</td>
        <td>'bottom'</td>
        <td>Indicate how to align the pagination. 'top', 'bottom', 'both' (put the pagination on top and bottom)  can be used.</td>
    </tr>
    <tr>
        <td>paginationHAlign</td>
        <td>data-pagination-h-align</td>
        <td>String</td>
        <td>'right'</td>
        <td>Indicate how to align the pagination. 'left', 'right' can be used.</td>
    </tr>
    <tr>
        <td>paginationDetailHAlign</td>
        <td>data-pagination-detail-h-align</td>
        <td>String</td>
        <td>'left'</td>
        <td>Indicate how to align the pagination detail. 'left', 'right' can be used.</td>
    </tr>
    <tr>
        <td>paginationPreText</td>
        <td>data-pagination-pre-text</td>
        <td>String</td>
        <td>'&lt;'</td>
        <td>Indicate the icon or text to be shown in the pagination detail, the previous button.</td>
    </tr>
    <tr>
        <td>paginationNextText</td>
        <td>data-pagination-next-text</td>
        <td>String</td>
        <td>'&gt;'</td>
        <td>Indicate the icon or text to be shown in the pagination detail, the next button.</td>
    </tr>
    <tr>
        <td>clickToSelect</td>
        <td>data-click-to-select</td>
        <td>Boolean</td>
        <td>false</td>
        <td>True to select checkbox or radiobox when click rows.</td>
    </tr>
    <tr>
        <td>singleSelect</td>
        <td>data-single-select</td>
        <td>Boolean</td>
        <td>false</td>
        <td>True to allow checkbox selecting only one row.</td>
    </tr>
    <tr>
        <td>toolbar</td>
        <td>data-toolbar</td>
        <td>String</td>
        <td>undefined</td>
        <td>
        A jQuery selector that indicate the toolbar, for example:<br>
        #toolbar, .toolbar.
        </td>
    </tr>
    <tr>
        <td>checkboxHeader</td>
        <td>data-checkbox-header</td>
        <td>Boolean</td>
        <td>true</td>
        <td>False to hide check-all checkbox in header row.</td>
    </tr>
    <tr>
        <td>maintainSelected</td>
        <td>data-maintain-selected</td>
        <td>Boolean</td>
        <td>false</td>
        <td>True to maintain selected rows on change page and search.</td>
    </tr>
    <tr>
        <td>sortable</td>
        <td>data-sortable</td>
        <td>Boolean</td>
        <td>true</td>
        <td>False to disable sortable of all columns.</td>
    </tr>
    <tr>
        <td>silentSort</td>
        <td>data-silent-sort</td>
        <td>Boolean</td>
        <td>true</td>
        <td>Set <code>false</code> to sort the data silently. This options works when the sidePagination option is set to <code>server</code>.</td>
    </tr>
    <tr>
        <td>rowStyle</td>
        <td>data-row-style</td>
        <td>Function</td>
        <td>{}</td>
        <td>
        The row style formatter function, take two parameters: <br>
        row: the row record data.<br>
        index: the row index.<br>
        Support classes or css.
        </td>
    </tr>
    <tr>
        <td>rowAttributes</td>
        <td>data-row-attributes</td>
        <td>Function</td>
        <td>{}</td>
        <td>
        The row attribute formatter function, take two parameters: <br>
        row: the row record data.<br>
        index: the row index.<br>
        Support all custom attributes.
        </td>
    </tr>
    </tbody>
</table>
