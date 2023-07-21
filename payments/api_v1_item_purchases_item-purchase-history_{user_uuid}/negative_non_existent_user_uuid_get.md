### Payments
#### Item purchases item purchase history {user_uuid} (negative - non-existent user_uuid)

Тестовые данные: https://payments.alpha.g-spot.website/v1/item_purchases/item-purchase-history/{user_uuid}/

Предусловие: 

1. Создать новый запрос в Postman
2. Выбрать метод GET для Request
3. Ввести URL: https://payments.alpha.g-spot.website/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/ 
4. Отправить Request

Ожидаемый результат: Server response: status code 500 - Internal Server Error

Body response (закомментирован):

<!--
<!DOCTYPE html>
<html lang="en">
<head>
  <meta http-equiv="content-type" content="text/html; charset=utf-8">
  <meta name="robots" content="NONE,NOARCHIVE">
  <title>KeyError
          at /api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/</title>
  <style type="text/css">
    html * { padding: 0; margin: 0;
}
    body * { padding: 10px 20px;
}
    body * * { padding: 0;
}
    body { font:small sans-serif; background-color:#fff; color:#000;
}
    body>div { border-bottom: 1px solid #ddd;
}
    h1 { font-weight:normal;
}
    h2 { margin-bottom:.8em;
}
    h3 { margin:1em 0 .5em 0;
}
    h4 { margin: 0 0 .5em 0; font-weight: normal;
}
    code, pre { font-size: 100%; white-space: pre-wrap; word-break: break-word;
}
    summary { cursor: pointer;
}
    table { border: 1px solid #ccc; border-collapse: collapse; width: 100%; background:white;
}
    tbody td, tbody th { vertical-align:top; padding: 2px 3px;
}
    thead th {
      padding: 1px 6px 1px 3px; background:#fefefe; text-align:left;
      font-weight:normal; font-size: 11px; border: 1px solid #ddd;
}
    tbody th { width:12em; text-align:right; color:#666; padding-right:.5em;
}
    table.vars { margin: 5px 10px 2px 40px; width: auto;
}
    table.vars td, table.req td { font-family:monospace;
}
    table td.code { width: 100%;
}
    table td.code pre { overflow:hidden;
}
    table.source th { color:#666;
}
    table.source td { font-family:monospace; white-space:pre; border-bottom: 1px solid #eee;
}
    ul.traceback { list-style-type:none; color: #222;
}
    ul.traceback li.cause { word-break: break-word;
}
    ul.traceback li.frame { padding-bottom:1em; color:#4f4f4f;
}
    ul.traceback li.user { background-color:#e0e0e0; color:#000
}
    div.context { padding: 10px 0; overflow:hidden;
}
    div.context ol { padding-left: 30px; margin: 0 10px; list-style-position: inside;
}
    div.context ol li { font-family:monospace; white-space:pre; color:#777; cursor:pointer; padding-left: 2px;
}
    div.context ol li pre { display:inline;
}
    div.context ol.context-line li { color:#464646; background-color:#dfdfdf; padding: 3px 2px;
}
    div.context ol.context-line li span { position:absolute; right: 32px;
}
    .user div.context ol.context-line li { background-color:#bbb; color:#000;
}
    .user div.context ol li { color:#666;
}
    div.commands, summary.commands { margin-left: 40px;
}
    div.commands a, summary.commands { color:#555; text-decoration:none;
}
    .user div.commands a { color: black;
}
    #summary { background: #ffc;
}
    #summary h2 { font-weight: normal; color: #666;
}
    #explanation { background:#eee;
}
    #template, #template-not-exist { background:#f6f6f6;
}
    #template-not-exist ul { margin: 0 0 10px 20px;
}
    #template-not-exist .postmortem-section { margin-bottom: 3px;
}
    #unicode-hint { background:#eee;
}
    #traceback { background:#eee;
}
    #requestinfo { background:#f6f6f6; padding-left: 120px;
}
    #summary table { border:none; background:transparent;
}
    #requestinfo h2, #requestinfo h3 { position:relative; margin-left: -100px;
}
    #requestinfo h3 { margin-bottom:-1em;
}
    .error { background: #ffc;
}
    .specific { color:#cc3300; font-weight:bold;
}
    h2 span.commands { font-size:.7em; font-weight:normal;
}
    span.commands a:link {color:#5E5694;
}
    pre.exception_value { font-family: sans-serif; color: #575757; font-size: 1.5em; margin: 10px 0 10px 0;
}
    .append-bottom { margin-bottom: 10px;
}
    .fname { user-select: all;
}
  </style>
  
  <script>
    function hideAll(elems) {
      for (var e = 0; e < elems.length; e++) {
        elems[e
        ].style.display = 'none';
    }
}
    window.onload = function() {
      hideAll(document.querySelectorAll('ol.pre-context'));
      hideAll(document.querySelectorAll('ol.post-context'));
      hideAll(document.querySelectorAll('div.pastebin'));
}
    function toggle() {
      for (var i = 0; i < arguments.length; i++) {
        var e = document.getElementById(arguments[i
        ]);
        if (e) {
          e.style.display = e.style.display == 'none' ? 'block': 'none';
        }
    }
      return false;
}
    function switchPastebinFriendly(link) {
      s1 = "Switch to copy-and-paste view";
      s2 = "Switch back to interactive view";
      link.textContent = link.textContent.trim() == s1 ? s2: s1;
      toggle('browserTraceback', 'pastebinTraceback');
      return false;
}
  </script>
  
</head>
<body>
<div id="summary">
  <h1>KeyError
       at /api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/</h1>
  <pre class="exception_value">&#x27;&#x27;</pre>
  <table class="meta">

    <tr>
      <th>Request Method:</th>
      <td>GET</td>
    </tr>
    <tr>
      <th>Request URL:</th>
      <td>http: //payments.alpha.g-spot.website/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/</td>
    </tr>

    <tr>
      <th>Django Version:</th>
      <td>4.1.7</td>
    </tr>

    <tr>
      <th>Exception Type:</th>
      <td>KeyError</td>
    </tr>


    <tr>
      <th>Exception Value:</th>
      <td><pre>&#x27;&#x27;</pre></td>
    </tr>


    <tr>
      <th>Exception Location:</th>
      <td><span class="fname">/home/app/web/apps/item_purchases/serializers.py</span>, line 60, in get_status</td>
    </tr>


    <tr>
      <th>Raised during:</th>
      <td>apps.item_purchases.views.ItemPurchaseHistoryView</td>
    </tr>

    <tr>
      <th>Python Executable:</th>
      <td>/usr/local/bin/python</td>
    </tr>
    <tr>
      <th>Python Version:</th>
      <td>3.11.4</td>
    </tr>
    <tr>
      <th>Python Path:</th>
      <td><pre>[&#x27;/home/app/web&#x27;,
 &#x27;/home/app/web&#x27;,
 &#x27;/usr/local/bin&#x27;,
 &#x27;/usr/local/lib/python311.zip&#x27;,
 &#x27;/usr/local/lib/python3.11&#x27;,
 &#x27;/usr/local/lib/python3.11/lib-dynload&#x27;,
 &#x27;/usr/local/lib/python3.11/site-packages&#x27;
]</pre></td>
    </tr>
    <tr>
      <th>Server time:</th>
      <td>Fri,
21 Jul 2023 09: 29: 59 +0000</td>
    </tr>
  </table>
</div>




