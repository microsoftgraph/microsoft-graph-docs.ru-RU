
# <a name="create-absolute-positioned-elements-in-onenote-pages"></a><span data-ttu-id="610b6-101">Создание элементов с абсолютным положением на страницах OneNote</span><span class="sxs-lookup"><span data-stu-id="610b6-101">Create absolute positioned elements in OneNote pages</span></span>

<span data-ttu-id="610b6-102">В тексте страницы OneNote может содержаться много прямых (`div`, `img`) и дочерних (`object`) элементов, которые можно разместить независимо друг от друга на странице.</span><span class="sxs-lookup"><span data-stu-id="610b6-102">The body of a onnvshort page can contain multiple direct child elements of type div, img, or object. These child elements can be positioned independently anywhere on the page.</span></span>

<a name="attributes"></a>
## <a name="attributes-and-positioning-behavior"></a><span data-ttu-id="610b6-103">Атрибуты и поведение при расположении</span><span class="sxs-lookup"><span data-stu-id="610b6-103">Attributes and positioning behavior</span></span>

<span data-ttu-id="610b6-104">Чтобы создать элементы с абсолютным положением на странице, используйте атрибуты `data-absolute-enabled` и [`style`](#supported-css-style-attributes), как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="610b6-104">Use the `data-absolute-enabled` and [`style`](#supported-css-style-attributes) attributes to create absolute positioned elements on a page, as follows:</span></span>

- <span data-ttu-id="610b6-105">Элемент body должен указывать `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="610b6-105">The body element must specify `data-absolute-enabled="true"`.</span></span> <span data-ttu-id="610b6-106">Если он опущен или имеет значение `false`, весь контент в элементе body отображается в элементе `_default` с абсолютным положением, созданным API, и все параметры положения будут проигнорированы.</span><span class="sxs-lookup"><span data-stu-id="610b6-106">The body`false` element must specify data-absolute-enabled="true"`_default`. If omitted or set to false, all body content is rendered inside  a _default absolutely positioned div that the API creates, and all position settings are ignored.</span></span>

- <span data-ttu-id="610b6-107">Только элементы `div`, `img` и `object` могут иметь абсолютное положение.</span><span class="sxs-lookup"><span data-stu-id="610b6-107">Only `div`, `img`, and `object` elements can be absolute positioned elements.</span></span> 

- <span data-ttu-id="610b6-108">Для элементов с абсолютным положением должен быть задан параметр `style="position:absolute"`.</span><span class="sxs-lookup"><span data-stu-id="610b6-108">Absolute positioned elements must specify `style="position:absolute"`.</span></span>

- <span data-ttu-id="610b6-109">Элементы с абсолютным положением должны быть прямыми дочерними элементами элемента `body`.</span><span class="sxs-lookup"><span data-stu-id="610b6-109">Absolute positioned elements must be direct children of the `body` element.</span></span> <span data-ttu-id="610b6-110">Любой прямой дочерний элемент элемента body, не являющийся элементом `div`, `img` или `object` с абсолютным положением, отображается в виде статичного контента внутри элемента div `_default` с абсолютным положением.</span><span class="sxs-lookup"><span data-stu-id="610b6-110">Any direct children of the body that aren't absolute positioned `div`, `img`, or `object` elements are rendered as static content inside the absolute positioned `_default` div.</span></span>

- <span data-ttu-id="610b6-111">Элементы с абсолютным положением размещаются согласно указанным для них координатам левого верхнего угла относительно начального положения 0:0, соответствующего левому верхнему углу страницы над областью заголовка.</span><span class="sxs-lookup"><span data-stu-id="610b6-111">Absolutely positioned elements are positioned at their specified top and left coordinates, relative to the 0:0 starting position at the absolute top, left corner of the page (above the title area).</span></span>

- <span data-ttu-id="610b6-112">Если у элемента с абсолютным положением опущена верхняя или левая координата, для этой координаты применяется соответствующее значение, используемое по умолчанию: `top:120px` или `left:48px`.</span><span class="sxs-lookup"><span data-stu-id="610b6-112">If an absolute positioned element omits the top or left coordinate, the missing coordinate is set to its default value: `top:120px` or `left:48px`.</span></span> <span data-ttu-id="610b6-113">Эти координаты, используемые по умолчанию, указывают положение непосредственно под областью заголовка.</span><span class="sxs-lookup"><span data-stu-id="610b6-113">These default coordinates specify a position just below the title area.</span></span> <span data-ttu-id="610b6-114">Помните, что если не указывать координаты элементов, последние будут накладываться друг на друга.</span><span class="sxs-lookup"><span data-stu-id="610b6-114">Be aware that omitting coordinates can result in elements that are stacked on top of each other.</span></span>

- <span data-ttu-id="610b6-115">Элементы с абсолютным положением не должны быть вложенными и не должны содержать элементы с заданными положениями.</span><span class="sxs-lookup"><span data-stu-id="610b6-115">Absolute positioned elements cannot be nested or contain positioned elements.</span></span> <span data-ttu-id="610b6-116">API игнорирует все параметры положения, указанные во вложенных элементах внутри элемента div с абсолютным положением, отображает вложенный контент внутри родительского элемента div с абсолютным положением и возвращает предупреждение через свойство **api.diagnostics** в ответе.</span><span class="sxs-lookup"><span data-stu-id="610b6-116">Absolutely positioned elements cannot be nested or contain positioned elements. The API ignores any position settings specified on nested elements inside an absolutely positioned div, renders the nested content inside the absolutely positioned parent div, and returns a warning in the **api.diagnostics** property in the  response.</span></span>


# <a name="example"></a><span data-ttu-id="610b6-117">Пример</span><span class="sxs-lookup"><span data-stu-id="610b6-117">Example</span></span>

 <span data-ttu-id="610b6-118">В примере ниже показан прямой дочерний элемент `p`, элемент div с абсолютным положением и элемент div с неабсолютным положением.</span><span class="sxs-lookup"><span data-stu-id="610b6-118">The following example contains a direct `p` child, an absolute positioned div, and a non-absolute positioned div.</span></span>

## <a name="input-html"></a><span data-ttu-id="610b6-119">Входной HTML-код</span><span class="sxs-lookup"><span data-stu-id="610b6-119">Input HTML</span></span>  

   ```html 
   <body data-absolute-enabled="true">
       <p>This content will appear in the _default div.</p>
       <div style="position:absolute;top:175px;left:100px" data-id="div1">
         <p>This content will appear in an absolute positioned div.</p>
       </div>
       <div>
           <p>This content will also appear in the _default div.</p>
       </div>
   </body>
   ```

<span data-ttu-id="610b6-120">API отрисовывает элемент div с неабсолютным положением в элементе div, используемом по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="610b6-120">The API renders the non-absolute positioned div in the default div.</span></span> <span data-ttu-id="610b6-121">Обратите внимание на то, что система игнорирует вложенные теги `<div>`, так как в них не определено никакой семантической информации (например, `data-id`).</span><span class="sxs-lookup"><span data-stu-id="610b6-121">Note that the nested  `<div>` tags are discarded because they do not define any semantic information (such as `data-id`).</span></span>

## <a name="output-html"></a><span data-ttu-id="610b6-122">Выходной HTML-код</span><span class="sxs-lookup"><span data-stu-id="610b6-122">Output HTML</span></span> 

   ```html 
   <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11pt">
       <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
           <p>This content will appear in the _default div.</p>
           <p>This content will also appear in the _default div.</p>
       </div>
       <div data-id="div1" style="position:absolute;left:99px;top:174px;width:624px">
           <p>This content will appear in an absolute positioned div.</p>
       </div>
   </body>
   ```

## <a name="example"></a><span data-ttu-id="610b6-123">Пример</span><span class="sxs-lookup"><span data-stu-id="610b6-123">Example</span></span>

 <span data-ttu-id="610b6-124">В примере ниже показано, как создать страницу, которая содержит один элемент div с абсолютным положением и одно изображение с абсолютным положением.</span><span class="sxs-lookup"><span data-stu-id="610b6-124">The following example creates a page that contains one absolutely positioned div and one absolutely positioned   image.</span></span>


### <a name="input-html"></a><span data-ttu-id="610b6-125">Входной HTML-код</span><span class="sxs-lookup"><span data-stu-id="610b6-125">Input HTML</span></span>  

```html 
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body data-absolute-enabled="true">
        <div style="position:absolute;width:280px;top:120px;left:68px">
            <p>Some text</p>
            <img style="width:120px" src="http://officeimg.vo.msecnd.net/en-us/files/018/949/ZA103278226.png" />
            <div>
                <p>More text inside a regular, nested div</p>
            </div>
        </div>
        <img style="position:absolute;width:360px;top:350px;left:300px" src="http://officeimg.vo.msecnd.net/en-us/files/018/949/ZA103278226.png" />
    </body>
</html>
```
 
<span data-ttu-id="610b6-126">API OneNote оценивает входной HTML-код и сохраняет весь семантический контент и информацию о структуре, которые поддерживает OneNote.</span><span class="sxs-lookup"><span data-stu-id="610b6-126">The OneNote API evaluates the input HTML and preserves all semantic content and any structural information that is supported by OneNote.</span></span> <span data-ttu-id="610b6-127">Полученная в результате страница отображается, как показано на рисунке ниже (но без видимых границ для элемента div и изображения).</span><span class="sxs-lookup"><span data-stu-id="610b6-127">The resulting page renders as shown in the following image (but without the visible borders for the div and image).</span></span> 

![Полученная в результате страница с элементом div и изображением с абсолютными положениями](images/abs-pos.PNG)

<span data-ttu-id="610b6-129">Обратите внимание на изменение незначимого вложенного элемента div по сравнению со входным HTML-кодом.</span><span class="sxs-lookup"><span data-stu-id="610b6-129">Notice the changes to the non-contributing, nested div from the input HTML.</span></span> <span data-ttu-id="610b6-130">API сохраняет контент, содержащийся в элементе div, но игнорирует теги `<div>`, так как в элементе div не определена семантическая информация (например, `data-id`).</span><span class="sxs-lookup"><span data-stu-id="610b6-130">The API preserves the div's content but discards the `<div>` tags because the div doesn't define semantic information (such as `data-id`).</span></span>

<span data-ttu-id="610b6-131">Дополнительные сведения о том, как API OneNote обрабатывает входной и выходной HTML-код, см. в статье [Входной и выходной HTML-код на страницах OneNote](onenote_input_output_html.md).</span><span class="sxs-lookup"><span data-stu-id="610b6-131">For more information about how the onnvshort API handles input and output HTML, see Input and output HTML for OneNote pages.</span></span>

<a name="style-attributes"></a>
### <a name="supported-css-style-attributes"></a><span data-ttu-id="610b6-132">Поддерживаемые атрибуты стиля CSS</span><span class="sxs-lookup"><span data-stu-id="610b6-132">Supported CSS style attributes</span></span>

<span data-ttu-id="610b6-133">Для всех элементов с абсолютными положениями можно указать положения левого верхнего угла.</span><span class="sxs-lookup"><span data-stu-id="610b6-133">All absolute positioned elements can specify top and left positions.</span></span> <span data-ttu-id="610b6-134">Для элемента div и изображения можно указать ширину. Кроме того, для изображений можно указать высоту.</span><span class="sxs-lookup"><span data-stu-id="610b6-134">All absolutely positioned elements can  specify top and left positions. Divs and images can specify width, and images can also specify height. For example:</span></span> <span data-ttu-id="610b6-135">Пример:</span><span class="sxs-lookup"><span data-stu-id="610b6-135">For example:</span></span>

```html
<img style="position:absolute;top:140px;left:95px;width:480px;height:665px" src="..." />
```

| <span data-ttu-id="610b6-136">Атрибут</span><span class="sxs-lookup"><span data-stu-id="610b6-136">Attribute</span></span> | <span data-ttu-id="610b6-137">Поддерживаемый элемент</span><span class="sxs-lookup"><span data-stu-id="610b6-137">Supported element</span></span> | <span data-ttu-id="610b6-138">Описание</span><span class="sxs-lookup"><span data-stu-id="610b6-138">Description</span></span> |  
|:------|:------|:------|  
| <span data-ttu-id="610b6-139">top</span><span class="sxs-lookup"><span data-stu-id="610b6-139">top</span></span> | <span data-ttu-id="610b6-140">div, img, object</span><span class="sxs-lookup"><span data-stu-id="610b6-140">div, img, object</span></span> | <span data-ttu-id="610b6-141">Координата верхней границы элемента по оси Y; только в пикселях.</span><span class="sxs-lookup"><span data-stu-id="610b6-141">The y-axis coordinate of the div, img, or object element's top border, in pixels only. Default is 120 pixels.</span></span> <span data-ttu-id="610b6-142">По умолчанию используется значение 120 пикселей.</span><span class="sxs-lookup"><span data-stu-id="610b6-142">Default is 120 pixels.</span></span><p><span data-ttu-id="610b6-143">Пример: `top:140px`</span><span class="sxs-lookup"><span data-stu-id="610b6-143">Example: `top:140px`</span></span></p> |  
| <span data-ttu-id="610b6-144">left</span><span class="sxs-lookup"><span data-stu-id="610b6-144">left</span></span> |  <span data-ttu-id="610b6-145">div, img, object</span><span class="sxs-lookup"><span data-stu-id="610b6-145">div, img, object</span></span>  | <span data-ttu-id="610b6-146">Координата левой границы элемента по оси X; только в пикселях.</span><span class="sxs-lookup"><span data-stu-id="610b6-146">The x-axis coordinate of the div, img, or object element's left border, in pixels only. Default is 48 pixels.</span></span> <span data-ttu-id="610b6-147">По умолчанию используется значение 48 пикселей.</span><span class="sxs-lookup"><span data-stu-id="610b6-147">Default is 48 pixels.</span></span><p><span data-ttu-id="610b6-148">Пример: `left:95px`</span><span class="sxs-lookup"><span data-stu-id="610b6-148">Example: `left:95px`</span></span></p> |  
| <span data-ttu-id="610b6-149">width</span><span class="sxs-lookup"><span data-stu-id="610b6-149">width</span></span> |  <span data-ttu-id="610b6-150">div, img</span><span class="sxs-lookup"><span data-stu-id="610b6-150">div, img</span></span>  | <span data-ttu-id="610b6-151">Ширина элемента; только в пикселях.</span><span class="sxs-lookup"><span data-stu-id="610b6-151">The width of the div or img element, in pixels only.</span></span><p><span data-ttu-id="610b6-152">Пример: `width:480px`</span><span class="sxs-lookup"><span data-stu-id="610b6-152">Example: `width:480px`</span></span></p> |  
| <span data-ttu-id="610b6-153">height</span><span class="sxs-lookup"><span data-stu-id="610b6-153">height</span></span> | <span data-ttu-id="610b6-154">img</span><span class="sxs-lookup"><span data-stu-id="610b6-154">img</span></span> | <span data-ttu-id="610b6-155">Высота элемента; только в пикселях.</span><span class="sxs-lookup"><span data-stu-id="610b6-155">The height of the thumbnail, in pixels.</span></span> <span data-ttu-id="610b6-156">Для элементов div высота рассчитывается в среде выполнения, и система игнорирует любое заданное значение высоты.</span><span class="sxs-lookup"><span data-stu-id="610b6-156">The height of the img element, in pixels only.  For div elements, height is calculated at runtime and any specified height value is ignored.</span></span><p><span data-ttu-id="610b6-157">Пример: `height:665px`</span><span class="sxs-lookup"><span data-stu-id="610b6-157">Example: `height:665px`</span></span></p> |  
 
<span data-ttu-id="610b6-158">Система игнорирует другие атрибуты положения, например `z-index`.</span><span class="sxs-lookup"><span data-stu-id="610b6-158">Other position attributes, such as z-index`z-index`, are ignored.</span></span> <span data-ttu-id="610b6-159">Для изображений с абсолютными положениями можно использовать атрибут `data-render-src` или `src`.</span><span class="sxs-lookup"><span data-stu-id="610b6-159">Absolute positioned images can use either the `data-render-src` or `src` attribute.</span></span>


<a name="request-response-info"></a>
## <a name="response-information"></a><span data-ttu-id="610b6-160">Информация в ответе</span><span class="sxs-lookup"><span data-stu-id="610b6-160">Response information</span></span>
<span data-ttu-id="610b6-161">API OneNote возвращает указанные ниже сведения в ответе.</span><span class="sxs-lookup"><span data-stu-id="610b6-161">The onnvshort API returns the following information in the response.</span></span>

| <span data-ttu-id="610b6-162">Данные в ответе</span><span class="sxs-lookup"><span data-stu-id="610b6-162">Response data</span></span> | <span data-ttu-id="610b6-163">Описание</span><span class="sxs-lookup"><span data-stu-id="610b6-163">Description</span></span> |  
|:------|:------|  
| <span data-ttu-id="610b6-164">код успешного завершения действия;</span><span class="sxs-lookup"><span data-stu-id="610b6-164">Success code</span></span> | <span data-ttu-id="610b6-165">Код состояния HTTP 201 при успешном выполнении запроса POST и код состояния HTTP 204 при успешном выполнении запроса PATCH.</span><span class="sxs-lookup"><span data-stu-id="610b6-165">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |  
| <span data-ttu-id="610b6-166">Ошибки</span><span class="sxs-lookup"><span data-stu-id="610b6-166">Errors</span></span> | <span data-ttu-id="610b6-167">Дополнительные сведения об ошибках OneNote, которые может возвращать Microsoft Graph, см. в статье [Коды ошибок для API OneNote в Microsoft Graph](onenote_error_codes.md).</span><span class="sxs-lookup"><span data-stu-id="610b6-167">Read [Error codes for OneNote APIs in Microsoft Graph](onenote_error_codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
  


<a name="permissions"></a>
## <a name="permissions"></a><span data-ttu-id="610b6-168">Разрешения</span><span class="sxs-lookup"><span data-stu-id="610b6-168">Permissions</span></span>

<span data-ttu-id="610b6-169">Чтобы можно было создавать или изменять страницы OneNote, вам придется запросить соответствующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="610b6-169">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="610b6-170">Выберите минимальный уровень разрешений, необходимый для работы вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="610b6-170">Choose the lowest level of permissions that your app needs to do its work.</span></span>

### <a name="permissions-for-post-pages"></a><span data-ttu-id="610b6-171">Разрешения для _запросов POST со страницами_</span><span class="sxs-lookup"><span data-stu-id="610b6-171">Permissions for _POST pages_</span></span> 
- <span data-ttu-id="610b6-172">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="610b6-172">Notes.Create</span></span>
- <span data-ttu-id="610b6-173">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="610b6-173">Notes.ReadWrite</span></span>
- <span data-ttu-id="610b6-174">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="610b6-174">Notes.ReadWrite.All</span></span>  


### <a name="permissions-for-patch-pages"></a><span data-ttu-id="610b6-175">Разрешения для _запросов PATCH со страницами_</span><span class="sxs-lookup"><span data-stu-id="610b6-175">Permissions for _PATCH pages_</span></span> 

- <span data-ttu-id="610b6-176">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="610b6-176">Notes.ReadWrite</span></span>
- <span data-ttu-id="610b6-177">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="610b6-177">Notes.ReadWrite.All</span></span>

<span data-ttu-id="610b6-178">Дополнительные сведения об областях разрешений и принципах их работы см. в разделе [Разрешения OneNote](permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="610b6-178">For more information about how permission scopes work, see [OneNote permission scopes](permissions_reference.md#notes-permissions).</span></span>


<a name="see-also"></a>
## <a name="additional-resources"></a><span data-ttu-id="610b6-179">Дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="610b6-179">Additional resources</span></span>

- [<span data-ttu-id="610b6-180">Создание страниц OneNote</span><span class="sxs-lookup"><span data-stu-id="610b6-180">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="610b6-181">Обновление содержимого страницы OneNote</span><span class="sxs-lookup"><span data-stu-id="610b6-181">Update OneNote page content</span></span>](onenote_update_page.md)
- [<span data-ttu-id="610b6-182">Интеграция с OneNote</span><span class="sxs-lookup"><span data-stu-id="610b6-182">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="610b6-183">Блог разработчиков OneNote</span><span class="sxs-lookup"><span data-stu-id="610b6-183">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="610b6-184">Вопросы разработки OneNote на сайте Stack Overflow</span><span class="sxs-lookup"><span data-stu-id="610b6-184">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="610b6-185">Репозитории GitHub OneNote</span><span class="sxs-lookup"><span data-stu-id="610b6-185">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  