<div id="traceback">
  <h2>Traceback <span class="commands"><a href="#" onclick="return switchPastebinFriendly(this);">
    Switch to copy-and-paste view</a></span>
  </h2>
  <div id="browserTraceback">
    <ul class="traceback">
      
        
        <li class="frame django">
          
            <code class="fname">/usr/local/lib/python3.11/site-packages/django/core/handlers/exception.py</code>, line 56, in inner
          

          
            <div class="context" id="c140475792330240">
              
                <ol start="49" class="pre-context" id="pre140475792330240">
                
                  <li onclick="toggle('pre140475792330240', 'post140475792330240')"><pre></pre></li>
                
                  <li onclick="toggle('pre140475792330240', 'post140475792330240')"><pre>        return inner</pre></li>
                
                  <li onclick="toggle('pre140475792330240', 'post140475792330240')"><pre>    else:</pre></li>
                
                  <li onclick="toggle('pre140475792330240', 'post140475792330240')"><pre></pre></li>
                
                  <li onclick="toggle('pre140475792330240', 'post140475792330240')"><pre>        @wraps(get_response)</pre></li>
                
                  <li onclick="toggle('pre140475792330240', 'post140475792330240')"><pre>        def inner(request):</pre></li>
                
                  <li onclick="toggle('pre140475792330240', 'post140475792330240')"><pre>            try:</pre></li>
                
                </ol>
              
              <ol start="56" class="context-line">
                <li onclick="toggle('pre140475792330240', 'post140475792330240')"><pre>                response = get_response(request)</pre> <span>…</span></li>
              </ol>
              
                <ol start='57' class="post-context" id="post140475792330240">
                  
                  <li onclick="toggle('pre140475792330240', 'post140475792330240')"><pre>            except Exception as exc:</pre></li>
                  
                  <li onclick="toggle('pre140475792330240', 'post140475792330240')"><pre>                response = response_for_exception(request, exc)</pre></li>
                  
                  <li onclick="toggle('pre140475792330240', 'post140475792330240')"><pre>            return response</pre></li>
                  
                  <li onclick="toggle('pre140475792330240', 'post140475792330240')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475792330240', 'post140475792330240')"><pre>        return inner</pre></li>
                  
                  <li onclick="toggle('pre140475792330240', 'post140475792330240')"><pre></pre></li>
                  
              </ol>
              
            </div>
          

          
            
              <details>
                <summary class="commands">Local vars</summary>
            
            <table class="vars" id="v140475792330240">
              <thead>
                <tr>
                  <th>Variable</th>
                  <th>Value</th>
                </tr>
              </thead>
              <tbody>
                
                  <tr>
                    <td>exc</td>
                    <td class="code"><pre>KeyError(&#x27;&#x27;)</pre></td>
                  </tr>
                
                  <tr>
                    <td>get_response</td>
                    <td class="code"><pre>&lt;bound method BaseHandler._get_response of &lt;django.core.handlers.wsgi.WSGIHandler object at 0x7fc316188a50&gt;&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>request</td>
                    <td class="code"><pre>&lt;WSGIRequest: GET &#x27;/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/&#x27;&gt;</pre></td>
                  </tr>
                
              </tbody>
            </table>
            </details>
          
        </li>
      
        
        <li class="frame django">
          
            <code class="fname">/usr/local/lib/python3.11/site-packages/django/core/handlers/base.py</code>, line 197, in _get_response
          

          
            <div class="context" id="c140475793998592">
              
                <ol start="190" class="pre-context" id="pre140475793998592">
                
                  <li onclick="toggle('pre140475793998592', 'post140475793998592')"><pre></pre></li>
                
                  <li onclick="toggle('pre140475793998592', 'post140475793998592')"><pre>        if response is None:</pre></li>
                
                  <li onclick="toggle('pre140475793998592', 'post140475793998592')"><pre>            wrapped_callback = self.make_view_atomic(callback)</pre></li>
                
                  <li onclick="toggle('pre140475793998592', 'post140475793998592')"><pre>            # If it is an asynchronous view, run it in a subthread.</pre></li>
                
                  <li onclick="toggle('pre140475793998592', 'post140475793998592')"><pre>            if asyncio.iscoroutinefunction(wrapped_callback):</pre></li>
                
                  <li onclick="toggle('pre140475793998592', 'post140475793998592')"><pre>                wrapped_callback = async_to_sync(wrapped_callback)</pre></li>
                
                  <li onclick="toggle('pre140475793998592', 'post140475793998592')"><pre>            try:</pre></li>
                
                </ol>
              
              <ol start="197" class="context-line">
                <li onclick="toggle('pre140475793998592', 'post140475793998592')"><pre>                response = wrapped_callback(request, *callback_args, **callback_kwargs)</pre> <span>…</span></li>
              </ol>
              
                <ol start='198' class="post-context" id="post140475793998592">
                  
                  <li onclick="toggle('pre140475793998592', 'post140475793998592')"><pre>            except Exception as e:</pre></li>
                  
                  <li onclick="toggle('pre140475793998592', 'post140475793998592')"><pre>                response = self.process_exception_by_middleware(e, request)</pre></li>
                  
                  <li onclick="toggle('pre140475793998592', 'post140475793998592')"><pre>                if response is None:</pre></li>
                  
                  <li onclick="toggle('pre140475793998592', 'post140475793998592')"><pre>                    raise</pre></li>
                  
                  <li onclick="toggle('pre140475793998592', 'post140475793998592')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475793998592', 'post140475793998592')"><pre>        # Complain if the view returned None (a common error).</pre></li>
                  
              </ol>
              
            </div>
          

          
            
              <details>
                <summary class="commands">Local vars</summary>
            
            <table class="vars" id="v140475793998592">
              <thead>
                <tr>
                  <th>Variable</th>
                  <th>Value</th>
                </tr>
              </thead>
              <tbody>
                
                  <tr>
                    <td>callback</td>
                    <td class="code"><pre>&lt;function ItemPurchaseHistoryView at 0x7fc3137a36a0&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>callback_args</td>
                    <td class="code"><pre>()</pre></td>
                  </tr>
                
                  <tr>
                    <td>callback_kwargs</td>
                    <td class="code"><pre>{&#x27;user_uuid&#x27;: UUID(&#x27;3fa85f64-5717-4562-b3fc-2c963f66afa6&#x27;)
}</pre></td>
                  </tr>
                
                  <tr>
                    <td>middleware_method</td>
                    <td class="code"><pre>&lt;bound method CsrfViewMiddleware.process_view of &lt;CsrfViewMiddleware get_response=convert_exception_to_response.&lt;locals&gt;.inner&gt;&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>request</td>
                    <td class="code"><pre>&lt;WSGIRequest: GET &#x27;/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/&#x27;&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>response</td>
                    <td class="code"><pre>None</pre></td>
                  </tr>
                
                  <tr>
                    <td>self</td>
                    <td class="code"><pre>&lt;django.core.handlers.wsgi.WSGIHandler object at 0x7fc316188a50&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>wrapped_callback</td>
                    <td class="code"><pre>&lt;function ItemPurchaseHistoryView at 0x7fc3137a36a0&gt;</pre></td>
                  </tr>
                
              </tbody>
            </table>
            </details>
          
        </li>
      
        
        <li class="frame django">
          
            <code class="fname">/usr/local/lib/python3.11/site-packages/django/views/decorators/csrf.py</code>, line 55, in wrapped_view
          

          
            <div class="context" id="c140475794011520">
              
                <ol start="48" class="pre-context" id="pre140475794011520">
                
                  <li onclick="toggle('pre140475794011520', 'post140475794011520')"><pre></pre></li>
                
                  <li onclick="toggle('pre140475794011520', 'post140475794011520')"><pre>def csrf_exempt(view_func):</pre></li>
                
                  <li onclick="toggle('pre140475794011520', 'post140475794011520')"><pre>    &quot;&quot;&quot;Mark a view function as being exempt from the CSRF view protection.&quot;&quot;&quot;</pre></li>
                
                  <li onclick="toggle('pre140475794011520', 'post140475794011520')"><pre></pre></li>
                
                  <li onclick="toggle('pre140475794011520', 'post140475794011520')"><pre>    # view_func.csrf_exempt = True would also work, but decorators are nicer</pre></li>
                
                  <li onclick="toggle('pre140475794011520', 'post140475794011520')"><pre>    # if they don&#x27;t have side effects, so return a new function.</pre></li>
                
                  <li onclick="toggle('pre140475794011520', 'post140475794011520')"><pre>    def wrapped_view(*args, **kwargs):</pre></li>
                
                </ol>
              
              <ol start="55" class="context-line">
                <li onclick="toggle('pre140475794011520', 'post140475794011520')"><pre>        return view_func(*args, **kwargs)</pre> <span>…</span></li>
              </ol>
              
                <ol start='56' class="post-context" id="post140475794011520">
                  
                  <li onclick="toggle('pre140475794011520', 'post140475794011520')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475794011520', 'post140475794011520')"><pre>    wrapped_view.csrf_exempt = True</pre></li>
                  
                  <li onclick="toggle('pre140475794011520', 'post140475794011520')"><pre>    return wraps(view_func)(wrapped_view)</pre></li>
                  
              </ol>
              
            </div>
          

          
            
              <details>
                <summary class="commands">Local vars</summary>
            
            <table class="vars" id="v140475794011520">
              <thead>
                <tr>
                  <th>Variable</th>
                  <th>Value</th>
                </tr>
              </thead>
              <tbody>
                
                  <tr>
                    <td>args</td>
                    <td class="code"><pre>(&lt;WSGIRequest: GET &#x27;/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/&#x27;&gt;,)</pre></td>
                  </tr>
                
                  <tr>
                    <td>kwargs</td>
                    <td class="code"><pre>{&#x27;user_uuid&#x27;: UUID(&#x27;3fa85f64-5717-4562-b3fc-2c963f66afa6&#x27;)
}</pre></td>
                  </tr>
                
                  <tr>
                    <td>view_func</td>
                    <td class="code"><pre>&lt;function ItemPurchaseHistoryView at 0x7fc3137a3600&gt;</pre></td>
                  </tr>
                
              </tbody>
            </table>
            </details>
          
        </li>
      
        
        <li class="frame user">
          
            <code class="fname">/usr/local/lib/python3.11/site-packages/rest_framework/viewsets.py</code>, line 125, in view
          

          
            <div class="context" id="c140475792300736">
              
                <ol start="118" class="pre-context" id="pre140475792300736">
                
                  <li onclick="toggle('pre140475792300736', 'post140475792300736')"><pre>                setattr(self, method, handler)</pre></li>
                
                  <li onclick="toggle('pre140475792300736', 'post140475792300736')"><pre></pre></li>
                
                  <li onclick="toggle('pre140475792300736', 'post140475792300736')"><pre>            self.request = request</pre></li>
                
                  <li onclick="toggle('pre140475792300736', 'post140475792300736')"><pre>            self.args = args</pre></li>
                
                  <li onclick="toggle('pre140475792300736', 'post140475792300736')"><pre>            self.kwargs = kwargs</pre></li>
                
                  <li onclick="toggle('pre140475792300736', 'post140475792300736')"><pre></pre></li>
                
                  <li onclick="toggle('pre140475792300736', 'post140475792300736')"><pre>            # And continue as usual</pre></li>
                
                </ol>
              
              <ol start="125" class="context-line">
                <li onclick="toggle('pre140475792300736', 'post140475792300736')"><pre>            return self.dispatch(request, *args, **kwargs)</pre> <span>…</span></li>
              </ol>
              
                <ol start='126' class="post-context" id="post140475792300736">
                  
                  <li onclick="toggle('pre140475792300736', 'post140475792300736')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475792300736', 'post140475792300736')"><pre>        # take name and docstring from class</pre></li>
                  
                  <li onclick="toggle('pre140475792300736', 'post140475792300736')"><pre>        update_wrapper(view, cls, updated=())</pre></li>
                  
                  <li onclick="toggle('pre140475792300736', 'post140475792300736')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475792300736', 'post140475792300736')"><pre>        # and possible attributes set by decorators</pre></li>
                  
                  <li onclick="toggle('pre140475792300736', 'post140475792300736')"><pre>        # like csrf_exempt from dispatch</pre></li>
                  
              </ol>
              
            </div>
          

          
            
              <details>
                <summary class="commands">Local vars</summary>
            
            <table class="vars" id="v140475792300736">
              <thead>
                <tr>
                  <th>Variable</th>
                  <th>Value</th>
                </tr>
              </thead>
              <tbody>
                
                  <tr>
                    <td>action</td>
                    <td class="code"><pre>&#x27;list&#x27;</pre></td>
                  </tr>
                
                  <tr>
                    <td>actions</td>
                    <td class="code"><pre>{&#x27;get&#x27;: &#x27;list&#x27;, &#x27;head&#x27;: &#x27;list&#x27;
}</pre></td>
                  </tr>
                
                  <tr>
                    <td>args</td>
                    <td class="code"><pre>()</pre></td>
                  </tr>
                
                  <tr>
                    <td>cls</td>
                    <td class="code"><pre>&lt;class &#x27;apps.item_purchases.views.ItemPurchaseHistoryView&#x27;&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>handler</td>
                    <td class="code"><pre>&lt;bound method ListModelMixin.list of &lt;apps.item_purchases.views.ItemPurchaseHistoryView object at 0x7fc311cba850&gt;&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>initkwargs</td>
                    <td class="code"><pre>{}</pre></td>
                  </tr>
                
                  <tr>
                    <td>kwargs</td>
                    <td class="code"><pre>{&#x27;user_uuid&#x27;: UUID(&#x27;3fa85f64-5717-4562-b3fc-2c963f66afa6&#x27;)
}</pre></td>
                  </tr>
                
                  <tr>
                    <td>method</td>
                    <td class="code"><pre>&#x27;head&#x27;</pre></td>
                  </tr>
                
                  <tr>
                    <td>request</td>
                    <td class="code"><pre>&lt;WSGIRequest: GET &#x27;/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/&#x27;&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>self</td>
                    <td class="code"><pre>&lt;apps.item_purchases.views.ItemPurchaseHistoryView object at 0x7fc311cba850&gt;</pre></td>
                  </tr>
                
              </tbody>
            </table>
            </details>
          
        </li>
      
        
        <li class="frame user">
          
            <code class="fname">/usr/local/lib/python3.11/site-packages/rest_framework/views.py</code>, line 509, in dispatch
          

          
            <div class="context" id="c140475794002752">
              
                <ol start="502" class="pre-context" id="pre140475794002752">
                
                  <li onclick="toggle('pre140475794002752', 'post140475794002752')"><pre>                                  self.http_method_not_allowed)</pre></li>
                
                  <li onclick="toggle('pre140475794002752', 'post140475794002752')"><pre>            else:</pre></li>
                
                  <li onclick="toggle('pre140475794002752', 'post140475794002752')"><pre>                handler = self.http_method_not_allowed</pre></li>
                
                  <li onclick="toggle('pre140475794002752', 'post140475794002752')"><pre></pre></li>
                
                  <li onclick="toggle('pre140475794002752', 'post140475794002752')"><pre>            response = handler(request, *args, **kwargs)</pre></li>
                
                  <li onclick="toggle('pre140475794002752', 'post140475794002752')"><pre></pre></li>
                
                  <li onclick="toggle('pre140475794002752', 'post140475794002752')"><pre>        except Exception as exc:</pre></li>
                
                </ol>
              
              <ol start="509" class="context-line">
                <li onclick="toggle('pre140475794002752', 'post140475794002752')"><pre>            response = self.handle_exception(exc)</pre> <span>…</span></li>
              </ol>
              
                <ol start='510' class="post-context" id="post140475794002752">
                  
                  <li onclick="toggle('pre140475794002752', 'post140475794002752')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475794002752', 'post140475794002752')"><pre>        self.response = self.finalize_response(request, response, *args, **kwargs)</pre></li>
                  
                  <li onclick="toggle('pre140475794002752', 'post140475794002752')"><pre>        return self.response</pre></li>
                  
                  <li onclick="toggle('pre140475794002752', 'post140475794002752')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475794002752', 'post140475794002752')"><pre>    def options(self, request, *args, **kwargs):</pre></li>
                  
                  <li onclick="toggle('pre140475794002752', 'post140475794002752')"><pre>        &quot;&quot;&quot;</pre></li>
                  
              </ol>
              
            </div>
          

          
            
              <details>
                <summary class="commands">Local vars</summary>
            
            <table class="vars" id="v140475794002752">
              <thead>
                <tr>
                  <th>Variable</th>
                  <th>Value</th>
                </tr>
              </thead>
              <tbody>
                
                  <tr>
                    <td>args</td>
                    <td class="code"><pre>()</pre></td>
                  </tr>
                
                  <tr>
                    <td>handler</td>
                    <td class="code"><pre>&lt;bound method ListModelMixin.list of &lt;apps.item_purchases.views.ItemPurchaseHistoryView object at 0x7fc311cba850&gt;&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>kwargs</td>
                    <td class="code"><pre>{&#x27;user_uuid&#x27;: UUID(&#x27;3fa85f64-5717-4562-b3fc-2c963f66afa6&#x27;)
}</pre></td>
                  </tr>
                
                  <tr>
                    <td>request</td>
                    <td class="code"><pre>&lt;rest_framework.request.Request: GET &#x27;/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/&#x27;&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>self</td>
                    <td class="code"><pre>&lt;apps.item_purchases.views.ItemPurchaseHistoryView object at 0x7fc311cba850&gt;</pre></td>
                  </tr>
                
              </tbody>
            </table>
            </details>
          
        </li>
      
        
        <li class="frame user">
          
            <code class="fname">/usr/local/lib/python3.11/site-packages/rest_framework/views.py</code>, line 469, in handle_exception
          

          
            <div class="context" id="c140475794001216">
              
                <ol start="462" class="pre-context" id="pre140475794001216">
                
                  <li onclick="toggle('pre140475794001216', 'post140475794001216')"><pre></pre></li>
                
                  <li onclick="toggle('pre140475794001216', 'post140475794001216')"><pre>        exception_handler = self.get_exception_handler()</pre></li>
                
                  <li onclick="toggle('pre140475794001216', 'post140475794001216')"><pre></pre></li>
                
                  <li onclick="toggle('pre140475794001216', 'post140475794001216')"><pre>        context = self.get_exception_handler_context()</pre></li>
                
                  <li onclick="toggle('pre140475794001216', 'post140475794001216')"><pre>        response = exception_handler(exc, context)</pre></li>
                
                  <li onclick="toggle('pre140475794001216', 'post140475794001216')"><pre></pre></li>
                
                  <li onclick="toggle('pre140475794001216', 'post140475794001216')"><pre>        if response is None:</pre></li>
                
                </ol>
              
              <ol start="469" class="context-line">
                <li onclick="toggle('pre140475794001216', 'post140475794001216')"><pre>            self.raise_uncaught_exception(exc)</pre> <span>…</span></li>
              </ol>
              
                <ol start='470' class="post-context" id="post140475794001216">
                  
                  <li onclick="toggle('pre140475794001216', 'post140475794001216')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475794001216', 'post140475794001216')"><pre>        response.exception = True</pre></li>
                  
                  <li onclick="toggle('pre140475794001216', 'post140475794001216')"><pre>        return response</pre></li>
                  
                  <li onclick="toggle('pre140475794001216', 'post140475794001216')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475794001216', 'post140475794001216')"><pre>    def raise_uncaught_exception(self, exc):</pre></li>
                  
                  <li onclick="toggle('pre140475794001216', 'post140475794001216')"><pre>        if settings.DEBUG:</pre></li>
                  
              </ol>
              
            </div>
          

          
            
              <details>
                <summary class="commands">Local vars</summary>
            
            <table class="vars" id="v140475794001216">
              <thead>
                <tr>
                  <th>Variable</th>
                  <th>Value</th>
                </tr>
              </thead>
              <tbody>
                
                  <tr>
                    <td>context</td>
                    <td class="code"><pre>{&#x27;args&#x27;: (),
 &#x27;kwargs&#x27;: {&#x27;user_uuid&#x27;: UUID(&#x27;3fa85f64-5717-4562-b3fc-2c963f66afa6&#x27;)
    },
 &#x27;request&#x27;: &lt;rest_framework.request.Request: GET &#x27;/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/&#x27;&gt;,
 &#x27;view&#x27;: &lt;apps.item_purchases.views.ItemPurchaseHistoryView object at 0x7fc311cba850&gt;
}</pre></td>
                  </tr>
                
                  <tr>
                    <td>exc</td>
                    <td class="code"><pre>KeyError(&#x27;&#x27;)</pre></td>
                  </tr>
                
                  <tr>
                    <td>exception_handler</td>
                    <td class="code"><pre>&lt;function post_exception_handler at 0x7fc31352d940&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>response</td>
                    <td class="code"><pre>None</pre></td>
                  </tr>
                
                  <tr>
                    <td>self</td>
                    <td class="code"><pre>&lt;apps.item_purchases.views.ItemPurchaseHistoryView object at 0x7fc311cba850&gt;</pre></td>
                  </tr>
                
              </tbody>
            </table>
            </details>
          
        </li>
      
        
        <li class="frame user">
          
            <code class="fname">/usr/local/lib/python3.11/site-packages/rest_framework/views.py</code>, line 480, in raise_uncaught_exception
          

          
            <div class="context" id="c140475793744192">
              
                <ol start="473" class="pre-context" id="pre140475793744192">
                
                  <li onclick="toggle('pre140475793744192', 'post140475793744192')"><pre></pre></li>
                
                  <li onclick="toggle('pre140475793744192', 'post140475793744192')"><pre>    def raise_uncaught_exception(self, exc):</pre></li>
                
                  <li onclick="toggle('pre140475793744192', 'post140475793744192')"><pre>        if settings.DEBUG:</pre></li>
                
                  <li onclick="toggle('pre140475793744192', 'post140475793744192')"><pre>            request = self.request</pre></li>
                
                  <li onclick="toggle('pre140475793744192', 'post140475793744192')"><pre>            renderer_format = getattr(request.accepted_renderer, &#x27;format&#x27;)</pre></li>
                
                  <li onclick="toggle('pre140475793744192', 'post140475793744192')"><pre>            use_plaintext_traceback = renderer_format not in (&#x27;html&#x27;, &#x27;api&#x27;, &#x27;admin&#x27;)</pre></li>
                
                  <li onclick="toggle('pre140475793744192', 'post140475793744192')"><pre>            request.force_plaintext_errors(use_plaintext_traceback)</pre></li>
                
                </ol>
              
              <ol start="480" class="context-line">
                <li onclick="toggle('pre140475793744192', 'post140475793744192')"><pre>        raise exc</pre> <span>…</span></li>
              </ol>
              
                <ol start='481' class="post-context" id="post140475793744192">
                  
                  <li onclick="toggle('pre140475793744192', 'post140475793744192')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475793744192', 'post140475793744192')"><pre>    # Note: Views are made CSRF exempt from within `as_view` as to prevent</pre></li>
                  
                  <li onclick="toggle('pre140475793744192', 'post140475793744192')"><pre>    # accidental removal of this exemption in cases where `dispatch` needs to</pre></li>
                  
                  <li onclick="toggle('pre140475793744192', 'post140475793744192')"><pre>    # be overridden.</pre></li>
                  
                  <li onclick="toggle('pre140475793744192', 'post140475793744192')"><pre>    def dispatch(self, request, *args, **kwargs):</pre></li>
                  
                  <li onclick="toggle('pre140475793744192', 'post140475793744192')"><pre>        &quot;&quot;&quot;</pre></li>
                  
              </ol>
              
            </div>
          

          
            
              <details>
                <summary class="commands">Local vars</summary>
            
            <table class="vars" id="v140475793744192">
              <thead>
                <tr>
                  <th>Variable</th>
                  <th>Value</th>
                </tr>
              </thead>
              <tbody>
                
                  <tr>
                    <td>exc</td>
                    <td class="code"><pre>KeyError(&#x27;&#x27;)</pre></td>
                  </tr>
                
                  <tr>
                    <td>renderer_format</td>
                    <td class="code"><pre>&#x27;json&#x27;</pre></td>
                  </tr>
                
                  <tr>
                    <td>request</td>
                    <td class="code"><pre>&lt;rest_framework.request.Request: GET &#x27;/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/&#x27;&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>self</td>
                    <td class="code"><pre>&lt;apps.item_purchases.views.ItemPurchaseHistoryView object at 0x7fc311cba850&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>use_plaintext_traceback</td>
                    <td class="code"><pre>True</pre></td>
                  </tr>
                
              </tbody>
            </table>
            </details>
          
        </li>
      
        
        <li class="frame user">
          
            <code class="fname">/usr/local/lib/python3.11/site-packages/rest_framework/views.py</code>, line 506, in dispatch
          

          
            <div class="context" id="c140475794012544">
              
                <ol start="499" class="pre-context" id="pre140475794012544">
                
                  <li onclick="toggle('pre140475794012544', 'post140475794012544')"><pre>            # Get the appropriate handler method</pre></li>
                
                  <li onclick="toggle('pre140475794012544', 'post140475794012544')"><pre>            if request.method.lower() in self.http_method_names:</pre></li>
                
                  <li onclick="toggle('pre140475794012544', 'post140475794012544')"><pre>                handler = getattr(self, request.method.lower(),</pre></li>
                
                  <li onclick="toggle('pre140475794012544', 'post140475794012544')"><pre>                                  self.http_method_not_allowed)</pre></li>
                
                  <li onclick="toggle('pre140475794012544', 'post140475794012544')"><pre>            else:</pre></li>
                
                  <li onclick="toggle('pre140475794012544', 'post140475794012544')"><pre>                handler = self.http_method_not_allowed</pre></li>
                
                  <li onclick="toggle('pre140475794012544', 'post140475794012544')"><pre></pre></li>
                
                </ol>
              
              <ol start="506" class="context-line">
                <li onclick="toggle('pre140475794012544', 'post140475794012544')"><pre>            response = handler(request, *args, **kwargs)</pre> <span>…</span></li>
              </ol>
              
                <ol start='507' class="post-context" id="post140475794012544">
                  
                  <li onclick="toggle('pre140475794012544', 'post140475794012544')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475794012544', 'post140475794012544')"><pre>        except Exception as exc:</pre></li>
                  
                  <li onclick="toggle('pre140475794012544', 'post140475794012544')"><pre>            response = self.handle_exception(exc)</pre></li>
                  
                  <li onclick="toggle('pre140475794012544', 'post140475794012544')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475794012544', 'post140475794012544')"><pre>        self.response = self.finalize_response(request, response, *args, **kwargs)</pre></li>
                  
                  <li onclick="toggle('pre140475794012544', 'post140475794012544')"><pre>        return self.response</pre></li>
                  
              </ol>
              
            </div>
          

          
            
              <details>
                <summary class="commands">Local vars</summary>
            
            <table class="vars" id="v140475794012544">
              <thead>
                <tr>
                  <th>Variable</th>
                  <th>Value</th>
                </tr>
              </thead>
              <tbody>
                
                  <tr>
                    <td>args</td>
                    <td class="code"><pre>()</pre></td>
                  </tr>
                
                  <tr>
                    <td>handler</td>
                    <td class="code"><pre>&lt;bound method ListModelMixin.list of &lt;apps.item_purchases.views.ItemPurchaseHistoryView object at 0x7fc311cba850&gt;&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>kwargs</td>
                    <td class="code"><pre>{&#x27;user_uuid&#x27;: UUID(&#x27;3fa85f64-5717-4562-b3fc-2c963f66afa6&#x27;)
}</pre></td>
                  </tr>
                
                  <tr>
                    <td>request</td>
                    <td class="code"><pre>&lt;rest_framework.request.Request: GET &#x27;/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/&#x27;&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>self</td>
                    <td class="code"><pre>&lt;apps.item_purchases.views.ItemPurchaseHistoryView object at 0x7fc311cba850&gt;</pre></td>
                  </tr>
                
              </tbody>
            </table>
            </details>
          
        </li>
      
        
        <li class="frame user">
          
            <code class="fname">/usr/local/lib/python3.11/site-packages/rest_framework/mixins.py</code>, line 43, in list
          

          
            <div class="context" id="c140475803544896">
              
                <ol start="36" class="pre-context" id="pre140475803544896">
                
                  <li onclick="toggle('pre140475803544896', 'post140475803544896')"><pre>    &quot;&quot;&quot;</pre></li>
                
                  <li onclick="toggle('pre140475803544896', 'post140475803544896')"><pre>    def list(self, request, *args, **kwargs):</pre></li>
                
                  <li onclick="toggle('pre140475803544896', 'post140475803544896')"><pre>        queryset = self.filter_queryset(self.get_queryset())</pre></li>
                
                  <li onclick="toggle('pre140475803544896', 'post140475803544896')"><pre></pre></li>
                
                  <li onclick="toggle('pre140475803544896', 'post140475803544896')"><pre>        page = self.paginate_queryset(queryset)</pre></li>
                
                  <li onclick="toggle('pre140475803544896', 'post140475803544896')"><pre>        if page is not None:</pre></li>
                
                  <li onclick="toggle('pre140475803544896', 'post140475803544896')"><pre>            serializer = self.get_serializer(page, many=True)</pre></li>
                
                </ol>
              
              <ol start="43" class="context-line">
                <li onclick="toggle('pre140475803544896', 'post140475803544896')"><pre>            return self.get_paginated_response(serializer.data)</pre> <span>…</span></li>
              </ol>
              
                <ol start='44' class="post-context" id="post140475803544896">
                  
                  <li onclick="toggle('pre140475803544896', 'post140475803544896')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475803544896', 'post140475803544896')"><pre>        serializer = self.get_serializer(queryset, many=True)</pre></li>
                  
                  <li onclick="toggle('pre140475803544896', 'post140475803544896')"><pre>        return Response(serializer.data)</pre></li>
                  
                  <li onclick="toggle('pre140475803544896', 'post140475803544896')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475803544896', 'post140475803544896')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475803544896', 'post140475803544896')"><pre>class RetrieveModelMixin:</pre></li>
                  
              </ol>
              
            </div>
          

          
            
              <details>
                <summary class="commands">Local vars</summary>
            
            <table class="vars" id="v140475803544896">
              <thead>
                <tr>
                  <th>Variable</th>
                  <th>Value</th>
                </tr>
              </thead>
              <tbody>
                
                  <tr>
                    <td>args</td>
                    <td class="code"><pre>()</pre></td>
                  </tr>
                
                  <tr>
                    <td>kwargs</td>
                    <td class="code"><pre>{&#x27;user_uuid&#x27;: UUID(&#x27;3fa85f64-5717-4562-b3fc-2c963f66afa6&#x27;)
}</pre></td>
                  </tr>
                
                  <tr>
                    <td>page</td>
                    <td class="code"><pre>[&lt;ItemPurchaseHistory: Item_purchase_id: Account from: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 -&gt; Account to: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 Item_uid: 3fa85f64-5717-4562-b3fc-2c963f66afa6Date time of creation: 2023-07-19 09: 05: 00.090829+00: 00&gt;
]</pre></td>
                  </tr>
                
                  <tr>
                    <td>queryset</td>
                    <td class="code"><pre>&lt;QuerySet [&lt;ItemPurchaseHistory: Item_purchase_id: Account from: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 -&gt; Account to: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 Item_uid: 3fa85f64-5717-4562-b3fc-2c963f66afa6Date time of creation: 2023-07-19 09: 05: 00.090829+00: 00&gt;
]&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>request</td>
                    <td class="code"><pre>&lt;rest_framework.request.Request: GET &#x27;/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/&#x27;&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>self</td>
                    <td class="code"><pre>&lt;apps.item_purchases.views.ItemPurchaseHistoryView object at 0x7fc311cba850&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>serializer</td>
                    <td class="code"><pre>ItemPurchaseHistorySerializer([&lt;ItemPurchaseHistory: Item_purchase_id: Account from: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 -&gt; Account to: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 Item_uid: 3fa85f64-5717-4562-b3fc-2c963f66afa6Date time of creation: 2023-07-19 09: 05: 00.090829+00: 00&gt;
], context={&#x27;request&#x27;: &lt;rest_framework.request.Request: GET &#x27;/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/&#x27;&gt;, &#x27;format&#x27;: None, &#x27;view&#x27;: &lt;apps.item_purchases.views.ItemPurchaseHistoryView object&gt;
}, many=True):
    history_id = IntegerField(source=&#x27;id&#x27;)
    offer_uuid = UUIDField(source=&#x27;item_purchase_id.item_uuid&#x27;)
    price = MoneySerializer(source=&#x27;item_purchase_id.item_price&#x27;):
        amount = DecimalField(decimal_places=2, max_digits=11, min_value=0)
        currency = EnumField(choices=&lt;enum &#x27;Currencies&#x27;&gt;)
    purchase_type = SerializerMethodField()
    status = SerializerMethodField()
    created_at = DateTimeField(source=&#x27;created_date&#x27;)</pre></td>
                  </tr>
                
              </tbody>
            </table>
            </details>
          
        </li>
      
        
        <li class="frame user">
          
            <code class="fname">/usr/local/lib/python3.11/site-packages/rest_framework/serializers.py</code>, line 768, in data
          

          
            <div class="context" id="c140475803661312">
              
                <ol start="761" class="pre-context" id="pre140475803661312">
                
                  <li onclick="toggle('pre140475803661312', 'post140475803661312')"><pre>        return representation.list_repr(self, indent=1)</pre></li>
                
                  <li onclick="toggle('pre140475803661312', 'post140475803661312')"><pre></pre></li>
                
                  <li onclick="toggle('pre140475803661312', 'post140475803661312')"><pre>    # Include a backlink to the serializer class on return objects.</pre></li>
                
                  <li onclick="toggle('pre140475803661312', 'post140475803661312')"><pre>    # Allows renderers such as HTMLFormRenderer to get the full field info.</pre></li>
                
                  <li onclick="toggle('pre140475803661312', 'post140475803661312')"><pre></pre></li>
                
                  <li onclick="toggle('pre140475803661312', 'post140475803661312')"><pre>    @property</pre></li>
                
                  <li onclick="toggle('pre140475803661312', 'post140475803661312')"><pre>    def data(self):</pre></li>
                
                </ol>
              
              <ol start="768" class="context-line">
                <li onclick="toggle('pre140475803661312', 'post140475803661312')"><pre>        ret = super().data</pre> <span>…</span></li>
              </ol>
              
                <ol start='769' class="post-context" id="post140475803661312">
                  
                  <li onclick="toggle('pre140475803661312', 'post140475803661312')"><pre>        return ReturnList(ret, serializer=self)</pre></li>
                  
                  <li onclick="toggle('pre140475803661312', 'post140475803661312')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475803661312', 'post140475803661312')"><pre>    @property</pre></li>
                  
                  <li onclick="toggle('pre140475803661312', 'post140475803661312')"><pre>    def errors(self):</pre></li>
                  
                  <li onclick="toggle('pre140475803661312', 'post140475803661312')"><pre>        ret = super().errors</pre></li>
                  
                  <li onclick="toggle('pre140475803661312', 'post140475803661312')"><pre>        if isinstance(ret, list) and len(ret) == 1 and getattr(ret[
    0
], &#x27;code&#x27;, None) == &#x27;null&#x27;:</pre></li>
                  
              </ol>
              
            </div>
          

          
            
              <details>
                <summary class="commands">Local vars</summary>
            
            <table class="vars" id="v140475803661312">
              <thead>
                <tr>
                  <th>Variable</th>
                  <th>Value</th>
                </tr>
              </thead>
              <tbody>
                
                  <tr>
                    <td>__class__</td>
                    <td class="code"><pre>&lt;class &#x27;rest_framework.serializers.ListSerializer&#x27;&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>self</td>
                    <td class="code"><pre>ItemPurchaseHistorySerializer([&lt;ItemPurchaseHistory: Item_purchase_id: Account from: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 -&gt; Account to: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 Item_uid: 3fa85f64-5717-4562-b3fc-2c963f66afa6Date time of creation: 2023-07-19 09: 05: 00.090829+00: 00&gt;
], context={&#x27;request&#x27;: &lt;rest_framework.request.Request: GET &#x27;/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/&#x27;&gt;, &#x27;format&#x27;: None, &#x27;view&#x27;: &lt;apps.item_purchases.views.ItemPurchaseHistoryView object&gt;
}, many=True):
    history_id = IntegerField(source=&#x27;id&#x27;)
    offer_uuid = UUIDField(source=&#x27;item_purchase_id.item_uuid&#x27;)
    price = MoneySerializer(source=&#x27;item_purchase_id.item_price&#x27;):
        amount = DecimalField(decimal_places=2, max_digits=11, min_value=0)
        currency = EnumField(choices=&lt;enum &#x27;Currencies&#x27;&gt;)
    purchase_type = SerializerMethodField()
    status = SerializerMethodField()
    created_at = DateTimeField(source=&#x27;created_date&#x27;)</pre></td>
                  </tr>
                
              </tbody>
            </table>
            </details>
          
        </li>
      
        
        <li class="frame user">
          
            <code class="fname">/usr/local/lib/python3.11/site-packages/rest_framework/serializers.py</code>, line 253, in data
          

          
            <div class="context" id="c140475803664064">
              
                <ol start="246" class="pre-context" id="pre140475803664064">
                
                  <li onclick="toggle('pre140475803664064', 'post140475803664064')"><pre>                &#x27;You should either call `.is_valid()` first, &#x27;</pre></li>
                
                  <li onclick="toggle('pre140475803664064', 'post140475803664064')"><pre>                &#x27;or access `.initial_data` instead.&#x27;</pre></li>
                
                  <li onclick="toggle('pre140475803664064', 'post140475803664064')"><pre>            )</pre></li>
                
                  <li onclick="toggle('pre140475803664064', 'post140475803664064')"><pre>            raise AssertionError(msg)</pre></li>
                
                  <li onclick="toggle('pre140475803664064', 'post140475803664064')"><pre></pre></li>
                
                  <li onclick="toggle('pre140475803664064', 'post140475803664064')"><pre>        if not hasattr(self, &#x27;_data&#x27;):</pre></li>
                
                  <li onclick="toggle('pre140475803664064', 'post140475803664064')"><pre>            if self.instance is not None and not getattr(self, &#x27;_errors&#x27;, None):</pre></li>
                
                </ol>
              
              <ol start="253" class="context-line">
                <li onclick="toggle('pre140475803664064', 'post140475803664064')"><pre>                self._data = self.to_representation(self.instance)</pre> <span>…</span></li>
              </ol>
              
                <ol start='254' class="post-context" id="post140475803664064">
                  
                  <li onclick="toggle('pre140475803664064', 'post140475803664064')"><pre>            elif hasattr(self, &#x27;_validated_data&#x27;) and not getattr(self, &#x27;_errors&#x27;, None):</pre></li>
                  
                  <li onclick="toggle('pre140475803664064', 'post140475803664064')"><pre>                self._data = self.to_representation(self.validated_data)</pre></li>
                  
                  <li onclick="toggle('pre140475803664064', 'post140475803664064')"><pre>            else:</pre></li>
                  
                  <li onclick="toggle('pre140475803664064', 'post140475803664064')"><pre>                self._data = self.get_initial()</pre></li>
                  
                  <li onclick="toggle('pre140475803664064', 'post140475803664064')"><pre>        return self._data</pre></li>
                  
                  <li onclick="toggle('pre140475803664064', 'post140475803664064')"><pre></pre></li>
                  
              </ol>
              
            </div>
          

          
            
              <details>
                <summary class="commands">Local vars</summary>
            
            <table class="vars" id="v140475803664064">
              <thead>
                <tr>
                  <th>Variable</th>
                  <th>Value</th>
                </tr>
              </thead>
              <tbody>
                
                  <tr>
                    <td>self</td>
                    <td class="code"><pre>ItemPurchaseHistorySerializer([&lt;ItemPurchaseHistory: Item_purchase_id: Account from: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 -&gt; Account to: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 Item_uid: 3fa85f64-5717-4562-b3fc-2c963f66afa6Date time of creation: 2023-07-19 09: 05: 00.090829+00: 00&gt;
], context={&#x27;request&#x27;: &lt;rest_framework.request.Request: GET &#x27;/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/&#x27;&gt;, &#x27;format&#x27;: None, &#x27;view&#x27;: &lt;apps.item_purchases.views.ItemPurchaseHistoryView object&gt;
}, many=True):
    history_id = IntegerField(source=&#x27;id&#x27;)
    offer_uuid = UUIDField(source=&#x27;item_purchase_id.item_uuid&#x27;)
    price = MoneySerializer(source=&#x27;item_purchase_id.item_price&#x27;):
        amount = DecimalField(decimal_places=2, max_digits=11, min_value=0)
        currency = EnumField(choices=&lt;enum &#x27;Currencies&#x27;&gt;)
    purchase_type = SerializerMethodField()
    status = SerializerMethodField()
    created_at = DateTimeField(source=&#x27;created_date&#x27;)</pre></td>
                  </tr>
                
              </tbody>
            </table>
            </details>
          
        </li>
      
        
        <li class="frame user">
          
            <code class="fname">/usr/local/lib/python3.11/site-packages/rest_framework/serializers.py</code>, line 686, in to_representation
          

          
            <div class="context" id="c140475793918272">
              
                <ol start="679" class="pre-context" id="pre140475793918272">
                
                  <li onclick="toggle('pre140475793918272', 'post140475793918272')"><pre>        &quot;&quot;&quot;</pre></li>
                
                  <li onclick="toggle('pre140475793918272', 'post140475793918272')"><pre>        List of object instances -&gt; List of dicts of primitive datatypes.</pre></li>
                
                  <li onclick="toggle('pre140475793918272', 'post140475793918272')"><pre>        &quot;&quot;&quot;</pre></li>
                
                  <li onclick="toggle('pre140475793918272', 'post140475793918272')"><pre>        # Dealing with nested relationships, data can be a Manager,</pre></li>
                
                  <li onclick="toggle('pre140475793918272', 'post140475793918272')"><pre>        # so, first get a queryset from the Manager if needed</pre></li>
                
                  <li onclick="toggle('pre140475793918272', 'post140475793918272')"><pre>        iterable = data.all() if isinstance(data, models.Manager) else data</pre></li>
                
                  <li onclick="toggle('pre140475793918272', 'post140475793918272')"><pre></pre></li>
                
                </ol>
              
              <ol start="686" class="context-line">
                <li onclick="toggle('pre140475793918272', 'post140475793918272')"><pre>        return [</pre> <span>…</span></li>
              </ol>
              
                <ol start='687' class="post-context" id="post140475793918272">
                  
                  <li onclick="toggle('pre140475793918272', 'post140475793918272')"><pre>            self.child.to_representation(item) for item in iterable</pre></li>
                  
                  <li onclick="toggle('pre140475793918272', 'post140475793918272')"><pre>
]</pre></li>
                  
                  <li onclick="toggle('pre140475793918272', 'post140475793918272')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475793918272', 'post140475793918272')"><pre>    def validate(self, attrs):</pre></li>
                  
                  <li onclick="toggle('pre140475793918272', 'post140475793918272')"><pre>        return attrs</pre></li>
                  
                  <li onclick="toggle('pre140475793918272', 'post140475793918272')"><pre></pre></li>
                  
              </ol>
              
            </div>
          

          
            
              <details>
                <summary class="commands">Local vars</summary>
            
            <table class="vars" id="v140475793918272">
              <thead>
                <tr>
                  <th>Variable</th>
                  <th>Value</th>
                </tr>
              </thead>
              <tbody>
                
                  <tr>
                    <td>data</td>
                    <td class="code"><pre>[&lt;ItemPurchaseHistory: Item_purchase_id: Account from: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 -&gt; Account to: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 Item_uid: 3fa85f64-5717-4562-b3fc-2c963f66afa6Date time of creation: 2023-07-19 09: 05: 00.090829+00: 00&gt;
]</pre></td>
                  </tr>
                
                  <tr>
                    <td>iterable</td>
                    <td class="code"><pre>[&lt;ItemPurchaseHistory: Item_purchase_id: Account from: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 -&gt; Account to: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 Item_uid: 3fa85f64-5717-4562-b3fc-2c963f66afa6Date time of creation: 2023-07-19 09: 05: 00.090829+00: 00&gt;
]</pre></td>
                  </tr>
                
                  <tr>
                    <td>self</td>
                    <td class="code"><pre>ItemPurchaseHistorySerializer([&lt;ItemPurchaseHistory: Item_purchase_id: Account from: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 -&gt; Account to: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 Item_uid: 3fa85f64-5717-4562-b3fc-2c963f66afa6Date time of creation: 2023-07-19 09: 05: 00.090829+00: 00&gt;
], context={&#x27;request&#x27;: &lt;rest_framework.request.Request: GET &#x27;/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/&#x27;&gt;, &#x27;format&#x27;: None, &#x27;view&#x27;: &lt;apps.item_purchases.views.ItemPurchaseHistoryView object&gt;
}, many=True):
    history_id = IntegerField(source=&#x27;id&#x27;)
    offer_uuid = UUIDField(source=&#x27;item_purchase_id.item_uuid&#x27;)
    price = MoneySerializer(source=&#x27;item_purchase_id.item_price&#x27;):
        amount = DecimalField(decimal_places=2, max_digits=11, min_value=0)
        currency = EnumField(choices=&lt;enum &#x27;Currencies&#x27;&gt;)
    purchase_type = SerializerMethodField()
    status = SerializerMethodField()
    created_at = DateTimeField(source=&#x27;created_date&#x27;)</pre></td>
                  </tr>
                
              </tbody>
            </table>
            </details>
          
        </li>
      
        
        <li class="frame user">
          
            <code class="fname">/usr/local/lib/python3.11/site-packages/rest_framework/serializers.py</code>, line 687, in &lt;listcomp&gt;
          

          
            <div class="context" id="c140475803765632">
              
                <ol start="680" class="pre-context" id="pre140475803765632">
                
                  <li onclick="toggle('pre140475803765632', 'post140475803765632')"><pre>        List of object instances -&gt; List of dicts of primitive datatypes.</pre></li>
                
                  <li onclick="toggle('pre140475803765632', 'post140475803765632')"><pre>        &quot;&quot;&quot;</pre></li>
                
                  <li onclick="toggle('pre140475803765632', 'post140475803765632')"><pre>        # Dealing with nested relationships, data can be a Manager,</pre></li>
                
                  <li onclick="toggle('pre140475803765632', 'post140475803765632')"><pre>        # so, first get a queryset from the Manager if needed</pre></li>
                
                  <li onclick="toggle('pre140475803765632', 'post140475803765632')"><pre>        iterable = data.all() if isinstance(data, models.Manager) else data</pre></li>
                
                  <li onclick="toggle('pre140475803765632', 'post140475803765632')"><pre></pre></li>
                
                  <li onclick="toggle('pre140475803765632', 'post140475803765632')"><pre>        return [</pre></li>
                
                </ol>
              
              <ol start="687" class="context-line">
                <li onclick="toggle('pre140475803765632', 'post140475803765632')"><pre>            self.child.to_representation(item) for item in iterable</pre> <span>…</span></li>
              </ol>
              
                <ol start='688' class="post-context" id="post140475803765632">
                  
                  <li onclick="toggle('pre140475803765632', 'post140475803765632')"><pre>
]</pre></li>
                  
                  <li onclick="toggle('pre140475803765632', 'post140475803765632')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475803765632', 'post140475803765632')"><pre>    def validate(self, attrs):</pre></li>
                  
                  <li onclick="toggle('pre140475803765632', 'post140475803765632')"><pre>        return attrs</pre></li>
                  
                  <li onclick="toggle('pre140475803765632', 'post140475803765632')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475803765632', 'post140475803765632')"><pre>    def update(self, instance, validated_data):</pre></li>
                  
              </ol>
              
            </div>
          

          
            
              <details>
                <summary class="commands">Local vars</summary>
            
            <table class="vars" id="v140475803765632">
              <thead>
                <tr>
                  <th>Variable</th>
                  <th>Value</th>
                </tr>
              </thead>
              <tbody>
                
                  <tr>
                    <td>.0</td>
                    <td class="code"><pre>&lt;list_iterator object at 0x7fc311d056f0&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>item</td>
                    <td class="code"><pre>&lt;ItemPurchaseHistory: Item_purchase_id: Account from: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 -&gt; Account to: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 Item_uid: 3fa85f64-5717-4562-b3fc-2c963f66afa6Date time of creation: 2023-07-19 09: 05: 00.090829+00: 00&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>self</td>
                    <td class="code"><pre>ItemPurchaseHistorySerializer([&lt;ItemPurchaseHistory: Item_purchase_id: Account from: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 -&gt; Account to: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 Item_uid: 3fa85f64-5717-4562-b3fc-2c963f66afa6Date time of creation: 2023-07-19 09: 05: 00.090829+00: 00&gt;
], context={&#x27;request&#x27;: &lt;rest_framework.request.Request: GET &#x27;/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/&#x27;&gt;, &#x27;format&#x27;: None, &#x27;view&#x27;: &lt;apps.item_purchases.views.ItemPurchaseHistoryView object&gt;
}, many=True):
    history_id = IntegerField(source=&#x27;id&#x27;)
    offer_uuid = UUIDField(source=&#x27;item_purchase_id.item_uuid&#x27;)
    price = MoneySerializer(source=&#x27;item_purchase_id.item_price&#x27;):
        amount = DecimalField(decimal_places=2, max_digits=11, min_value=0)
        currency = EnumField(choices=&lt;enum &#x27;Currencies&#x27;&gt;)
    purchase_type = SerializerMethodField()
    status = SerializerMethodField()
    created_at = DateTimeField(source=&#x27;created_date&#x27;)</pre></td>
                  </tr>
                
              </tbody>
            </table>
            </details>
          
        </li>
      
        
        <li class="frame user">
          
            <code class="fname">/usr/local/lib/python3.11/site-packages/rest_framework/serializers.py</code>, line 522, in to_representation
          

          
            <div class="context" id="c140475803059584">
              
                <ol start="515" class="pre-context" id="pre140475803059584">
                
                  <li onclick="toggle('pre140475803059584', 'post140475803059584')"><pre>            #</pre></li>
                
                  <li onclick="toggle('pre140475803059584', 'post140475803059584')"><pre>            # For related fields with `use_pk_only_optimization` we need to</pre></li>
                
                  <li onclick="toggle('pre140475803059584', 'post140475803059584')"><pre>            # resolve the pk value.</pre></li>
                
                  <li onclick="toggle('pre140475803059584', 'post140475803059584')"><pre>            check_for_none = attribute.pk if isinstance(attribute, PKOnlyObject) else attribute</pre></li>
                
                  <li onclick="toggle('pre140475803059584', 'post140475803059584')"><pre>            if check_for_none is None:</pre></li>
                
                  <li onclick="toggle('pre140475803059584', 'post140475803059584')"><pre>                ret[field.field_name
] = None</pre></li>
                
                  <li onclick="toggle('pre140475803059584', 'post140475803059584')"><pre>            else:</pre></li>
                
                </ol>
              
              <ol start="522" class="context-line">
                <li onclick="toggle('pre140475803059584', 'post140475803059584')"><pre>                ret[field.field_name
] = field.to_representation(attribute)</pre> <span>…</span></li>
              </ol>
              
                <ol start='523' class="post-context" id="post140475803059584">
                  
                  <li onclick="toggle('pre140475803059584', 'post140475803059584')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475803059584', 'post140475803059584')"><pre>        return ret</pre></li>
                  
                  <li onclick="toggle('pre140475803059584', 'post140475803059584')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475803059584', 'post140475803059584')"><pre>    def validate(self, attrs):</pre></li>
                  
                  <li onclick="toggle('pre140475803059584', 'post140475803059584')"><pre>        return attrs</pre></li>
                  
                  <li onclick="toggle('pre140475803059584', 'post140475803059584')"><pre></pre></li>
                  
              </ol>
              
            </div>
          

          
            
              <details>
                <summary class="commands">Local vars</summary>
            
            <table class="vars" id="v140475803059584">
              <thead>
                <tr>
                  <th>Variable</th>
                  <th>Value</th>
                </tr>
              </thead>
              <tbody>
                
                  <tr>
                    <td>attribute</td>
                    <td class="code"><pre>&lt;ItemPurchaseHistory: Item_purchase_id: Account from: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 -&gt; Account to: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 Item_uid: 3fa85f64-5717-4562-b3fc-2c963f66afa6Date time of creation: 2023-07-19 09: 05: 00.090829+00: 00&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>check_for_none</td>
                    <td class="code"><pre>&lt;ItemPurchaseHistory: Item_purchase_id: Account from: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 -&gt; Account to: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 Item_uid: 3fa85f64-5717-4562-b3fc-2c963f66afa6Date time of creation: 2023-07-19 09: 05: 00.090829+00: 00&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>field</td>
                    <td class="code"><pre>SerializerMethodField()</pre></td>
                  </tr>
                
                  <tr>
                    <td>fields</td>
                    <td class="code"><pre>&lt;generator object Serializer._readable_fields at 0x7fc311b3d080&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>instance</td>
                    <td class="code"><pre>&lt;ItemPurchaseHistory: Item_purchase_id: Account from: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 -&gt; Account to: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 Item_uid: 3fa85f64-5717-4562-b3fc-2c963f66afa6Date time of creation: 2023-07-19 09: 05: 00.090829+00: 00&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>ret</td>
                    <td class="code"><pre>OrderedDict([(&#x27;history_id&#x27;,
    1),
             (&#x27;offer_uuid&#x27;, &#x27;3fa85f64-5717-4562-b3fc-2c963f66afa6&#x27;),
             (&#x27;price&#x27;,
              OrderedDict([(&#x27;amount&#x27;, &#x27;100.00&#x27;),
                           (&#x27;currency&#x27;, &#x27;Russian Ruble&#x27;)
    ])),
             (&#x27;purchase_type&#x27;, &#x27;for_self&#x27;)
])</pre></td>
                  </tr>
                
                  <tr>
                    <td>self</td>
                    <td class="code"><pre>ItemPurchaseHistorySerializer([&lt;ItemPurchaseHistory: Item_purchase_id: Account from: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 -&gt; Account to: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 Item_uid: 3fa85f64-5717-4562-b3fc-2c963f66afa6Date time of creation: 2023-07-19 09: 05: 00.090829+00: 00&gt;
], context={&#x27;request&#x27;: &lt;rest_framework.request.Request: GET &#x27;/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/&#x27;&gt;, &#x27;format&#x27;: None, &#x27;view&#x27;: &lt;apps.item_purchases.views.ItemPurchaseHistoryView object&gt;
}):
    history_id = IntegerField(source=&#x27;id&#x27;)
    offer_uuid = UUIDField(source=&#x27;item_purchase_id.item_uuid&#x27;)
    price = MoneySerializer(source=&#x27;item_purchase_id.item_price&#x27;):
        amount = DecimalField(decimal_places=2, max_digits=11, min_value=0)
        currency = EnumField(choices=&lt;enum &#x27;Currencies&#x27;&gt;)
    purchase_type = SerializerMethodField()
    status = SerializerMethodField()
    created_at = DateTimeField(source=&#x27;created_date&#x27;)</pre></td>
                  </tr>
                
              </tbody>
            </table>
            </details>
          
        </li>
      
        
        <li class="frame user">
          
            <code class="fname">/usr/local/lib/python3.11/site-packages/rest_framework/fields.py</code>, line 1838, in to_representation
          

          
            <div class="context" id="c140475803067712">
              
                <ol start="1831" class="pre-context" id="pre140475803067712">
                
                  <li onclick="toggle('pre140475803067712', 'post140475803067712')"><pre>        if self.method_name is None:</pre></li>
                
                  <li onclick="toggle('pre140475803067712', 'post140475803067712')"><pre>            self.method_name = &#x27;get_{field_name
}&#x27;.format(field_name=field_name)</pre></li>
                
                  <li onclick="toggle('pre140475803067712', 'post140475803067712')"><pre></pre></li>
                
                  <li onclick="toggle('pre140475803067712', 'post140475803067712')"><pre>        super().bind(field_name, parent)</pre></li>
                
                  <li onclick="toggle('pre140475803067712', 'post140475803067712')"><pre></pre></li>
                
                  <li onclick="toggle('pre140475803067712', 'post140475803067712')"><pre>    def to_representation(self, value):</pre></li>
                
                  <li onclick="toggle('pre140475803067712', 'post140475803067712')"><pre>        method = getattr(self.parent, self.method_name)</pre></li>
                
                </ol>
              
              <ol start="1838" class="context-line">
                <li onclick="toggle('pre140475803067712', 'post140475803067712')"><pre>        return method(value)</pre> <span>…</span></li>
              </ol>
              
                <ol start='1839' class="post-context" id="post140475803067712">
                  
                  <li onclick="toggle('pre140475803067712', 'post140475803067712')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475803067712', 'post140475803067712')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475803067712', 'post140475803067712')"><pre>class ModelField(Field):</pre></li>
                  
                  <li onclick="toggle('pre140475803067712', 'post140475803067712')"><pre>    &quot;&quot;&quot;</pre></li>
                  
                  <li onclick="toggle('pre140475803067712', 'post140475803067712')"><pre>    A generic field that can be used against an arbitrary model field.</pre></li>
                  
                  <li onclick="toggle('pre140475803067712', 'post140475803067712')"><pre></pre></li>
                  
              </ol>
              
            </div>
          

          
            
              <details>
                <summary class="commands">Local vars</summary>
            
            <table class="vars" id="v140475803067712">
              <thead>
                <tr>
                  <th>Variable</th>
                  <th>Value</th>
                </tr>
              </thead>
              <tbody>
                
                  <tr>
                    <td>method</td>
                    <td class="code"><pre>&lt;bound method ItemPurchaseHistorySerializer.get_status of ItemPurchaseHistorySerializer([&lt;ItemPurchaseHistory: Item_purchase_id: Account from: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 -&gt; Account to: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 Item_uid: 3fa85f64-5717-4562-b3fc-2c963f66afa6Date time of creation: 2023-07-19 09: 05: 00.090829+00: 00&gt;
], context={&#x27;request&#x27;: &lt;rest_framework.request.Request: GET &#x27;/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/&#x27;&gt;, &#x27;format&#x27;: None, &#x27;view&#x27;: &lt;apps.item_purchases.views.ItemPurchaseHistoryView object&gt;
}):
    history_id = IntegerField(source=&#x27;id&#x27;)
    offer_uuid = UUIDField(source=&#x27;item_purchase_id.item_uuid&#x27;)
    price = MoneySerializer(source=&#x27;item_purchase_id.item_price&#x27;):
        amount = DecimalField(decimal_places=2, max_digits=11, min_value=0)
        currency = EnumField(choices=&lt;enum &#x27;Currencies&#x27;&gt;)
    purchase_type = SerializerMethodField()
    status = SerializerMethodField()
    created_at = DateTimeField(source=&#x27;created_date&#x27;)&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>self</td>
                    <td class="code"><pre>SerializerMethodField()</pre></td>
                  </tr>
                
                  <tr>
                    <td>value</td>
                    <td class="code"><pre>&lt;ItemPurchaseHistory: Item_purchase_id: Account from: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 -&gt; Account to: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 Item_uid: 3fa85f64-5717-4562-b3fc-2c963f66afa6Date time of creation: 2023-07-19 09: 05: 00.090829+00: 00&gt;</pre></td>
                  </tr>
                
              </tbody>
            </table>
            </details>
          
        </li>
      
        
        <li class="frame user">
          
            <code class="fname">/home/app/web/apps/item_purchases/serializers.py</code>, line 60, in get_status
          

          
            <div class="context" id="c140475794039616">
              
                <ol start="53" class="pre-context" id="pre140475794039616">
                
                  <li onclick="toggle('pre140475794039616', 'post140475794039616')"><pre>    def get_status(self, obj: ItemPurchaseHistory):</pre></li>
                
                  <li onclick="toggle('pre140475794039616', 'post140475794039616')"><pre>        _status = obj.item_purchase_id.status</pre></li>
                
                  <li onclick="toggle('pre140475794039616', 'post140475794039616')"><pre>        if (</pre></li>
                
                  <li onclick="toggle('pre140475794039616', 'post140475794039616')"><pre>            _status == ItemPurchase.ItemPurchaseStatus.REFUNDED</pre></li>
                
                  <li onclick="toggle('pre140475794039616', 'post140475794039616')"><pre>            and obj.event_type == obj.ItemPurchaseType.CREATED</pre></li>
                
                  <li onclick="toggle('pre140475794039616', 'post140475794039616')"><pre>        ):</pre></li>
                
                  <li onclick="toggle('pre140475794039616', 'post140475794039616')"><pre>            return ItemPurchase.ItemPurchaseStatus.PAID.label.lower()</pre></li>
                
                </ol>
              
              <ol start="60" class="context-line">
                <li onclick="toggle('pre140475794039616', 'post140475794039616')"><pre>        return self.STATUSES[_status
]</pre> <span>…</span></li>
              </ol>
              
                <ol start='61' class="post-context" id="post140475794039616">
                  
                  <li onclick="toggle('pre140475794039616', 'post140475794039616')"><pre></pre></li>
                  
                  <li onclick="toggle('pre140475794039616', 'post140475794039616')"><pre>    def get_purchase_type(self, obj: ItemPurchaseHistory):</pre></li>
                  
                  <li onclick="toggle('pre140475794039616', 'post140475794039616')"><pre>        if obj.item_purchase_id.account_from != obj.item_purchase_id.account_to:</pre></li>
                  
                  <li onclick="toggle('pre140475794039616', 'post140475794039616')"><pre>            return &#x27;gift&#x27;</pre></li>
                  
                  <li onclick="toggle('pre140475794039616', 'post140475794039616')"><pre>        return &#x27;for_self&#x27;</pre></li>
                  
              </ol>
              
            </div>
          

          
            
              <details>
                <summary class="commands">Local vars</summary>
            
            <table class="vars" id="v140475794039616">
              <thead>
                <tr>
                  <th>Variable</th>
                  <th>Value</th>
                </tr>
              </thead>
              <tbody>
                
                  <tr>
                    <td>_status</td>
                    <td class="code"><pre>&#x27;&#x27;</pre></td>
                  </tr>
                
                  <tr>
                    <td>obj</td>
                    <td class="code"><pre>&lt;ItemPurchaseHistory: Item_purchase_id: Account from: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 -&gt; Account to: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 Item_uid: 3fa85f64-5717-4562-b3fc-2c963f66afa6Date time of creation: 2023-07-19 09: 05: 00.090829+00: 00&gt;</pre></td>
                  </tr>
                
                  <tr>
                    <td>self</td>
                    <td class="code"><pre>ItemPurchaseHistorySerializer([&lt;ItemPurchaseHistory: Item_purchase_id: Account from: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 -&gt; Account to: User uuid: 3fa85f64-5717-4562-b3fc-2c963f66afa6 Item_uid: 3fa85f64-5717-4562-b3fc-2c963f66afa6Date time of creation: 2023-07-19 09: 05: 00.090829+00: 00&gt;
], context={&#x27;request&#x27;: &lt;rest_framework.request.Request: GET &#x27;/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/&#x27;&gt;, &#x27;format&#x27;: None, &#x27;view&#x27;: &lt;apps.item_purchases.views.ItemPurchaseHistoryView object&gt;
}):
    history_id = IntegerField(source=&#x27;id&#x27;)
    offer_uuid = UUIDField(source=&#x27;item_purchase_id.item_uuid&#x27;)
    price = MoneySerializer(source=&#x27;item_purchase_id.item_price&#x27;):
        amount = DecimalField(decimal_places=2, max_digits=11, min_value=0)
        currency = EnumField(choices=&lt;enum &#x27;Currencies&#x27;&gt;)
    purchase_type = SerializerMethodField()
    status = SerializerMethodField()
    created_at = DateTimeField(source=&#x27;created_date&#x27;)</pre></td>
                  </tr>
                
              </tbody>
            </table>
            </details>
          
        </li>
      
    </ul>
  </div>

  <form action="https://dpaste.com/" name="pasteform" id="pasteform" method="post">
  <div id="pastebinTraceback" class="pastebin">
    <input type="hidden" name="language" value="PythonConsole">
    <input type="hidden" name="title"
      value="KeyError at /api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/">
    <input type="hidden" name="source" value="Django Dpaste Agent">
    <input type="hidden" name="poster" value="Django">
    <textarea name="content" id="traceback_area" cols="140" rows="25">
Environment:


Request Method: GET
Request URL: http: //payments.alpha.g-spot.website/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/

Django Version: 4.1.7
Python Version: 3.11.4
Installed Applications: [&#x27;django.contrib.admin&#x27;,
 &#x27;django.contrib.auth&#x27;,
 &#x27;django.contrib.contenttypes&#x27;,
 &#x27;django.contrib.sessions&#x27;,
 &#x27;django.contrib.messages&#x27;,
 &#x27;django.contrib.staticfiles&#x27;,
 &#x27;djmoney&#x27;,
 &#x27;django_extensions&#x27;,
 &#x27;drf_spectacular&#x27;,
 &#x27;rest_framework&#x27;,
 &#x27;apps.payment_accounts&#x27;,
 &#x27;apps.item_purchases&#x27;,
 &#x27;apps.external_payments&#x27;
]
Installed Middleware: [&#x27;django.middleware.security.SecurityMiddleware&#x27;,
 &#x27;django.contrib.sessions.middleware.SessionMiddleware&#x27;,
 &#x27;django.middleware.common.CommonMiddleware&#x27;,
 &#x27;django.middleware.csrf.CsrfViewMiddleware&#x27;,
 &#x27;django.contrib.auth.middleware.AuthenticationMiddleware&#x27;,
 &#x27;django.contrib.messages.middleware.MessageMiddleware&#x27;,
 &#x27;django.middleware.clickjacking.XFrameOptionsMiddleware&#x27;,
 &#x27;rollbar.contrib.django.middleware.RollbarNotifierMiddleware&#x27;
]



Traceback (most recent call last):
  File "/usr/local/lib/python3.11/site-packages/django/core/handlers/exception.py", line 56, in inner
    response = get_response(request)
  File "/usr/local/lib/python3.11/site-packages/django/core/handlers/base.py", line 197, in _get_response
    response = wrapped_callback(request, *callback_args, **callback_kwargs)
  File "/usr/local/lib/python3.11/site-packages/django/views/decorators/csrf.py", line 55, in wrapped_view
    return view_func(*args, **kwargs)
  File "/usr/local/lib/python3.11/site-packages/rest_framework/viewsets.py", line 125, in view
    return self.dispatch(request, *args, **kwargs)
  File "/usr/local/lib/python3.11/site-packages/rest_framework/views.py", line 509, in dispatch
    response = self.handle_exception(exc)
  File "/usr/local/lib/python3.11/site-packages/rest_framework/views.py", line 469, in handle_exception
    self.raise_uncaught_exception(exc)
  File "/usr/local/lib/python3.11/site-packages/rest_framework/views.py", line 480, in raise_uncaught_exception
    raise exc
  File "/usr/local/lib/python3.11/site-packages/rest_framework/views.py", line 506, in dispatch
    response = handler(request, *args, **kwargs)
  File "/usr/local/lib/python3.11/site-packages/rest_framework/mixins.py", line 43, in list
    return self.get_paginated_response(serializer.data)
  File "/usr/local/lib/python3.11/site-packages/rest_framework/serializers.py", line 768, in data
    ret = super().data
  File "/usr/local/lib/python3.11/site-packages/rest_framework/serializers.py", line 253, in data
    self._data = self.to_representation(self.instance)
  File "/usr/local/lib/python3.11/site-packages/rest_framework/serializers.py", line 686, in to_representation
    return [
  File "/usr/local/lib/python3.11/site-packages/rest_framework/serializers.py", line 687, in &lt;listcomp&gt;
    self.child.to_representation(item) for item in iterable
  File "/usr/local/lib/python3.11/site-packages/rest_framework/serializers.py", line 522, in to_representation
    ret[field.field_name
    ] = field.to_representation(attribute)
  File "/usr/local/lib/python3.11/site-packages/rest_framework/fields.py", line 1838, in to_representation
    return method(value)
  File "/home/app/web/apps/item_purchases/serializers.py", line 60, in get_status
    return self.STATUSES[_status
    ]

Exception Type: KeyError at /api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/
Exception Value: &#x27;&#x27;
</textarea>
  <br><br>
  <input type="submit" value="Share this traceback on a public website">
  </div>
</form>

</div>


<div id="requestinfo">
  <h2>Request information</h2>


  
    <h3 id="user-info">USER</h3>
    <p>AnonymousUser</p>
  

  <h3 id="get-info">GET</h3>
  
    <p>No GET data</p>
  

  <h3 id="post-info">POST</h3>
  
    <p>No POST data</p>
  
  <h3 id="files-info">FILES</h3>
  
    <p>No FILES data</p>
  


  <h3 id="cookie-info">COOKIES</h3>
  
    <p>No cookie data</p>
  

  <h3 id="meta-info">META</h3>
  <table class="req">
    <thead>
      <tr>
        <th>Variable</th>
        <th>Value</th>
      </tr>
    </thead>
    <tbody>
      
        <tr>
          <td>HTTP_ACCEPT</td>
          <td class="code"><pre>&#x27;* /*&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>HTTP_ACCEPT_ENCODING</td>
          <td class="code"><pre>&#x27;gzip, deflate, br&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>HTTP_CACHE_CONTROL</td>
          <td class="code"><pre>&#x27;no-cache&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>HTTP_HOST</td>
          <td class="code"><pre>&#x27;payments.alpha.g-spot.website&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>HTTP_POSTMAN_TOKEN</td>
          <td class="code"><pre>&#x27;********************&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>HTTP_USER_AGENT</td>
          <td class="code"><pre>&#x27;PostmanRuntime/7.32.3&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>HTTP_X_FORWARDED_FOR</td>
          <td class="code"><pre>&#x27;178.88.105.153&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>HTTP_X_FORWARDED_HOST</td>
          <td class="code"><pre>&#x27;payments.alpha.g-spot.website&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>HTTP_X_FORWARDED_PORT</td>
          <td class="code"><pre>&#x27;443&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>HTTP_X_FORWARDED_PROTO</td>
          <td class="code"><pre>&#x27;https&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>HTTP_X_FORWARDED_SERVER</td>
          <td class="code"><pre>&#x27;757c3590a137&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>HTTP_X_REAL_IP</td>
          <td class="code"><pre>&#x27;178.88.105.153&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>PATH_INFO</td>
          <td class="code"><pre>&#x27;/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>QUERY_STRING</td>
          <td class="code"><pre>&#x27;&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>RAW_URI</td>
          <td class="code"><pre>&#x27;/api/v1/item_purchases/item-purchase-history/3fa85f64-5717-4562-b3fc-2c963f66afa6/&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>REMOTE_ADDR</td>
          <td class="code"><pre>&#x27;172.19.0.4&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>REMOTE_PORT</td>
          <td class="code"><pre>&#x27;45828&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>REQUEST_METHOD</td>
          <td class="code"><pre>&#x27;GET&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SCRIPT_NAME</td>
          <td class="code"><pre>&#x27;&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SERVER_NAME</td>
          <td class="code"><pre>&#x27;0.0.0.0&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SERVER_PORT</td>
          <td class="code"><pre>&#x27;8000&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SERVER_PROTOCOL</td>
          <td class="code"><pre>&#x27;HTTP/1.1&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SERVER_SOFTWARE</td>
          <td class="code"><pre>&#x27;gunicorn/20.1.0&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>gunicorn.socket</td>
          <td class="code"><pre>&lt;gevent._socket3.socket at 0x7fc311cf8700 object, fd=11, family=2, type=1, proto=6&gt;</pre></td>
        </tr>
      
        <tr>
          <td>rollbar.uuid</td>
          <td class="code"><pre>&#x27;c0c065bd-1b65-47bb-855b-e8320b135ef0&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>wsgi.errors</td>
          <td class="code"><pre>&lt;gunicorn.http.wsgi.WSGIErrorsWrapper object at 0x7fc311d06170&gt;</pre></td>
        </tr>
      
        <tr>
          <td>wsgi.file_wrapper</td>
          <td class="code"><pre>&lt;class &#x27;gunicorn.http.wsgi.FileWrapper&#x27;&gt;</pre></td>
        </tr>
      
        <tr>
          <td>wsgi.input</td>
          <td class="code"><pre>&lt;gunicorn.http.body.Body object at 0x7fc311b311d0&gt;</pre></td>
        </tr>
      
        <tr>
          <td>wsgi.input_terminated</td>
          <td class="code"><pre>True</pre></td>
        </tr>
      
        <tr>
          <td>wsgi.multiprocess</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>wsgi.multithread</td>
          <td class="code"><pre>True</pre></td>
        </tr>
      
        <tr>
          <td>wsgi.run_once</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>wsgi.url_scheme</td>
          <td class="code"><pre>&#x27;http&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>wsgi.version</td>
          <td class="code"><pre>(1, 0)</pre></td>
        </tr>
      
    </tbody>
  </table>


  <h3 id="settings-info">Settings</h3>
  <h4>Using settings module <code>config.settings</code></h4>
  <table class="req">
    <thead>
      <tr>
        <th>Setting</th>
        <th>Value</th>
      </tr>
    </thead>
    <tbody>
      
        <tr>
          <td>ABSOLUTE_URL_OVERRIDES</td>
          <td class="code"><pre>{}</pre></td>
        </tr>
      
        <tr>
          <td>ADMINS</td>
          <td class="code"><pre>[]</pre></td>
        </tr>
      
        <tr>
          <td>ALLOWED_HOSTS</td>
          <td class="code"><pre>[&#x27;*&#x27;]</pre></td>
        </tr>
      
        <tr>
          <td>APPEND_SLASH</td>
          <td class="code"><pre>True</pre></td>
        </tr>
      
        <tr>
          <td>AUTHENTICATION_BACKENDS</td>
          <td class="code"><pre>[&#x27;django.contrib.auth.backends.ModelBackend&#x27;]</pre></td>
        </tr>
      
        <tr>
          <td>AUTH_PASSWORD_VALIDATORS</td>
          <td class="code"><pre>&#x27;********************&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>AUTH_USER_MODEL</td>
          <td class="code"><pre>&#x27;auth.User&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>BASE_DIR</td>
          <td class="code"><pre>PosixPath(&#x27;/home/app/web&#x27;)</pre></td>
        </tr>
      
        <tr>
          <td>CACHES</td>
          <td class="code"><pre>{&#x27;default&#x27;: {&#x27;BACKEND&#x27;: &#x27;django.core.cache.backends.redis.RedisCache&#x27;,
             &#x27;LOCATION&#x27;: &#x27;redis://redis:6379/0&#x27;,
             &#x27;OPTIONS&#x27;: {&#x27;CLIENT_CLASS&#x27;: &#x27;django_redis.client.DefaultClient&#x27;}}}</pre></td>
        </tr>
      
        <tr>
          <td>CACHE_MIDDLEWARE_ALIAS</td>
          <td class="code"><pre>&#x27;default&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>CACHE_MIDDLEWARE_KEY_PREFIX</td>
          <td class="code"><pre>&#x27;********************&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>CACHE_MIDDLEWARE_SECONDS</td>
          <td class="code"><pre>600</pre></td>
        </tr>
      
        <tr>
          <td>CELERY_BROKER_URL</td>
          <td class="code"><pre>&#x27;redis://redis:6379/0&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>CSRF_COOKIE_AGE</td>
          <td class="code"><pre>31449600</pre></td>
        </tr>
      
        <tr>
          <td>CSRF_COOKIE_DOMAIN</td>
          <td class="code"><pre>None</pre></td>
        </tr>
      
        <tr>
          <td>CSRF_COOKIE_HTTPONLY</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>CSRF_COOKIE_MASKED</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>CSRF_COOKIE_NAME</td>
          <td class="code"><pre>&#x27;csrftoken&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>CSRF_COOKIE_PATH</td>
          <td class="code"><pre>&#x27;/&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>CSRF_COOKIE_SAMESITE</td>
          <td class="code"><pre>&#x27;Lax&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>CSRF_COOKIE_SECURE</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>CSRF_FAILURE_VIEW</td>
          <td class="code"><pre>&#x27;django.views.csrf.csrf_failure&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>CSRF_HEADER_NAME</td>
          <td class="code"><pre>&#x27;HTTP_X_CSRFTOKEN&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>CSRF_TRUSTED_ORIGINS</td>
          <td class="code"><pre>[]</pre></td>
        </tr>
      
        <tr>
          <td>CSRF_USE_SESSIONS</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>CURRENCIES</td>
          <td class="code"><pre>(&#x27;RUB&#x27;, &#x27;USD&#x27;, &#x27;EUR&#x27;)</pre></td>
        </tr>
      
        <tr>
          <td>DATABASES</td>
          <td class="code"><pre>{&#x27;default&#x27;: {&#x27;ATOMIC_REQUESTS&#x27;: False,
             &#x27;AUTOCOMMIT&#x27;: True,
             &#x27;CONN_HEALTH_CHECKS&#x27;: False,
             &#x27;CONN_MAX_AGE&#x27;: 0,
             &#x27;ENGINE&#x27;: &#x27;django.db.backends.postgresql&#x27;,
             &#x27;HOST&#x27;: &#x27;payments_db&#x27;,
             &#x27;NAME&#x27;: &#x27;payment&#x27;,
             &#x27;OPTIONS&#x27;: {},
             &#x27;PASSWORD&#x27;: &#x27;********************&#x27;,
             &#x27;PORT&#x27;: 5432,
             &#x27;TEST&#x27;: {&#x27;CHARSET&#x27;: None,
                      &#x27;COLLATION&#x27;: None,
                      &#x27;MIGRATE&#x27;: True,
                      &#x27;MIRROR&#x27;: None,
                      &#x27;NAME&#x27;: None},
             &#x27;TIME_ZONE&#x27;: None,
             &#x27;USER&#x27;: &#x27;postgres&#x27;}}</pre></td>
        </tr>
      
        <tr>
          <td>DATABASE_ROUTERS</td>
          <td class="code"><pre>[]</pre></td>
        </tr>
      
        <tr>
          <td>DATA_UPLOAD_MAX_MEMORY_SIZE</td>
          <td class="code"><pre>2621440</pre></td>
        </tr>
      
        <tr>
          <td>DATA_UPLOAD_MAX_NUMBER_FIELDS</td>
          <td class="code"><pre>1000</pre></td>
        </tr>
      
        <tr>
          <td>DATA_UPLOAD_MAX_NUMBER_FILES</td>
          <td class="code"><pre>100</pre></td>
        </tr>
      
        <tr>
          <td>DATETIME_FORMAT</td>
          <td class="code"><pre>&#x27;N j, Y, P&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>DATETIME_INPUT_FORMATS</td>
          <td class="code"><pre>[&#x27;%Y-%m-%d %H:%M:%S&#x27;,
 &#x27;%Y-%m-%d %H:%M:%S.%f&#x27;,
 &#x27;%Y-%m-%d %H:%M&#x27;,
 &#x27;%m/%d/%Y %H:%M:%S&#x27;,
 &#x27;%m/%d/%Y %H:%M:%S.%f&#x27;,
 &#x27;%m/%d/%Y %H:%M&#x27;,
 &#x27;%m/%d/%y %H:%M:%S&#x27;,
 &#x27;%m/%d/%y %H:%M:%S.%f&#x27;,
 &#x27;%m/%d/%y %H:%M&#x27;]</pre></td>
        </tr>
      
        <tr>
          <td>DATE_FORMAT</td>
          <td class="code"><pre>&#x27;N j, Y&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>DATE_INPUT_FORMATS</td>
          <td class="code"><pre>[&#x27;%Y-%m-%d&#x27;,
 &#x27;%m/%d/%Y&#x27;,
 &#x27;%m/%d/%y&#x27;,
 &#x27;%b %d %Y&#x27;,
 &#x27;%b %d, %Y&#x27;,
 &#x27;%d %b %Y&#x27;,
 &#x27;%d %b, %Y&#x27;,
 &#x27;%B %d %Y&#x27;,
 &#x27;%B %d, %Y&#x27;,
 &#x27;%d %B %Y&#x27;,
 &#x27;%d %B, %Y&#x27;]</pre></td>
        </tr>
      
        <tr>
          <td>DEBUG</td>
          <td class="code"><pre>True</pre></td>
        </tr>
      
        <tr>
          <td>DEBUG_PROPAGATE_EXCEPTIONS</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>DECIMAL_SEPARATOR</td>
          <td class="code"><pre>&#x27;.&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>DEFAULT_AUTO_FIELD</td>
          <td class="code"><pre>&#x27;django.db.models.BigAutoField&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>DEFAULT_CHARSET</td>
          <td class="code"><pre>&#x27;utf-8&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>DEFAULT_CURRENCY</td>
          <td class="code"><pre>&#x27;RUB&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>DEFAULT_EXCEPTION_REPORTER</td>
          <td class="code"><pre>&#x27;django.views.debug.ExceptionReporter&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>DEFAULT_EXCEPTION_REPORTER_FILTER</td>
          <td class="code"><pre>&#x27;django.views.debug.SafeExceptionReporterFilter&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>DEFAULT_FILE_STORAGE</td>
          <td class="code"><pre>&#x27;django.core.files.storage.FileSystemStorage&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>DEFAULT_FROM_EMAIL</td>
          <td class="code"><pre>&#x27;webmaster@localhost&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>DEFAULT_INDEX_TABLESPACE</td>
          <td class="code"><pre>&#x27;&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>DEFAULT_TABLESPACE</td>
          <td class="code"><pre>&#x27;&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>DISALLOWED_USER_AGENTS</td>
          <td class="code"><pre>[]</pre></td>
        </tr>
      
        <tr>
          <td>EMAIL_BACKEND</td>
          <td class="code"><pre>&#x27;django.core.mail.backends.smtp.EmailBackend&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>EMAIL_HOST</td>
          <td class="code"><pre>&#x27;localhost&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>EMAIL_HOST_PASSWORD</td>
          <td class="code"><pre>&#x27;********************&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>EMAIL_HOST_USER</td>
          <td class="code"><pre>&#x27;&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>EMAIL_PORT</td>
          <td class="code"><pre>25</pre></td>
        </tr>
      
        <tr>
          <td>EMAIL_SSL_CERTFILE</td>
          <td class="code"><pre>None</pre></td>
        </tr>
      
        <tr>
          <td>EMAIL_SSL_KEYFILE</td>
          <td class="code"><pre>&#x27;********************&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>EMAIL_SUBJECT_PREFIX</td>
          <td class="code"><pre>&#x27;[Django] &#x27;</pre></td>
        </tr>
      
        <tr>
          <td>EMAIL_TIMEOUT</td>
          <td class="code"><pre>None</pre></td>
        </tr>
      
        <tr>
          <td>EMAIL_USE_LOCALTIME</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>EMAIL_USE_SSL</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>EMAIL_USE_TLS</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>FILE_UPLOAD_DIRECTORY_PERMISSIONS</td>
          <td class="code"><pre>None</pre></td>
        </tr>
      
        <tr>
          <td>FILE_UPLOAD_HANDLERS</td>
          <td class="code"><pre>[&#x27;django.core.files.uploadhandler.MemoryFileUploadHandler&#x27;,
 &#x27;django.core.files.uploadhandler.TemporaryFileUploadHandler&#x27;]</pre></td>
        </tr>
      
        <tr>
          <td>FILE_UPLOAD_MAX_MEMORY_SIZE</td>
          <td class="code"><pre>2621440</pre></td>
        </tr>
      
        <tr>
          <td>FILE_UPLOAD_PERMISSIONS</td>
          <td class="code"><pre>420</pre></td>
        </tr>
      
        <tr>
          <td>FILE_UPLOAD_TEMP_DIR</td>
          <td class="code"><pre>None</pre></td>
        </tr>
      
        <tr>
          <td>FIRST_DAY_OF_WEEK</td>
          <td class="code"><pre>0</pre></td>
        </tr>
      
        <tr>
          <td>FIXTURE_DIRS</td>
          <td class="code"><pre>[]</pre></td>
        </tr>
      
        <tr>
          <td>FORCE_SCRIPT_NAME</td>
          <td class="code"><pre>None</pre></td>
        </tr>
      
        <tr>
          <td>FORMAT_MODULE_PATH</td>
          <td class="code"><pre>None</pre></td>
        </tr>
      
        <tr>
          <td>FORM_RENDERER</td>
          <td class="code"><pre>&#x27;django.forms.renderers.DjangoTemplates&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>GAMES_SERVICE</td>
          <td class="code"><pre>GamesService(GAMES_DOMAIN=&#x27;https://alpha.g-spot.website/api/v*/games&#x27;, GAMES_REFUND=&#x27;/refund_url&#x27;)</pre></td>
        </tr>
      
        <tr>
          <td>IGNORABLE_404_URLS</td>
          <td class="code"><pre>[]</pre></td>
        </tr>
      
        <tr>
          <td>INSTALLED_APPS</td>
          <td class="code"><pre>[&#x27;django.contrib.admin&#x27;,
 &#x27;django.contrib.auth&#x27;,
 &#x27;django.contrib.contenttypes&#x27;,
 &#x27;django.contrib.sessions&#x27;,
 &#x27;django.contrib.messages&#x27;,
 &#x27;django.contrib.staticfiles&#x27;,
 &#x27;djmoney&#x27;,
 &#x27;django_extensions&#x27;,
 &#x27;drf_spectacular&#x27;,
 &#x27;rest_framework&#x27;,
 &#x27;apps.payment_accounts&#x27;,
 &#x27;apps.item_purchases&#x27;,
 &#x27;apps.external_payments&#x27;
    ]</pre></td>
        </tr>
      
        <tr>
          <td>INTERNAL_IPS</td>
          <td class="code"><pre>[]</pre></td>
        </tr>
      
        <tr>
          <td>INVOICE_ATTEMPTS_PER_PERIOD</td>
          <td class="code"><pre>5</pre></td>
        </tr>
      
        <tr>
          <td>JWT_SECRET_KEY</td>
          <td class="code"><pre>&#x27;********************&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>LANGUAGES</td>
          <td class="code"><pre>[(&#x27;af&#x27;, &#x27;Afrikaans&#x27;),
 (&#x27;ar&#x27;, &#x27;Arabic&#x27;),
 (&#x27;ar-dz&#x27;, &#x27;Algerian Arabic&#x27;),
 (&#x27;ast&#x27;, &#x27;Asturian&#x27;),
 (&#x27;az&#x27;, &#x27;Azerbaijani&#x27;),
 (&#x27;bg&#x27;, &#x27;Bulgarian&#x27;),
 (&#x27;be&#x27;, &#x27;Belarusian&#x27;),
 (&#x27;bn&#x27;, &#x27;Bengali&#x27;),
 (&#x27;br&#x27;, &#x27;Breton&#x27;),
 (&#x27;bs&#x27;, &#x27;Bosnian&#x27;),
 (&#x27;ca&#x27;, &#x27;Catalan&#x27;),
 (&#x27;cs&#x27;, &#x27;Czech&#x27;),
 (&#x27;cy&#x27;, &#x27;Welsh&#x27;),
 (&#x27;da&#x27;, &#x27;Danish&#x27;),
 (&#x27;de&#x27;, &#x27;German&#x27;),
 (&#x27;dsb&#x27;, &#x27;Lower Sorbian&#x27;),
 (&#x27;el&#x27;, &#x27;Greek&#x27;),
 (&#x27;en&#x27;, &#x27;English&#x27;),
 (&#x27;en-au&#x27;, &#x27;Australian English&#x27;),
 (&#x27;en-gb&#x27;, &#x27;British English&#x27;),
 (&#x27;eo&#x27;, &#x27;Esperanto&#x27;),
 (&#x27;es&#x27;, &#x27;Spanish&#x27;),
 (&#x27;es-ar&#x27;, &#x27;Argentinian Spanish&#x27;),
 (&#x27;es-co&#x27;, &#x27;Colombian Spanish&#x27;),
 (&#x27;es-mx&#x27;, &#x27;Mexican Spanish&#x27;),
 (&#x27;es-ni&#x27;, &#x27;Nicaraguan Spanish&#x27;),
 (&#x27;es-ve&#x27;, &#x27;Venezuelan Spanish&#x27;),
 (&#x27;et&#x27;, &#x27;Estonian&#x27;),
 (&#x27;eu&#x27;, &#x27;Basque&#x27;),
 (&#x27;fa&#x27;, &#x27;Persian&#x27;),
 (&#x27;fi&#x27;, &#x27;Finnish&#x27;),
 (&#x27;fr&#x27;, &#x27;French&#x27;),
 (&#x27;fy&#x27;, &#x27;Frisian&#x27;),
 (&#x27;ga&#x27;, &#x27;Irish&#x27;),
 (&#x27;gd&#x27;, &#x27;Scottish Gaelic&#x27;),
 (&#x27;gl&#x27;, &#x27;Galician&#x27;),
 (&#x27;he&#x27;, &#x27;Hebrew&#x27;),
 (&#x27;hi&#x27;, &#x27;Hindi&#x27;),
 (&#x27;hr&#x27;, &#x27;Croatian&#x27;),
 (&#x27;hsb&#x27;, &#x27;Upper Sorbian&#x27;),
 (&#x27;hu&#x27;, &#x27;Hungarian&#x27;),
 (&#x27;hy&#x27;, &#x27;Armenian&#x27;),
 (&#x27;ia&#x27;, &#x27;Interlingua&#x27;),
 (&#x27;id&#x27;, &#x27;Indonesian&#x27;),
 (&#x27;ig&#x27;, &#x27;Igbo&#x27;),
 (&#x27;io&#x27;, &#x27;Ido&#x27;),
 (&#x27;is&#x27;, &#x27;Icelandic&#x27;),
 (&#x27;it&#x27;, &#x27;Italian&#x27;),
 (&#x27;ja&#x27;, &#x27;Japanese&#x27;),
 (&#x27;ka&#x27;, &#x27;Georgian&#x27;),
 (&#x27;kab&#x27;, &#x27;Kabyle&#x27;),
 (&#x27;kk&#x27;, &#x27;Kazakh&#x27;),
 (&#x27;km&#x27;, &#x27;Khmer&#x27;),
 (&#x27;kn&#x27;, &#x27;Kannada&#x27;),
 (&#x27;ko&#x27;, &#x27;Korean&#x27;),
 (&#x27;ky&#x27;, &#x27;Kyrgyz&#x27;),
 (&#x27;lb&#x27;, &#x27;Luxembourgish&#x27;),
 (&#x27;lt&#x27;, &#x27;Lithuanian&#x27;),
 (&#x27;lv&#x27;, &#x27;Latvian&#x27;),
 (&#x27;mk&#x27;, &#x27;Macedonian&#x27;),
 (&#x27;ml&#x27;, &#x27;Malayalam&#x27;),
 (&#x27;mn&#x27;, &#x27;Mongolian&#x27;),
 (&#x27;mr&#x27;, &#x27;Marathi&#x27;),
 (&#x27;ms&#x27;, &#x27;Malay&#x27;),
 (&#x27;my&#x27;, &#x27;Burmese&#x27;),
 (&#x27;nb&#x27;, &#x27;Norwegian Bokmål&#x27;),
 (&#x27;ne&#x27;, &#x27;Nepali&#x27;),
 (&#x27;nl&#x27;, &#x27;Dutch&#x27;),
 (&#x27;nn&#x27;, &#x27;Norwegian Nynorsk&#x27;),
 (&#x27;os&#x27;, &#x27;Ossetic&#x27;),
 (&#x27;pa&#x27;, &#x27;Punjabi&#x27;),
 (&#x27;pl&#x27;, &#x27;Polish&#x27;),
 (&#x27;pt&#x27;, &#x27;Portuguese&#x27;),
 (&#x27;pt-br&#x27;, &#x27;Brazilian Portuguese&#x27;),
 (&#x27;ro&#x27;, &#x27;Romanian&#x27;),
 (&#x27;ru&#x27;, &#x27;Russian&#x27;),
 (&#x27;sk&#x27;, &#x27;Slovak&#x27;),
 (&#x27;sl&#x27;, &#x27;Slovenian&#x27;),
 (&#x27;sq&#x27;, &#x27;Albanian&#x27;),
 (&#x27;sr&#x27;, &#x27;Serbian&#x27;),
 (&#x27;sr-latn&#x27;, &#x27;Serbian Latin&#x27;),
 (&#x27;sv&#x27;, &#x27;Swedish&#x27;),
 (&#x27;sw&#x27;, &#x27;Swahili&#x27;),
 (&#x27;ta&#x27;, &#x27;Tamil&#x27;),
 (&#x27;te&#x27;, &#x27;Telugu&#x27;),
 (&#x27;tg&#x27;, &#x27;Tajik&#x27;),
 (&#x27;th&#x27;, &#x27;Thai&#x27;),
 (&#x27;tk&#x27;, &#x27;Turkmen&#x27;),
 (&#x27;tr&#x27;, &#x27;Turkish&#x27;),
 (&#x27;tt&#x27;, &#x27;Tatar&#x27;),
 (&#x27;udm&#x27;, &#x27;Udmurt&#x27;),
 (&#x27;uk&#x27;, &#x27;Ukrainian&#x27;),
 (&#x27;ur&#x27;, &#x27;Urdu&#x27;),
 (&#x27;uz&#x27;, &#x27;Uzbek&#x27;),
 (&#x27;vi&#x27;, &#x27;Vietnamese&#x27;),
 (&#x27;zh-hans&#x27;, &#x27;Simplified Chinese&#x27;),
 (&#x27;zh-hant&#x27;, &#x27;Traditional Chinese&#x27;)
    ]</pre></td>
        </tr>
      
        <tr>
          <td>LANGUAGES_BIDI</td>
          <td class="code"><pre>[&#x27;he&#x27;, &#x27;ar&#x27;, &#x27;ar-dz&#x27;, &#x27;fa&#x27;, &#x27;ur&#x27;
    ]</pre></td>
        </tr>
      
        <tr>
          <td>LANGUAGE_CODE</td>
          <td class="code"><pre>&#x27;en-us&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>LANGUAGE_COOKIE_AGE</td>
          <td class="code"><pre>None</pre></td>
        </tr>
      
        <tr>
          <td>LANGUAGE_COOKIE_DOMAIN</td>
          <td class="code"><pre>None</pre></td>
        </tr>
      
        <tr>
          <td>LANGUAGE_COOKIE_HTTPONLY</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>LANGUAGE_COOKIE_NAME</td>
          <td class="code"><pre>&#x27;django_language&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>LANGUAGE_COOKIE_PATH</td>
          <td class="code"><pre>&#x27;/&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>LANGUAGE_COOKIE_SAMESITE</td>
          <td class="code"><pre>None</pre></td>
        </tr>
      
        <tr>
          <td>LANGUAGE_COOKIE_SECURE</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>LOCALE_PATHS</td>
          <td class="code"><pre>[]</pre></td>
        </tr>
      
        <tr>
          <td>LOGGING</td>
          <td class="code"><pre>{}</pre></td>
        </tr>
      
        <tr>
          <td>LOGGING_CONFIG</td>
          <td class="code"><pre>&#x27;logging.config.dictConfig&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>LOGIN_REDIRECT_URL</td>
          <td class="code"><pre>&#x27;/accounts/profile/&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>LOGIN_URL</td>
          <td class="code"><pre>&#x27;/accounts/login/&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>LOGOUT_REDIRECT_URL</td>
          <td class="code"><pre>None</pre></td>
        </tr>
      
        <tr>
          <td>MANAGERS</td>
          <td class="code"><pre>[]</pre></td>
        </tr>
      
        <tr>
          <td>MAXIMUM_PAYOUTS_PER_MONTH</td>
          <td class="code"><pre>1</pre></td>
        </tr>
      
        <tr>
          <td>MAXIMUM_YOOKASSA_PAYOUT</td>
          <td class="code"><pre>Decimal(&#x27;500000&#x27;)</pre></td>
        </tr>
      
        <tr>
          <td>MAX_BALANCE_DIGITS</td>
          <td class="code"><pre>11</pre></td>
        </tr>
      
        <tr>
          <td>MAX_COMMISSION_VALUE</td>
          <td class="code"><pre>Decimal(&#x27;100&#x27;)</pre></td>
        </tr>
      
        <tr>
          <td>MEDIA_ROOT</td>
          <td class="code"><pre>&#x27;&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>MEDIA_URL</td>
          <td class="code"><pre>&#x27;/&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>MESSAGE_STORAGE</td>
          <td class="code"><pre>&#x27;django.contrib.messages.storage.fallback.FallbackStorage&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>MIDDLEWARE</td>
          <td class="code"><pre>[&#x27;django.middleware.security.SecurityMiddleware&#x27;,
 &#x27;django.contrib.sessions.middleware.SessionMiddleware&#x27;,
 &#x27;django.middleware.common.CommonMiddleware&#x27;,
 &#x27;django.middleware.csrf.CsrfViewMiddleware&#x27;,
 &#x27;django.contrib.auth.middleware.AuthenticationMiddleware&#x27;,
 &#x27;django.contrib.messages.middleware.MessageMiddleware&#x27;,
 &#x27;django.middleware.clickjacking.XFrameOptionsMiddleware&#x27;,
 &#x27;rollbar.contrib.django.middleware.RollbarNotifierMiddleware&#x27;
    ]</pre></td>
        </tr>
      
        <tr>
          <td>MIGRATION_MODULES</td>
          <td class="code"><pre>{}</pre></td>
        </tr>
      
        <tr>
          <td>MINIMUM_PAYOUT_AMOUNT</td>
          <td class="code"><pre>Decimal(&#x27;500&#x27;)</pre></td>
        </tr>
      
        <tr>
          <td>MINUTES_FOR_INVOICE_ATTEMPTS</td>
          <td class="code"><pre>60</pre></td>
        </tr>
      
        <tr>
          <td>MONTH_DAY_FORMAT</td>
          <td class="code"><pre>&#x27;F j&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>NUMBER_GROUPING</td>
          <td class="code"><pre>0</pre></td>
        </tr>
      
        <tr>
          <td>PASSWORD_HASHERS</td>
          <td class="code"><pre>&#x27;********************&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>PASSWORD_RESET_TIMEOUT</td>
          <td class="code"><pre>&#x27;********************&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>PERIOD_FOR_GIFT_TASK</td>
          <td class="code"><pre>datetime.timedelta(days=7)</pre></td>
        </tr>
      
        <tr>
          <td>PERIOD_FOR_MYSELF_TASK</td>
          <td class="code"><pre>datetime.timedelta(days=1)</pre></td>
        </tr>
      
        <tr>
          <td>PREPEND_WWW</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>REST_FRAMEWORK</td>
          <td class="code"><pre>{&#x27;DEFAULT_PAGINATION_CLASS&#x27;: &#x27;rest_framework.pagination.PageNumberPagination&#x27;,
 &#x27;DEFAULT_PERMISSION_CLASSES&#x27;: [&#x27;rest_framework.permissions.AllowAny&#x27;
        ],
 &#x27;DEFAULT_SCHEMA_CLASS&#x27;: &#x27;drf_spectacular.openapi.AutoSchema&#x27;,
 &#x27;EXCEPTION_HANDLER&#x27;: &#x27;rollbar.contrib.django_rest_framework.post_exception_handler&#x27;,
 &#x27;PAGE_SIZE&#x27;: 100
    }</pre></td>
        </tr>
      
        <tr>
          <td>ROLLBAR</td>
          <td class="code"><pre>{&#x27;access_token&#x27;: &#x27;********************&#x27;,
 &#x27;code_version&#x27;: &#x27;1.0&#x27;,
 &#x27;environment&#x27;: &#x27;development&#x27;,
 &#x27;root&#x27;: PosixPath(&#x27;/home/app/web&#x27;)
    }</pre></td>
        </tr>
      
        <tr>
          <td>ROOT_URLCONF</td>
          <td class="code"><pre>&#x27;config.urls&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SECRET_KEY</td>
          <td class="code"><pre>&#x27;********************&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SECRET_KEY_FALLBACKS</td>
          <td class="code"><pre>&#x27;********************&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SECURE_CONTENT_TYPE_NOSNIFF</td>
          <td class="code"><pre>True</pre></td>
        </tr>
      
        <tr>
          <td>SECURE_CROSS_ORIGIN_OPENER_POLICY</td>
          <td class="code"><pre>&#x27;same-origin&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SECURE_HSTS_INCLUDE_SUBDOMAINS</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>SECURE_HSTS_PRELOAD</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>SECURE_HSTS_SECONDS</td>
          <td class="code"><pre>0</pre></td>
        </tr>
      
        <tr>
          <td>SECURE_PROXY_SSL_HEADER</td>
          <td class="code"><pre>None</pre></td>
        </tr>
      
        <tr>
          <td>SECURE_REDIRECT_EXEMPT</td>
          <td class="code"><pre>[]</pre></td>
        </tr>
      
        <tr>
          <td>SECURE_REFERRER_POLICY</td>
          <td class="code"><pre>&#x27;same-origin&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SECURE_SSL_HOST</td>
          <td class="code"><pre>None</pre></td>
        </tr>
      
        <tr>
          <td>SECURE_SSL_REDIRECT</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>SERVER_EMAIL</td>
          <td class="code"><pre>&#x27;root@localhost&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SESSION_CACHE_ALIAS</td>
          <td class="code"><pre>&#x27;default&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SESSION_COOKIE_AGE</td>
          <td class="code"><pre>1209600</pre></td>
        </tr>
      
        <tr>
          <td>SESSION_COOKIE_DOMAIN</td>
          <td class="code"><pre>None</pre></td>
        </tr>
      
        <tr>
          <td>SESSION_COOKIE_HTTPONLY</td>
          <td class="code"><pre>True</pre></td>
        </tr>
      
        <tr>
          <td>SESSION_COOKIE_NAME</td>
          <td class="code"><pre>&#x27;sessionid&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SESSION_COOKIE_PATH</td>
          <td class="code"><pre>&#x27;/&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SESSION_COOKIE_SAMESITE</td>
          <td class="code"><pre>&#x27;Lax&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SESSION_COOKIE_SECURE</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>SESSION_ENGINE</td>
          <td class="code"><pre>&#x27;django.contrib.sessions.backends.db&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SESSION_EXPIRE_AT_BROWSER_CLOSE</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>SESSION_FILE_PATH</td>
          <td class="code"><pre>None</pre></td>
        </tr>
      
        <tr>
          <td>SESSION_SAVE_EVERY_REQUEST</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>SESSION_SERIALIZER</td>
          <td class="code"><pre>&#x27;django.contrib.sessions.serializers.JSONSerializer&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SETTINGS_MODULE</td>
          <td class="code"><pre>&#x27;config.settings&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SHORT_DATETIME_FORMAT</td>
          <td class="code"><pre>&#x27;m/d/Y P&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SHORT_DATE_FORMAT</td>
          <td class="code"><pre>&#x27;m/d/Y&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SIGNING_BACKEND</td>
          <td class="code"><pre>&#x27;django.core.signing.TimestampSigner&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SILENCED_SYSTEM_CHECKS</td>
          <td class="code"><pre>[]</pre></td>
        </tr>
      
        <tr>
          <td>SPECTACULAR_SETTINGS</td>
          <td class="code"><pre>{&#x27;DESCRIPTION&#x27;: &#x27;API for game store payments service&#x27;,
 &#x27;TITLE&#x27;: &#x27;GSpot Payments API&#x27;,
 &#x27;VERSION&#x27;: &#x27;1.0.0&#x27;
    }</pre></td>
        </tr>
      
        <tr>
          <td>STATICFILES_DIRS</td>
          <td class="code"><pre>[]</pre></td>
        </tr>
      
        <tr>
          <td>STATICFILES_FINDERS</td>
          <td class="code"><pre>[&#x27;django.contrib.staticfiles.finders.FileSystemFinder&#x27;,
 &#x27;django.contrib.staticfiles.finders.AppDirectoriesFinder&#x27;
    ]</pre></td>
        </tr>
      
        <tr>
          <td>STATICFILES_STORAGE</td>
          <td class="code"><pre>&#x27;django.contrib.staticfiles.storage.StaticFilesStorage&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>STATIC_ROOT</td>
          <td class="code"><pre>&#x27;/home/app/web/static&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>STATIC_URL</td>
          <td class="code"><pre>&#x27;/static/&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>SUPPORTED_CURRENCIES</td>
          <td class="code"><pre>(&#x27;RUB&#x27;,)</pre></td>
        </tr>
      
        <tr>
          <td>TEMPLATES</td>
          <td class="code"><pre>[
        {&#x27;APP_DIRS&#x27;: True,
  &#x27;BACKEND&#x27;: &#x27;django.template.backends.django.DjangoTemplates&#x27;,
  &#x27;DIRS&#x27;: [],
  &#x27;OPTIONS&#x27;: {&#x27;context_processors&#x27;: [&#x27;django.template.context_processors.debug&#x27;,
                                     &#x27;django.template.context_processors.request&#x27;,
                                     &#x27;django.contrib.auth.context_processors.auth&#x27;,
                                     &#x27;django.contrib.messages.context_processors.messages&#x27;
                ]
            }
        }
    ]</pre></td>
        </tr>
      
        <tr>
          <td>TEST_NON_SERIALIZED_APPS</td>
          <td class="code"><pre>[]</pre></td>
        </tr>
      
        <tr>
          <td>TEST_RUNNER</td>
          <td class="code"><pre>&#x27;django.test.runner.DiscoverRunner&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>THOUSAND_SEPARATOR</td>
          <td class="code"><pre>&#x27;,&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>TIME_FORMAT</td>
          <td class="code"><pre>&#x27;P&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>TIME_INPUT_FORMATS</td>
          <td class="code"><pre>[&#x27;%H:%M:%S&#x27;, &#x27;%H:%M:%S.%f&#x27;, &#x27;%H:%M&#x27;
    ]</pre></td>
        </tr>
      
        <tr>
          <td>TIME_ZONE</td>
          <td class="code"><pre>&#x27;UTC&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>USE_DEPRECATED_PYTZ</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>USE_I18N</td>
          <td class="code"><pre>True</pre></td>
        </tr>
      
        <tr>
          <td>USE_L10N</td>
          <td class="code"><pre>True</pre></td>
        </tr>
      
        <tr>
          <td>USE_THOUSAND_SEPARATOR</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>USE_TZ</td>
          <td class="code"><pre>True</pre></td>
        </tr>
      
        <tr>
          <td>USE_X_FORWARDED_HOST</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>USE_X_FORWARDED_PORT</td>
          <td class="code"><pre>False</pre></td>
        </tr>
      
        <tr>
          <td>WSGI_APPLICATION</td>
          <td class="code"><pre>&#x27;config.wsgi.application&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>X_FRAME_OPTIONS</td>
          <td class="code"><pre>&#x27;DENY&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>YEAR_MONTH_FORMAT</td>
          <td class="code"><pre>&#x27;F Y&#x27;</pre></td>
        </tr>
      
        <tr>
          <td>YOOKASSA_CONFIG</td>
          <td class="code"><pre>YookassaConfig(SHOP_ACCOUNT_ID=111111, SHOP_SECRET_KEY=&#x27;test_1111111111&#x27;, GATE_AWAY_ACCOUNT_ID=123456, GATE_AWAY_SECRET_KEY=&#x27;your_gate_away_secret_key&#x27;)</pre></td>
        </tr>
      
    </tbody>
  </table>

</div>

  <div id="explanation">
    <p>
      You’re seeing this error because you have <code>DEBUG = True</code> in your
      Django settings file. Change that to <code>False</code>, and Django will
      display a standard page generated by the handler for this status code.
    </p>
  </div>

</body>
</html>

-->


Постусловие: удалить тестовые данные

Автор: Евгений

Тест выполнен
| Дата | Время | Результат | Имя | Баг № Trello |
| --- | --- | --- | --- | --- |
| 2023-07-21 | 12:45 | Passed | Евгений | - | 