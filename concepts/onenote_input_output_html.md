# <a name="input-and-output-html-in-onenote-pages"></a><span data-ttu-id="9fee0-101">Входной и выходной HTML-код на страницах OneNote</span><span class="sxs-lookup"><span data-stu-id="9fee0-101">Input and output HTML in OneNote pages</span></span>

<span data-ttu-id="9fee0-102">HTML-код, определяющий содержимое и структуру страницы при [создании](onenote-create-page.md) или [обновлении](onenote_update_page.md) страницы OneNote, называется *входным HTML-кодом*.</span><span class="sxs-lookup"><span data-stu-id="9fee0-102">The HTML that defines the page content and structure when you [create](onenote-create-page.md) or [update](onenote_update_page.md) a OneNote page is called *input HTML*.</span></span> 

<span data-ttu-id="9fee0-103">HTML-код, возвращаемый при [получении содержимого страницы](onenote-get-content.md), называется *выходным HTML-кодом*.</span><span class="sxs-lookup"><span data-stu-id="9fee0-103">The HTML that's returned when you [get page content](onenote-get-content.md) is called *output HTML*.</span></span> <span data-ttu-id="9fee0-104">Выходной HTML-код не совпадает со входным.</span><span class="sxs-lookup"><span data-stu-id="9fee0-104">Output HTML won't be the same as input HTML.</span></span>

<span data-ttu-id="9fee0-105">API OneNote в Microsoft Graph сохраняют семантическое содержимое и базовую структуру входного HTML-кода, но преобразовывают ее в набор [поддерживаемых элементов HTML и свойств CSS](onenote-create-page.md#supported-html-and-css-for-onenote-pages).</span><span class="sxs-lookup"><span data-stu-id="9fee0-105">The OneNote APIs in Microsoft Graph preserve the semantic content and basic structure of the input HTML, but convert it to a set of [supported HTML elements and CSS properties](onenote-create-page.md#supported-html-and-css-for-onenote-pages).</span></span> <span data-ttu-id="9fee0-106">API также добавляют настраиваемые атрибуты, поддерживающие функции OneNote.</span><span class="sxs-lookup"><span data-stu-id="9fee0-106">The APIs also add custom attributes that support OneNote features.</span></span>
 
<span data-ttu-id="9fee0-107">В этой статье описываются основные элементы и атрибуты входного и выходного HTML-кода.</span><span class="sxs-lookup"><span data-stu-id="9fee0-107">This article describes the principal elements and attributes of input and output HTML.</span></span> <span data-ttu-id="9fee0-108">Разбираться во входном HTML-коде полезно при создании и обновлении содержимого страницы, а в выходном — при анализе возвращаемого содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="9fee0-108">It can be helpful to understand input HTML when you're creating or updating page content, and output HTML when you're parsing returned page content.</span></span> 

## <a name="body-element"></a><span data-ttu-id="9fee0-109">элемент Body</span><span class="sxs-lookup"><span data-stu-id="9fee0-109">Body element</span></span>

<span data-ttu-id="9fee0-110">HTML-содержимое в тексте страницы представляет ее содержимое и структуру, в том числе ресурсы изображений и файлов.</span><span class="sxs-lookup"><span data-stu-id="9fee0-110">The HTML content in the page body represents the page content and structure, including image and file resources.</span></span> <span data-ttu-id="9fee0-111">Входной и выходной HTML-код для элемента **body** может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="9fee0-111">The **body** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="9fee0-112">Входные атрибуты</span><span class="sxs-lookup"><span data-stu-id="9fee0-112">Input attributes</span></span>

|<span data-ttu-id="9fee0-113">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="9fee0-113">Input attribute</span></span>|<span data-ttu-id="9fee0-114">Описание</span><span class="sxs-lookup"><span data-stu-id="9fee0-114">Description</span></span>|
|:------|:------|
| <span data-ttu-id="9fee0-115">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="9fee0-115">data-absolute-enabled</span></span> | <span data-ttu-id="9fee0-116">Указывает, поддерживают ли во входном тексте элементы с [абсолютным положением](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-116">Indicates whether the input body supports [absolute positioned](onenote-abs-pos.md) elements.</span></span> |
| <span data-ttu-id="9fee0-117">стиль</span><span class="sxs-lookup"><span data-stu-id="9fee0-117">style</span></span> | <p><span data-ttu-id="9fee0-118">Свойства CSS [style](#styles) для основного текста.</span><span class="sxs-lookup"><span data-stu-id="9fee0-118">The CSS [style](#styles) properties of the body.</span></span> <span data-ttu-id="9fee0-119">В выходном HTML-коде входные параметры могут быть встроены в соответствующие дочерние элементы.</span><span class="sxs-lookup"><span data-stu-id="9fee0-119">In the output HTML, input settings might be returned inline on appropriate child elements.</span></span></p><p><span data-ttu-id="9fee0-120">В настоящее время цвет фона не поддерживается для элемента **body**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-120">Background color is not currently supported for the **body** element.</span></span></p> |
 

#### <a name="output-attributes"></a><span data-ttu-id="9fee0-121">Выходные атрибуты</span><span class="sxs-lookup"><span data-stu-id="9fee0-121">Output attributes</span></span>

|<span data-ttu-id="9fee0-122">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="9fee0-122">Output attribute</span></span>|<span data-ttu-id="9fee0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9fee0-123">Description</span></span>|
|:------|:------|
| <span data-ttu-id="9fee0-124">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="9fee0-124">data-absolute-enabled</span></span> | <span data-ttu-id="9fee0-125">Указывает, поддерживаются ли в тексте элементы с [абсолютным положением](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-125">Indicates whether the body supports [absolute positioned](onenote-abs-pos.md) elements.</span></span> <span data-ttu-id="9fee0-126">В выходном HTML-коде всегда задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-126">Always **true** in output HTML.</span></span> |
| <span data-ttu-id="9fee0-127">стиль</span><span class="sxs-lookup"><span data-stu-id="9fee0-127">style</span></span> | <span data-ttu-id="9fee0-128">Свойства **font-family** и **font-size** основного текста.</span><span class="sxs-lookup"><span data-stu-id="9fee0-128">The **font-family** and **font-size** properties of the body.</span></span> |


## <a name="div-elements"></a><span data-ttu-id="9fee0-129">элементы Div</span><span class="sxs-lookup"><span data-stu-id="9fee0-129">Div elements</span></span>

<span data-ttu-id="9fee0-130">Элементы **Div** содержат текст, изображения и другое содержимое.</span><span class="sxs-lookup"><span data-stu-id="9fee0-130">**Div** elements contain text, images, and other content.</span></span> <span data-ttu-id="9fee0-131">Входной и выходной HTML-код для элемента **div** может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="9fee0-131">A **div** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="9fee0-132">Входные атрибуты</span><span class="sxs-lookup"><span data-stu-id="9fee0-132">Input attributes</span></span>

|<span data-ttu-id="9fee0-133">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="9fee0-133">Input attribute</span></span>|<span data-ttu-id="9fee0-134">Описание</span><span class="sxs-lookup"><span data-stu-id="9fee0-134">Description</span></span>|
|:------|:------|
| <span data-ttu-id="9fee0-135">data-id</span><span class="sxs-lookup"><span data-stu-id="9fee0-135">data-id</span></span> | <span data-ttu-id="9fee0-136">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="9fee0-136">A reference for the element.</span></span><br/><br/><span data-ttu-id="9fee0-137">Используется для [обновления содержимого страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-137">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="9fee0-138">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="9fee0-138">data-render-fallback</span></span> | <span data-ttu-id="9fee0-139">Резервное действие в случае ошибки [извлечения](onenote-extract-data.md): **render** (по умолчанию) или **none**</span><span class="sxs-lookup"><span data-stu-id="9fee0-139">The fallback action if the [extraction](onenote-extract-data.md) fails: **render** (default) or **none**.</span></span> |
| <span data-ttu-id="9fee0-140">data-render-method</span><span class="sxs-lookup"><span data-stu-id="9fee0-140">data-render-method</span></span> | <span data-ttu-id="9fee0-141">Выполняемый метод [извлечения](onenote-extract-data.md), например:</span><span class="sxs-lookup"><span data-stu-id="9fee0-141">The [extraction](onenote-extract-data.md) method to perform, for example:  or .</span></span><br/><span data-ttu-id="9fee0-142">`extract.businesscard` или `extract.recipe`</span><span class="sxs-lookup"><span data-stu-id="9fee0-142">`extract.businesscard` or `extract.recipe`</span></span> |
| <span data-ttu-id="9fee0-143">data-render-src</span><span class="sxs-lookup"><span data-stu-id="9fee0-143">data-render-src</span></span> | <span data-ttu-id="9fee0-144">Источник контента для [извлечения](onenote-extract-data.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-144">The content source for the [extraction](onenote-extract-data.md).</span></span> |
| <span data-ttu-id="9fee0-145">стиль</span><span class="sxs-lookup"><span data-stu-id="9fee0-145">style</span></span> | <span data-ttu-id="9fee0-146">Свойства положения, размера, шрифта и цвета для div:</span><span class="sxs-lookup"><span data-stu-id="9fee0-146">The position, size, font, and color properties for the div:</span></span> <ul><li><span data-ttu-id="9fee0-147">**положение** (только **абсолютное**), **left**, **top** и **width** (высота для элементов div настраивается автоматически)</span><span class="sxs-lookup"><span data-stu-id="9fee0-147">**position** (**absolute** only), **left**, **top**, and **width** (height is auto-configured for divs)</span></span><br/><br/><span data-ttu-id="9fee0-148">Используется для создания разделителя div с [абсолютным положением](onenote-abs-pos.md), только если разделитель является непосредственным дочерним элементом основного текста, для которого задан атрибут `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="9fee0-148">Used to create an [absolute positioned](onenote-abs-pos.md) div, only if the div is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="9fee0-149">Пример: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="9fee0-149">Example: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span></li><li><span data-ttu-id="9fee0-p108">Свойства CSS [style](#styles) элемента. В выходных данных HTML эти значения возвращаются встроенными в соответствующие дочерние элементы.</span><span class="sxs-lookup"><span data-stu-id="9fee0-p108">The CSS [style](#styles) properties of the element. In the output HTML, these values are returned inline on appropriate child elements.</span></span></li></ul> |
 

<span data-ttu-id="9fee0-152">API OneNote в Microsoft Graph заключают все содержимое основного текста по крайней мере в один разделитель.</span><span class="sxs-lookup"><span data-stu-id="9fee0-152">The OneNote APIs in Microsoft Graph wrap all body content in at least one div.</span></span> <span data-ttu-id="9fee0-153">API создает разделитель по умолчанию (с атрибутом `data-id="_default"`) для содержимого основного текста, если:</span><span class="sxs-lookup"><span data-stu-id="9fee0-153">The API creates a default div (attributed with `data-id="_default"`) to contain the body content if:</span></span>

- <span data-ttu-id="9fee0-154">Входной атрибут **data-absolute-enabled** элемента body пропущен или для него задано значение **false**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-154">The input body element's **data-absolute-enabled** attribute is omitted or set to **false**.</span></span> <span data-ttu-id="9fee0-155">В этом случае все содержимое основного текста помещается в разделитель по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9fee0-155">In this case, all body content is put in the default div.</span></span>

- <span data-ttu-id="9fee0-156">Для входного атрибута **data-absolute-enabled** элемента body задано значение **true**, но входной HTML-код содержит непосредственные дочерние элементы&nbsp;**div**, **img** или **object** без [абсолютного положения](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-156">The input body element's **data-absolute-enabled** attribute is **true**, but the input HTML contains direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements.</span></span> <span data-ttu-id="9fee0-157">В этом случае непосредственные дочерние элементы &nbsp;**div**, **img** или **object** без [абсолютного положения](onenote-abs-pos.md) помещаются в разделитель по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9fee0-157">In this case, direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements are put in the default div.</span></span>


#### <a name="output-attributes"></a><span data-ttu-id="9fee0-158">Выходные атрибуты</span><span class="sxs-lookup"><span data-stu-id="9fee0-158">Output attributes</span></span>

|<span data-ttu-id="9fee0-159">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="9fee0-159">Output attribute</span></span>|<span data-ttu-id="9fee0-160">Описание</span><span class="sxs-lookup"><span data-stu-id="9fee0-160">Description</span></span>|
|:------|:------|
| <span data-ttu-id="9fee0-161">data-id</span><span class="sxs-lookup"><span data-stu-id="9fee0-161">data-id</span></span> | <span data-ttu-id="9fee0-162">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="9fee0-162">A reference for the element.</span></span><br/><br/><span data-ttu-id="9fee0-163">Используется для [обновления содержимого страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-163">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="9fee0-164">идентификатор</span><span class="sxs-lookup"><span data-stu-id="9fee0-164">id</span></span> | <span data-ttu-id="9fee0-165">Уникальный сгенерированный ИД элемента.</span><span class="sxs-lookup"><span data-stu-id="9fee0-165">A unique, generated ID for the element.</span></span> <span data-ttu-id="9fee0-166">Возвращается [запросами GET к конечной точке *content* страницы](../api-reference/v1.0/api/page_get.md) при использовании параметра запроса `includeIDs=true`.</span><span class="sxs-lookup"><span data-stu-id="9fee0-166">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="9fee0-167">Используется для [обновления содержимого страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-167">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="9fee0-168">стиль</span><span class="sxs-lookup"><span data-stu-id="9fee0-168">style</span></span> | <span data-ttu-id="9fee0-169">Свойства позиции и размера разделителя.</span><span class="sxs-lookup"><span data-stu-id="9fee0-169">The position and size properties of the div.</span></span> |
 
### <a name="non-contributing-divs"></a><span data-ttu-id="9fee0-170">Вспомогательные разделители</span><span class="sxs-lookup"><span data-stu-id="9fee0-170">Non-contributing divs</span></span>

<span data-ttu-id="9fee0-171">Если элемент **div** во входных данных HTML не входит в структуру страницы и не переносит сведения, используемые приложением OneNote, API перемещает содержимое разделителя в родительский или используемый по умолчанию разделитель.</span><span class="sxs-lookup"><span data-stu-id="9fee0-171">When a **div** element in the input HTML does not contribute to the page structure or carry information that OneNote uses, the API moves the div's content into the parent or default div.</span></span> <span data-ttu-id="9fee0-172">Это процесс показан в приведенных ниже примерах.</span><span class="sxs-lookup"><span data-stu-id="9fee0-172">This is illustrated in the following examples.</span></span>

#### <a name="input-html"></a><span data-ttu-id="9fee0-173">Входной HTML-код</span><span class="sxs-lookup"><span data-stu-id="9fee0-173">Input HTML</span></span>

<span data-ttu-id="9fee0-174">Содержит вспомогательный, вложенный div.</span><span class="sxs-lookup"><span data-stu-id="9fee0-174">Contains a non-contributing, nested div.</span></span>

```html
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body>
        <div>
            <p>Some text</p>
            <div>
                <p>More text inside a div that doesn't define page structure</p>
            </div>
        </div>
    </body>
</html>
```

#### <a name="output-html"></a><span data-ttu-id="9fee0-175">Выходной HTML-код</span><span class="sxs-lookup"><span data-stu-id="9fee0-175">Output HTML</span></span>

> <span data-ttu-id="9fee0-176">**Примечание.** Содержимое разделителя было перемещено в родительский разделитель, а вложенные теги `<div>` были удалены.</span><span class="sxs-lookup"><span data-stu-id="9fee0-176">**Note:** The div's content was moved to the parent div and the nested `<div>` tags have been removed.</span></span> <span data-ttu-id="9fee0-177">Разделитель был бы сохранен, если бы в нем были определены какие-либо семантические сведения, такие как **data-id** (пример: `<div data-id="keep-me">`).</span><span class="sxs-lookup"><span data-stu-id="9fee0-177">The div would have been preserved if it defined any semantic information, such as a **data-id** (example: `<div data-id="keep-me">`).</span></span>

```html
<html htmlns="http://www.w3.org/1999/xhtml" lang="en-US">
    <head>
        <title>Page Title</title>
    </head>
    <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11px">
        <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
            <p>Some text</p>
            <p>More text inside a nested div</p>
        </div>
    </body>
</html>
```


## <a name="img-elements"></a><span data-ttu-id="9fee0-178">элементы Img</span><span class="sxs-lookup"><span data-stu-id="9fee0-178">Img elements</span></span>

<span data-ttu-id="9fee0-179">Для представления изображений на страницах OneNote используются элементы **img**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-179">Images on OneNote pages are represented by **img** elements.</span></span> <span data-ttu-id="9fee0-180">Входной и выходной HTML-код для элемента **img** может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="9fee0-180">An **img** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="9fee0-181">Входные атрибуты</span><span class="sxs-lookup"><span data-stu-id="9fee0-181">Input attributes</span></span>

|<span data-ttu-id="9fee0-182">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="9fee0-182">Input attribute</span></span>|<span data-ttu-id="9fee0-183">Описание</span><span class="sxs-lookup"><span data-stu-id="9fee0-183">Description</span></span>|
|:------|:------|
| <span data-ttu-id="9fee0-184">alt</span><span class="sxs-lookup"><span data-stu-id="9fee0-184">alt</span></span> | <span data-ttu-id="9fee0-185">Предоставленный замещающий текст для изображения.</span><span class="sxs-lookup"><span data-stu-id="9fee0-185">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="9fee0-186">data-id</span><span class="sxs-lookup"><span data-stu-id="9fee0-186">data-id</span></span> | <span data-ttu-id="9fee0-187">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="9fee0-187">A reference for the element.</span></span><br/><br/><span data-ttu-id="9fee0-188">Используется для [обновления содержимого страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-188">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="9fee0-189">data-render-src</span><span class="sxs-lookup"><span data-stu-id="9fee0-189">data-render-src</span></span> |<span data-ttu-id="9fee0-190">Должно было задано значение **data-render-src** или **src**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-190">Either **data-render-src** or **src** is required.</span></span><br/><br/><span data-ttu-id="9fee0-191">Веб-страница, которая будет отображаться в виде битового изображения на странице OneNote:</span><span class="sxs-lookup"><span data-stu-id="9fee0-191">The webpage to render as a bit-mapped image on the OneNote page:</span></span><br/><br/> <span data-ttu-id="9fee0-192">- `data-render-src="http://..."` для общедоступного URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="9fee0-192">- `data-render-src="http://..."` for a public URL.</span></span><br/><br/> <span data-ttu-id="9fee0-193">- `data-render-src="name:BlockName"` для части изображения в блоке Presentation [составного запроса](../api-reference/v1.0/api/section_post_pages.md#example).</span><span class="sxs-lookup"><span data-stu-id="9fee0-193">- `data-render-src="name:BlockName"` for an image part in the "Presentation" block of a [multipart request](../api-reference/v1.0/api/section_post_pages.md#example).</span></span><br/><br/><span data-ttu-id="9fee0-194">Этот метод удобно использовать, если веб-страница слишком сложна для достоверного отображения в OneNote или для использования страницы необходимы учетные данные.</span><span class="sxs-lookup"><span data-stu-id="9fee0-194">This method is useful when the webpage is more complex than the OneNote page can faithfully render, or when the page requires login credentials.</span></span>|
| <span data-ttu-id="9fee0-195">data-tag</span><span class="sxs-lookup"><span data-stu-id="9fee0-195">data-tag</span></span> | <span data-ttu-id="9fee0-196">[Тег заметки](onenote-note-tags.md) для элемента.</span><span class="sxs-lookup"><span data-stu-id="9fee0-196">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="9fee0-197">стиль</span><span class="sxs-lookup"><span data-stu-id="9fee0-197">style</span></span> |<span data-ttu-id="9fee0-198">Свойства положения и размера изображения: **position** (только **absolute**), **left**, **top**, **width** и **height**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-198">The position and size properties for the image: **position** (**absolute** only), **left**, **top**, **width**, and **height**.</span></span><br/><br/><span data-ttu-id="9fee0-199">Размер можно задать для любого изображения.</span><span class="sxs-lookup"><span data-stu-id="9fee0-199">Size can be set on any image.</span></span><br/><br/><span data-ttu-id="9fee0-200">Свойства положения используются для создания изображения с [абсолютным положением](onenote-abs-pos.md), только если изображение является непосредственным дочерним элементом основного текста, для которого задан атрибут `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="9fee0-200">Position properties are used to create an [absolute positioned](onenote-abs-pos.md) image, only if the image is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="9fee0-201">Пример: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="9fee0-201">Example: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span><br/><br/><span data-ttu-id="9fee0-202">В выходном HTML-коде размеры изображения возвращаются по отдельности через атрибуты **width** и **height**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-202">In the output HTML, the image size is returned separately in **width** and **height** attributes.</span></span> |
| <span data-ttu-id="9fee0-203">src</span><span class="sxs-lookup"><span data-stu-id="9fee0-203">src</span></span> |<span data-ttu-id="9fee0-204">Должно было задано значение **src** или **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-204">Either **src** or **data-render-src** is required.</span></span><br/><br/><span data-ttu-id="9fee0-205">Изображение, отображаемое на странице OneNote:</span><span class="sxs-lookup"><span data-stu-id="9fee0-205">The image to render on the OneNote page:</span></span><br/><br/><span data-ttu-id="9fee0-206">- `src="http://..."` для URL-адреса общедоступного изображения в Интернете.</span><span class="sxs-lookup"><span data-stu-id="9fee0-206">- `src="http://..."` for a URL to a publicly available image on the internet.</span></span><br/><br/> <span data-ttu-id="9fee0-207">- `src="name:BlockName"` : именованная часть составного запроса, представляющая изображение.</span><span class="sxs-lookup"><span data-stu-id="9fee0-207">- `src="name:BlockName"` for a named part in a multipart request that represents the image.</span></span>|
| <span data-ttu-id="9fee0-208">ширина, высота</span><span class="sxs-lookup"><span data-stu-id="9fee0-208">width, height</span></span> | <span data-ttu-id="9fee0-209">Ширина и высота изображения в пикселях, но без обозначения px.</span><span class="sxs-lookup"><span data-stu-id="9fee0-209">The width or height of the image, in pixels but without the px.</span></span> <span data-ttu-id="9fee0-210">Пример: `width="400"`</span><span class="sxs-lookup"><span data-stu-id="9fee0-210">Example: `width="400"`</span></span> |
 
> <span data-ttu-id="9fee0-211">**Примечание.** API OneNote автоматически определяют тип входного изображения и возвращают его в качестве атрибута **data-fullres-src-type** во входном HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="9fee0-211">**Note:** The OneNote APIs automatically detect the input image type, and returns it as the **data-fullres-src-type** in the output HTML.</span></span> <span data-ttu-id="9fee0-212">API также возвращает тип оптимизированного изображения в атрибуте **data-src-type**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-212">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 

#### <a name="output-attributes"></a><span data-ttu-id="9fee0-213">Выходные атрибуты</span><span class="sxs-lookup"><span data-stu-id="9fee0-213">Output attributes</span></span>

|<span data-ttu-id="9fee0-214">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="9fee0-214">Output attribute</span></span>|<span data-ttu-id="9fee0-215">Описание</span><span class="sxs-lookup"><span data-stu-id="9fee0-215">Description</span></span>|
|:------|:------|
| <span data-ttu-id="9fee0-216">alt</span><span class="sxs-lookup"><span data-stu-id="9fee0-216">alt</span></span> | <span data-ttu-id="9fee0-217">Предоставленный замещающий текст для изображения.</span><span class="sxs-lookup"><span data-stu-id="9fee0-217">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="9fee0-218">data-id</span><span class="sxs-lookup"><span data-stu-id="9fee0-218">data-id</span></span> | <span data-ttu-id="9fee0-219">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="9fee0-219">A reference for the element.</span></span><br/><br/><span data-ttu-id="9fee0-220">Используется для [обновления содержимого страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-220">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="9fee0-221">data-index</span><span class="sxs-lookup"><span data-stu-id="9fee0-221">data-index</span></span> | <span data-ttu-id="9fee0-p118">Позиция изображения. Для поддержки [разделения изображений](#split-images).</span><span class="sxs-lookup"><span data-stu-id="9fee0-p118">The position of the image. For [split image](#split-images) support.</span></span> |
| <span data-ttu-id="9fee0-224">data-fullres-src</span><span class="sxs-lookup"><span data-stu-id="9fee0-224">data-fullres-src</span></span> | <span data-ttu-id="9fee0-225">Конечная точка версии изображения, которая была изначально внедрена на странице.</span><span class="sxs-lookup"><span data-stu-id="9fee0-225">The endpoint for the version of the image resource that was originally embedded in the page.</span></span> |
| <span data-ttu-id="9fee0-226">data-fullres-src-type</span><span class="sxs-lookup"><span data-stu-id="9fee0-226">data-fullres-src-type</span></span> | <span data-ttu-id="9fee0-227">Тип мультимедиа для ресурса **data-fullres-src**, например `image/png` или `image/jpeg`.</span><span class="sxs-lookup"><span data-stu-id="9fee0-227">The media type of the **data-fullres-src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="9fee0-228">data-options</span><span class="sxs-lookup"><span data-stu-id="9fee0-228">data-options</span></span> | <span data-ttu-id="9fee0-p119">Тип источника: **printout** для PDF-файлов или **splitimage** для всех остальных. Применяется только к [разделенным изображениям](#split-images), созданным с помощью атрибута **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-p119">The source type: **printout** for PDF files or **splitimage** for all others. Applies only to [split images](#split-images) created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="9fee0-231">data-render-original-src</span><span class="sxs-lookup"><span data-stu-id="9fee0-231">data-render-original-src</span></span> | <span data-ttu-id="9fee0-232">Исходный URL-адрес источника изображения, если исходное изображение находится в общедоступной части Интернета и создано с использованием атрибута **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-232">The original source URL of the image, if the source image is from the public internet and was created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="9fee0-233">data-src-type</span><span class="sxs-lookup"><span data-stu-id="9fee0-233">data-src-type</span></span> | <span data-ttu-id="9fee0-234">Тип мультимедиа для ресурса **src**, например `image/png` или `image/jpeg`.</span><span class="sxs-lookup"><span data-stu-id="9fee0-234">The media type of the **src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="9fee0-235">data-tag</span><span class="sxs-lookup"><span data-stu-id="9fee0-235">data-tag</span></span> | <span data-ttu-id="9fee0-236">[Тег заметки](onenote-note-tags.md) для элемента.</span><span class="sxs-lookup"><span data-stu-id="9fee0-236">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="9fee0-237">идентификатор</span><span class="sxs-lookup"><span data-stu-id="9fee0-237">id</span></span> | <span data-ttu-id="9fee0-238">Уникальный сгенерированный ИД элемента.</span><span class="sxs-lookup"><span data-stu-id="9fee0-238">A unique, generated ID for the element.</span></span> <span data-ttu-id="9fee0-239">Возвращается [запросами GET к конечной точке *content* страницы](../api-reference/v1.0/api/page_get.md) при использовании параметра запроса `includeIDs=true`.</span><span class="sxs-lookup"><span data-stu-id="9fee0-239">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="9fee0-240">Используется для [обновления содержимого страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-240">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="9fee0-241">src</span><span class="sxs-lookup"><span data-stu-id="9fee0-241">src</span></span> | <span data-ttu-id="9fee0-242">Конечная точка версии изображения, оптимизированного для веб-браузеров, а также мобильных телефонов и планшетов.</span><span class="sxs-lookup"><span data-stu-id="9fee0-242">The endpoint for the version of the image resource that has been optimized for web browsers and mobile and tablet form factors.</span></span> |
| <span data-ttu-id="9fee0-243">стиль</span><span class="sxs-lookup"><span data-stu-id="9fee0-243">style</span></span> | <span data-ttu-id="9fee0-244">Свойства позиции изображения.</span><span class="sxs-lookup"><span data-stu-id="9fee0-244">The position properties of the image.</span></span> |
| <span data-ttu-id="9fee0-245">ширина, высота</span><span class="sxs-lookup"><span data-stu-id="9fee0-245">width, height</span></span> | <span data-ttu-id="9fee0-246">Ширина или высота изображения в пикселях.</span><span class="sxs-lookup"><span data-stu-id="9fee0-246">The width or height of the image, in pixels.</span></span> |
 

### <a name="output-html-examples-for-images"></a><span data-ttu-id="9fee0-247">Примеры выходного HTML-кода для изображений</span><span class="sxs-lookup"><span data-stu-id="9fee0-247">Output HTML examples for images</span></span>

<span data-ttu-id="9fee0-248">Выходные элементы **img** содержат конечные точки для ресурсов файлов изображений и типа изображения, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="9fee0-248">Output **img** elements contain endpoints for image file resources and the image type, as shown below.</span></span> <span data-ttu-id="9fee0-249">Вы можете отправлять отдельные [запросы GET к конечным точкам ресурсов изображений](../api-reference/v1.0/api/resource_get.md), чтобы получать их двоичное содержимое.</span><span class="sxs-lookup"><span data-stu-id="9fee0-249">You can make separate [GET requests to image resource endpoints](../api-reference/v1.0/api/resource_get.md) to retrieve their binary contents.</span></span>

```html
<img 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="9fee0-250">По умолчанию изображения не отображаются непосредственно в браузере, так как они являются личными и для их получения необходимо пройти проверку подлинности, как и для другого содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="9fee0-250">By default, images won't render directly in a browser because they are private and require authorization to retrieve them, like the rest of the page contents.</span></span> <span data-ttu-id="9fee0-251">Чтобы получить общедоступные URL-адреса ресурсов изображений на странице, включите параметр **preAuthenticated=true** в строку запроса при получении содержимого страницы (пример: `GET ../pages/{page-id}/content?preAuthenticated=true`).</span><span class="sxs-lookup"><span data-stu-id="9fee0-251">To get public URLs to the image resources on a page, include **preAuthenticated=true** in the query string when you retrieve the page content (example: `GET ../pages/{page-id}/content?preAuthenticated=true`).</span></span> <span data-ttu-id="9fee0-252">Возвращаемые общедоступные URL-адреса действительны в течение одного часа.</span><span class="sxs-lookup"><span data-stu-id="9fee0-252">The public URLs that are returned are valid for one hour.</span></span> 

#### <a name="image-with-public-url-when-preauthenticatedtrue-is-included-in-the-request"></a><span data-ttu-id="9fee0-253">Изображение с общедоступным URL-адресом (в запрос включен параметр _preAuthenticated=true_)</span><span class="sxs-lookup"><span data-stu-id="9fee0-253">Image with public URL when _preAuthenticated=true_ is included in the request</span></span>

```html
<img 
    width="170" height="128" 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-src-type="image/{type}" 
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-fullres-src-type="image/{type}"
/>
```

<span data-ttu-id="9fee0-254">В приведенных ниже примерах показаны сведения, которые может содержать элемент **img** в выходном HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="9fee0-254">The following examples show the information an **img** element might contain in the output HTML.</span></span>

#### <a name="image-with-web-ready-and-high-resolution-resources"></a><span data-ttu-id="9fee0-255">Изображение с ресурсами высокого разрешения для Интернета</span><span class="sxs-lookup"><span data-stu-id="9fee0-255">Image with web-ready and high resolution resources</span></span>

```html
<img
    src="{web-ready-image-resource-url}/$value"
    data-src-type="image/{type}"
    data-fullres-src="{high-resolution-image-resource-url}/$value"
    data-fullres-src-type="image/{type}"
    [data-render-original-src="{original-source-url-or-named-part}"]
    [data-id="{image-id}"]
    [alt="supplied alt text"]
    [width="345"] [height="180"]
    [style="..."] />
```

#### <a name="image-created-by-using-the-data-render-src-attribute"></a><span data-ttu-id="9fee0-256">Изображение, созданное с использованием атрибута *data-render-src*</span><span class="sxs-lookup"><span data-stu-id="9fee0-256">Image created by using the *data-render-src* attribute</span></span>

```html
<img
    src="{web-ready-image-resource-url}/$value"
    data-src-type="image/{type}"
    data-fullres-src="{high-resolution-image-resource-url}/$value"
    data-fullres-src-type="image/{type}"
    data-render-original-src="{original-source-url-or-named-part}"
    [data-id="{image-id}"]
    [data-index="{index-of-split-image}"]
    [data-options="{printout-or-splitimage}"]
    [alt="supplied alt text"]
    [width="1024"] [height="1900"]
    [style="..."] />
```

### <a name="split-images"></a><span data-ttu-id="9fee0-257">Разделенные изображения</span><span class="sxs-lookup"><span data-stu-id="9fee0-257">Split images</span></span>

<span data-ttu-id="9fee0-258">Изображения, созданные с использованием атрибута **data-render-src** (из URL-адреса страницы или именованной части), могут быть разделены на несколько компонентов для повышения производительности и удобства отрисовки.</span><span class="sxs-lookup"><span data-stu-id="9fee0-258">Images that are created using the **data-render-src** attribute (from a webpage URL or a named part) might be split into multiple component images for performance and rendering reasons.</span></span> <span data-ttu-id="9fee0-259">Всем компонентам изображения назначается одно и то же значение **data-id**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-259">Component images are all assigned the same **data-id** value.</span></span> <span data-ttu-id="9fee0-260">У каждого компонента изображения есть атрибут data-index с отсчетом от нуля, определяющий исходную вертикальную компоновку.</span><span class="sxs-lookup"><span data-stu-id="9fee0-260">Each component image has a zero-based data-index attribute that defines the original vertical layout.</span></span>

#### <a name="split-image-with-three-component-images"></a><span data-ttu-id="9fee0-261">Разделенное изображение с тремя компонентами</span><span class="sxs-lookup"><span data-stu-id="9fee0-261">Split image with three component images</span></span>

```html
<div data-id="multi-component-image" style="position:absolute;left:48px;top:120px;width:624px">
    <img
        src="{image-resource0-url}/$value"
        data-src-type="image/{type}"
        data-fullres-src="{image-resource0-url}/$value" 
        data-fullres-src-type="image/{type}" 
        data-index="0" 
        data-render-original-src="{original-source-url-or-named-part}"
        data-id="{same-image-id}" ... />
    <img 
        src="{image-resource1-url}/$value" 
        data-src-type="image/{type}" 
        data-fullres-src="{image-resource1-url}/$value" 
        data-fullres-src-type="image/{type}" 
        data-index="1" 
        data-render-original-src="{original-source-url-or-named-part}"
        data-id="{same-image-id}" ... />
    <img 
        src="{image-resource2-url}/$value" 
        data-src-type="image/{type}" 
        data-fullres-src="{image-resource2-url}/$value" 
        data-fullres-src-type="image/{type}" 
        data-index="2" 
        data-render-original-src=""{original-source-url-or-named-part}"
        data-id="{same-image-id}" ... />
</div>
```

<span data-ttu-id="9fee0-262">Так как пользователи могут перемещать изображения на странице, индексы могут возвращаться в измененном порядке.</span><span class="sxs-lookup"><span data-stu-id="9fee0-262">Because users can move the images on the page, the returned indexes might be out of order.</span></span> <span data-ttu-id="9fee0-263">Сортировка должна выполняться сверху вниз, а затем слева направо (если возникнут конфликты при вертикальной сортировке).</span><span class="sxs-lookup"><span data-stu-id="9fee0-263">Ordering should be in top to bottom y-order, then left to right x-order if there are y-order conflicts.</span></span>

## <a name="iframe-elements"></a><span data-ttu-id="9fee0-264">Элементы iframe</span><span class="sxs-lookup"><span data-stu-id="9fee0-264">iframe elements</span></span>

<span data-ttu-id="9fee0-265">Страницы OneNote могут содержать внедренные видео, представленные элементами **iframe**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-265">OneNote pages can contain embedded videos represented by **iframe** elements.</span></span> 

> <span data-ttu-id="9fee0-266">**Примечание.** Вы также можете [вложить видеофайл с помощью элемента **object**](onenote_images_files.md#adding-files).</span><span class="sxs-lookup"><span data-stu-id="9fee0-266">**Note:** You can also [attach a video file using an **object** element](onenote_images_files.md#adding-files).</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="9fee0-267">Входные атрибуты</span><span class="sxs-lookup"><span data-stu-id="9fee0-267">Input attributes</span></span>

|<span data-ttu-id="9fee0-268">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="9fee0-268">Input attribute</span></span>|<span data-ttu-id="9fee0-269">Описание</span><span class="sxs-lookup"><span data-stu-id="9fee0-269">Description</span></span>|
|:------|:------|
| <span data-ttu-id="9fee0-270">data-original-src</span><span class="sxs-lookup"><span data-stu-id="9fee0-270">data-original-src</span></span> | <span data-ttu-id="9fee0-271">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fee0-271">Required.</span></span> <span data-ttu-id="9fee0-272">URL-адрес источника видео.</span><span class="sxs-lookup"><span data-stu-id="9fee0-272">The URL of the video source.</span></span> <span data-ttu-id="9fee0-273">См. [список поддерживаемых источников видео](onenote_images_files.md#adding-videos).</span><span class="sxs-lookup"><span data-stu-id="9fee0-273">See the [list of supported video sources](onenote_images_files.md#adding-videos).</span></span> <br/><br/><span data-ttu-id="9fee0-274">Пример: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="9fee0-274">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span> |
| <span data-ttu-id="9fee0-275">ширина, высота</span><span class="sxs-lookup"><span data-stu-id="9fee0-275">width, height</span></span> | <span data-ttu-id="9fee0-276">Ширина или высота элемента iframe в пикселях.</span><span class="sxs-lookup"><span data-stu-id="9fee0-276">The width or height of the iframe, in pixels.</span></span> <span data-ttu-id="9fee0-277">Пример: `width=300`</span><span class="sxs-lookup"><span data-stu-id="9fee0-277">Example: `width=300`</span></span> |

#### <a name="output-attributes"></a><span data-ttu-id="9fee0-278">Выходные атрибуты</span><span class="sxs-lookup"><span data-stu-id="9fee0-278">Output attributes</span></span>

|<span data-ttu-id="9fee0-279">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="9fee0-279">Output attribute</span></span>|<span data-ttu-id="9fee0-280">Описание</span><span class="sxs-lookup"><span data-stu-id="9fee0-280">Description</span></span>|
|:------|:------|
| <span data-ttu-id="9fee0-281">data-original-src</span><span class="sxs-lookup"><span data-stu-id="9fee0-281">data-original-src</span></span> | <span data-ttu-id="9fee0-282">URL-адрес источника видео.</span><span class="sxs-lookup"><span data-stu-id="9fee0-282">The URL of the video source.</span></span> |
| <span data-ttu-id="9fee0-283">src</span><span class="sxs-lookup"><span data-stu-id="9fee0-283">src</span></span> | <span data-ttu-id="9fee0-284">Ссылка на видео, внедренное в страницу OneNote.</span><span class="sxs-lookup"><span data-stu-id="9fee0-284">A link to the video that is embedded in the OneNote page.</span></span> |
| <span data-ttu-id="9fee0-285">ширина, высота</span><span class="sxs-lookup"><span data-stu-id="9fee0-285">width, height</span></span> | <span data-ttu-id="9fee0-286">Ширина или высота элемента iframe в пикселях.</span><span class="sxs-lookup"><span data-stu-id="9fee0-286">The width or height of the iframe, in pixels.</span></span><br/><br/><span data-ttu-id="9fee0-287">Пример: `width=300`</span><span class="sxs-lookup"><span data-stu-id="9fee0-287">Example: `width=300`</span></span> |
 
### <a name="output-html-example-for-videos"></a><span data-ttu-id="9fee0-288">Пример выходного HTML-кода для видео</span><span class="sxs-lookup"><span data-stu-id="9fee0-288">Output HTML example for videos</span></span>

<span data-ttu-id="9fee0-289">Выходные элементы **iframe** содержат конечные точки, ссылающиеся на исходную страницу и видео, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="9fee0-289">Output **iframe** elements contain endpoints that link to the source page and video, as shown.</span></span> 

```html
<iframe 
    width="340" height="280" 
    data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" 
    src="https://www.youtube.com/embed/3Ztr44aKmQ8?feature=oembed&autoplay=true" />
``` 

## <a name="object-elements"></a><span data-ttu-id="9fee0-290">элементы Object</span><span class="sxs-lookup"><span data-stu-id="9fee0-290">Object elements</span></span>

<span data-ttu-id="9fee0-291">Страницы OneNote могут содержать вложения, представленные элементами **object**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-291">OneNote pages can contain file attachments represented by **object** elements.</span></span> <span data-ttu-id="9fee0-292">Входной и выходной HTML-код для элемента **object** может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="9fee0-292">An **object** element can contain the following attributes in the input and output HTML.</span></span>

> <span data-ttu-id="9fee0-293">**Примечание.** API OneNote также может отображать содержимое файлов в виде изображений на странице, если файл отправлен как изображение и использует атрибут **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-293">**Note:** The OneNote APIs can also render file content as images in a page when the file is sent as an image and uses the **data-render-src** attribute.</span></span>
> <span data-ttu-id="9fee0-294">Пример: `<img data-render-src="name:part-name" ... />`</span><span class="sxs-lookup"><span data-stu-id="9fee0-294">Example: `<img data-render-src="name:part-name" ... />`</span></span>
 

#### <a name="input-attributes"></a><span data-ttu-id="9fee0-295">Входные атрибуты</span><span class="sxs-lookup"><span data-stu-id="9fee0-295">Input attributes</span></span>

|<span data-ttu-id="9fee0-296">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="9fee0-296">Input attribute</span></span>|<span data-ttu-id="9fee0-297">Описание</span><span class="sxs-lookup"><span data-stu-id="9fee0-297">Description</span></span>|
|:------|:------|
| <span data-ttu-id="9fee0-298">данные</span><span class="sxs-lookup"><span data-stu-id="9fee0-298">data</span></span> | <span data-ttu-id="9fee0-299">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fee0-299">Required.</span></span> <span data-ttu-id="9fee0-300">Имя части, которая представляет файл в [составном запросе](../api-reference/v1.0/api/section_post_pages.md#example).</span><span class="sxs-lookup"><span data-stu-id="9fee0-300">The name of the part that represents the file in the [multipart request](../api-reference/v1.0/api/section_post_pages.md#example).</span></span> |
| <span data-ttu-id="9fee0-301">data-attachment</span><span class="sxs-lookup"><span data-stu-id="9fee0-301">data-attachment</span></span> | <span data-ttu-id="9fee0-p130">Обязательный параметр. Имя файла.</span><span class="sxs-lookup"><span data-stu-id="9fee0-p130">Required. The file name.</span></span> |
| <span data-ttu-id="9fee0-304">data-id</span><span class="sxs-lookup"><span data-stu-id="9fee0-304">data-id</span></span> | <span data-ttu-id="9fee0-305">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="9fee0-305">A reference for the element.</span></span><br/><br/><span data-ttu-id="9fee0-306">Используется для [обновления содержимого страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-306">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="9fee0-307">стиль</span><span class="sxs-lookup"><span data-stu-id="9fee0-307">style</span></span> | <span data-ttu-id="9fee0-308">Свойства положения и размера объекта: **position** (только **absolute**), **left**, **top** и **width**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-308">The position and size properties for the object: **position** (**absolute** only), **left**, **top**, and **width**.</span></span><br/><br/><span data-ttu-id="9fee0-309">Используется для создания объекта с [абсолютным положением](onenote-abs-pos.md), только если объект является непосредственным дочерним элементом основного текста, для которого задан атрибут `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="9fee0-309">Used to create an [absolute positioned](onenote-abs-pos.md) object, only if the object is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="9fee0-310">Пример: `<object style="position:absolute;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="9fee0-310">Example: `<object style="position:absolute;top:350px;left:300px" ... />`</span></span> |
| <span data-ttu-id="9fee0-311">шрифт</span><span class="sxs-lookup"><span data-stu-id="9fee0-311">type</span></span> | <span data-ttu-id="9fee0-312">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fee0-312">Required.</span></span><br/><br/><span data-ttu-id="9fee0-313">Стандартный тип файла мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="9fee0-313">The standard media file type.</span></span> <span data-ttu-id="9fee0-314">Для файлов известных типов на странице OneNote отображается значок, связанный с типом файла.</span><span class="sxs-lookup"><span data-stu-id="9fee0-314">Known file types display the icon associated with the file type on the OneNote page.</span></span> <span data-ttu-id="9fee0-315">Для файлов неизвестных типов отображается универсальный значок файла.</span><span class="sxs-lookup"><span data-stu-id="9fee0-315">Unknown file types display a generic file icon.</span></span> |
<!--todo: add link to known file types--> 

#### <a name="output-attributes"></a><span data-ttu-id="9fee0-316">Выходные атрибуты</span><span class="sxs-lookup"><span data-stu-id="9fee0-316">Output attributes</span></span>

|<span data-ttu-id="9fee0-317">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="9fee0-317">Output attribute</span></span>|<span data-ttu-id="9fee0-318">Описание</span><span class="sxs-lookup"><span data-stu-id="9fee0-318">Description</span></span>|
|:------|:------|
| <span data-ttu-id="9fee0-319">данные</span><span class="sxs-lookup"><span data-stu-id="9fee0-319">data</span></span> | <span data-ttu-id="9fee0-320">Конечная точка файлового ресурса.</span><span class="sxs-lookup"><span data-stu-id="9fee0-320">The endpoint for the file resource.</span></span> |
| <span data-ttu-id="9fee0-321">data-attachment</span><span class="sxs-lookup"><span data-stu-id="9fee0-321">data-attachment</span></span> | <span data-ttu-id="9fee0-322">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="9fee0-322">The file name.</span></span> |
| <span data-ttu-id="9fee0-323">data-id</span><span class="sxs-lookup"><span data-stu-id="9fee0-323">data-id</span></span> | <span data-ttu-id="9fee0-324">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="9fee0-324">A reference for the element.</span></span><br/><br/><span data-ttu-id="9fee0-325">Используется для [обновления содержимого страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-325">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="9fee0-326">идентификатор</span><span class="sxs-lookup"><span data-stu-id="9fee0-326">id</span></span> | <span data-ttu-id="9fee0-327">Уникальный сгенерированный ИД элемента.</span><span class="sxs-lookup"><span data-stu-id="9fee0-327">A unique, generated ID for the element.</span></span> <span data-ttu-id="9fee0-328">Возвращается [запросами GET к конечной точке *content* страницы](../api-reference/v1.0/api/page_get.md) при использовании параметра запроса `includeIDs=true`.</span><span class="sxs-lookup"><span data-stu-id="9fee0-328">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="9fee0-329">Используется для [обновления содержимого страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-329">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="9fee0-330">стиль</span><span class="sxs-lookup"><span data-stu-id="9fee0-330">style</span></span> | <span data-ttu-id="9fee0-331">Свойства позиции объекта.</span><span class="sxs-lookup"><span data-stu-id="9fee0-331">The position properties of the object.</span></span> |
| <span data-ttu-id="9fee0-332">шрифт</span><span class="sxs-lookup"><span data-stu-id="9fee0-332">type</span></span> | <span data-ttu-id="9fee0-333">Стандартный тип файла мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="9fee0-333">The standard media file type.</span></span> |
 

#### <a name="output-html-example-for-objects"></a><span data-ttu-id="9fee0-334">Пример выходных данных HTML для объектов</span><span class="sxs-lookup"><span data-stu-id="9fee0-334">Output HTML example for objects</span></span>

<span data-ttu-id="9fee0-335">Выходные элементы **object** содержат конечные точки, ссылающиеся на файловые ресурсы со страницы, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="9fee0-335">Output **object** elements contain endpoints that link to the file resources in the page, as shown.</span></span> <span data-ttu-id="9fee0-336">Вы можете отправлять отдельные [запросы GET к конечным точкам файловых ресурсов](../api-reference/v1.0/api/resource_get.md), чтобы получать их двоичное содержимое.</span><span class="sxs-lookup"><span data-stu-id="9fee0-336">You can make separate [GET requests to file resource endpoints](../api-reference/v1.0/api/resource_get.md) to retrieve their binary contents.</span></span>

```html
<object
    data="https://graph.microsoft.com/v1.0/me/onenote/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" 
    [style="..."] />
``` 

## <a name="paragraphs-and-headings"></a><span data-ttu-id="9fee0-337">Абзацы и заголовки</span><span class="sxs-lookup"><span data-stu-id="9fee0-337">Paragraphs and headings</span></span>

<span data-ttu-id="9fee0-338">Входной и выходной HTML-код для абзацев, заголовков и других текстовых контейнеров может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="9fee0-338">Paragraphs, headings, and other text containers can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="9fee0-339">Входные атрибуты</span><span class="sxs-lookup"><span data-stu-id="9fee0-339">Input attributes</span></span>

|<span data-ttu-id="9fee0-340">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="9fee0-340">Input attribute</span></span>|<span data-ttu-id="9fee0-341">Описание</span><span class="sxs-lookup"><span data-stu-id="9fee0-341">Description</span></span>|
|:------|:------|
| <span data-ttu-id="9fee0-342">data-id</span><span class="sxs-lookup"><span data-stu-id="9fee0-342">data-id</span></span> | <span data-ttu-id="9fee0-343">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="9fee0-343">A reference for the element.</span></span><br/><br/><span data-ttu-id="9fee0-344">Используется для [обновления содержимого страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-344">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="9fee0-345">data-tag</span><span class="sxs-lookup"><span data-stu-id="9fee0-345">data-tag</span></span> | <span data-ttu-id="9fee0-346">[Тег заметки](onenote-note-tags.md) для элемента **p** или **h1** - **h6**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-346">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="9fee0-347">стиль</span><span class="sxs-lookup"><span data-stu-id="9fee0-347">style</span></span> | <span data-ttu-id="9fee0-348">Свойства CSS [style](#styles) для элемента.</span><span class="sxs-lookup"><span data-stu-id="9fee0-348">The CSS [style](#styles) properties of the element.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="9fee0-349">Выходные атрибуты</span><span class="sxs-lookup"><span data-stu-id="9fee0-349">Output attributes</span></span>

|<span data-ttu-id="9fee0-350">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="9fee0-350">Output attribute</span></span>|<span data-ttu-id="9fee0-351">Описание</span><span class="sxs-lookup"><span data-stu-id="9fee0-351">Description</span></span>|
|:------|:------|
| <span data-ttu-id="9fee0-352">data-id</span><span class="sxs-lookup"><span data-stu-id="9fee0-352">data-id</span></span> | <span data-ttu-id="9fee0-353">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="9fee0-353">A reference for the element.</span></span><br/><br/><span data-ttu-id="9fee0-354">Используется для [обновления содержимого страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-354">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="9fee0-355">data-tag</span><span class="sxs-lookup"><span data-stu-id="9fee0-355">data-tag</span></span> | <span data-ttu-id="9fee0-356">[Тег заметки](onenote-note-tags.md) для элемента **p** или **h1** - **h6**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-356">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="9fee0-357">идентификатор</span><span class="sxs-lookup"><span data-stu-id="9fee0-357">id</span></span> | <span data-ttu-id="9fee0-358">Уникальный сгенерированный ИД элемента.</span><span class="sxs-lookup"><span data-stu-id="9fee0-358">A unique, generated ID for the element.</span></span> <span data-ttu-id="9fee0-359">Возвращается [запросами GET к конечной точке *content* страницы](../api-reference/v1.0/api/page_get.md) при использовании параметра запроса `includeIDs=true`.</span><span class="sxs-lookup"><span data-stu-id="9fee0-359">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="9fee0-360">Используется для [обновления содержимого страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-360">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="9fee0-361">стиль</span><span class="sxs-lookup"><span data-stu-id="9fee0-361">style</span></span> | <span data-ttu-id="9fee0-362">Свойства CSS [style](#styles) для элемента.</span><span class="sxs-lookup"><span data-stu-id="9fee0-362">The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="9fee0-363">В выходном HTML-коде эти значения могут быть встроены в элементы **span** или соответствующие дочерние элементы.</span><span class="sxs-lookup"><span data-stu-id="9fee0-363">In the output HTML, these values may be returned inline on appropriate child elements or on **span** elements.</span></span> |
 

<span data-ttu-id="9fee0-364">В приведенных ниже примерах показан входной HTML-код, где используются разные способы определения стилей в текстовых контейнерах, и возвращаемый выходной HTML-код.</span><span class="sxs-lookup"><span data-stu-id="9fee0-364">The following examples show input HTML that uses different ways to define styles on text containers and the output HTML that's returned.</span></span>

#### <a name="input-html-with-styles-defined-using-inline-character-styles-in-the-start-tag-and-within-a-span-element"></a><span data-ttu-id="9fee0-365">Входной HTML-код со стилями, определенными с помощью встроенных стилей знаков, в начальном теге внутри элемента span.</span><span class="sxs-lookup"><span data-stu-id="9fee0-365">Input HTML with styles defined using inline character styles, in the start tag, and within a span element.</span></span>

```html
<h1>Heading <i>One</i> text</h1>
<p style="font-size:8pt;color:green;font-family:Courier;text-align:center">Some text</p>
<p>Some <span  style="font-size:16px;color:#ff0000;font-family:Segoe UI Black">more</span> text</p>
``` 

#### <a name="output-html-with-the-i-character-style-and-the-font-settings-in-the-p-start-tag-returned-as-inline-css-styles-on-span-elements"></a><span data-ttu-id="9fee0-366">Выходной HTML-код со стилем знака `<i>` и параметрами шрифта в начальном теге `<p>`, возвращаемыми в виде встроенных стилей CSS в элементах span.</span><span class="sxs-lookup"><span data-stu-id="9fee0-366">Output HTML with the `<i>` character style and the font settings in the `<p>` start tag returned as inline CSS styles on span elements.</span></span>

```html
<h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">Heading <span style="font-style:italic">One</span> text</h1>
<p style="text-align:center"><span style="font-family:Courier;font-size:8pt;color:green">Some text</span></p>
<p>Some <span style="font-family:Segoe UI Black;font-size:12pt;color:red">more</span> text</p>
``` 


## <a name="lists"></a><span data-ttu-id="9fee0-367">Списки</span><span class="sxs-lookup"><span data-stu-id="9fee0-367">Lists</span></span>

<span data-ttu-id="9fee0-368">Для представления списков используются элементы **ol** или **ul**, которые содержат элементы списка, представленные элементами **li**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-368">Lists are represented as **ol** or **ul** elements that contain list items represented as **li** elements.</span></span>

<span data-ttu-id="9fee0-369">Входной и выходной HTML-код списков и их элементов может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="9fee0-369">Lists and list items can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="9fee0-370">Входные атрибуты</span><span class="sxs-lookup"><span data-stu-id="9fee0-370">Input attributes</span></span>

|<span data-ttu-id="9fee0-371">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="9fee0-371">Input attribute</span></span>|<span data-ttu-id="9fee0-372">Описание</span><span class="sxs-lookup"><span data-stu-id="9fee0-372">Description</span></span>|
|:------|:------|
| <span data-ttu-id="9fee0-373">data-id</span><span class="sxs-lookup"><span data-stu-id="9fee0-373">data-id</span></span> | <span data-ttu-id="9fee0-374">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="9fee0-374">A reference for the element.</span></span><br/><br/><span data-ttu-id="9fee0-375">Используется для [обновления содержимого страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-375">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="9fee0-376">data-tag</span><span class="sxs-lookup"><span data-stu-id="9fee0-376">data-tag</span></span> | <span data-ttu-id="9fee0-377">[Тег заметки](onenote-note-tags.md) в элементе **ul**, **ol** или **li**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-377">A [note tag](onenote-note-tags.md) on a **ul**, **ol**, or **li** element.</span></span> |
| <span data-ttu-id="9fee0-378">стиль</span><span class="sxs-lookup"><span data-stu-id="9fee0-378">style</span></span> | <span data-ttu-id="9fee0-379">Свойство **list-style-type** и свойство CSS [style](#styles) для списка или его элемента.</span><span class="sxs-lookup"><span data-stu-id="9fee0-379">The **list-style-type** and the CSS [style](#styles) properties for the list or list item.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="9fee0-380">Выходные атрибуты</span><span class="sxs-lookup"><span data-stu-id="9fee0-380">Output attributes</span></span>

|<span data-ttu-id="9fee0-381">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="9fee0-381">Output attribute</span></span>|<span data-ttu-id="9fee0-382">Описание</span><span class="sxs-lookup"><span data-stu-id="9fee0-382">Description</span></span>|
|:------|:------|
| <span data-ttu-id="9fee0-383">data-id</span><span class="sxs-lookup"><span data-stu-id="9fee0-383">data-id</span></span> | <span data-ttu-id="9fee0-384">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="9fee0-384">A reference for the element.</span></span><br/><br/><span data-ttu-id="9fee0-385">Используется для [обновления содержимого страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-385">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="9fee0-386">data-tag</span><span class="sxs-lookup"><span data-stu-id="9fee0-386">data-tag</span></span> |  <span data-ttu-id="9fee0-387">[Тег заметки](onenote-note-tags.md) в элементе span внутри элемента **li**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-387">A [note tag](onenote-note-tags.md) on a span in a **li** element.</span></span> |
| <span data-ttu-id="9fee0-388">идентификатор</span><span class="sxs-lookup"><span data-stu-id="9fee0-388">id</span></span> | <span data-ttu-id="9fee0-389">Уникальный сгенерированный ИД элемента.</span><span class="sxs-lookup"><span data-stu-id="9fee0-389">A unique, generated ID for the element.</span></span> <span data-ttu-id="9fee0-390">Возвращается [запросами GET к конечной точке *content* страницы](../api-reference/v1.0/api/page_get.md) при использовании параметра запроса `includeIDs=true`.</span><span class="sxs-lookup"><span data-stu-id="9fee0-390">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="9fee0-391">Используется для [обновления содержимого страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-391">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="9fee0-392">стиль</span><span class="sxs-lookup"><span data-stu-id="9fee0-392">style</span></span> | <span data-ttu-id="9fee0-393">Свойство **list-style-type** и свойство CSS [style](#styles) для элемента.</span><span class="sxs-lookup"><span data-stu-id="9fee0-393">The **list-style-type** and CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="9fee0-394">В выходном HTML-коде параметры на уровне списка возвращаются в элементах списка.</span><span class="sxs-lookup"><span data-stu-id="9fee0-394">In the output HTML, list-level settings are returned on list items.</span></span> <span data-ttu-id="9fee0-395">Свойства по умолчанию не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="9fee0-395">Default properties are not returned.</span></span> |
 
### <a name="list-styles"></a><span data-ttu-id="9fee0-396">Стили списков</span><span class="sxs-lookup"><span data-stu-id="9fee0-396">List styles</span></span>

<span data-ttu-id="9fee0-397">API OneNote в Microsoft Graph поддерживают следующие стили списков:</span><span class="sxs-lookup"><span data-stu-id="9fee0-397">The OneNote APIs in Microsoft Graph support the following list styles:</span></span>

|<span data-ttu-id="9fee0-398">Упорядоченный список</span><span class="sxs-lookup"><span data-stu-id="9fee0-398">Ordered list</span></span>|<span data-ttu-id="9fee0-399">Неупорядоченный список</span><span class="sxs-lookup"><span data-stu-id="9fee0-399">Unordered list</span></span>|
|:------|:------|
| <span data-ttu-id="9fee0-400">отсутствует</span><span class="sxs-lookup"><span data-stu-id="9fee0-400">none</span></span> | <span data-ttu-id="9fee0-401">отсутствует</span><span class="sxs-lookup"><span data-stu-id="9fee0-401">none</span></span> |
| <span data-ttu-id="9fee0-402">decimal (по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="9fee0-402">decimal (default)</span></span> | <span data-ttu-id="9fee0-403">disc (по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="9fee0-403">disc (default)</span></span> |
| <span data-ttu-id="9fee0-404">lower-alpha</span><span class="sxs-lookup"><span data-stu-id="9fee0-404">lower-alpha</span></span> | <span data-ttu-id="9fee0-405">circle</span><span class="sxs-lookup"><span data-stu-id="9fee0-405">circle</span></span> |
| <span data-ttu-id="9fee0-406">lower-roman</span><span class="sxs-lookup"><span data-stu-id="9fee0-406">lower-roman</span></span> | <span data-ttu-id="9fee0-407">square</span><span class="sxs-lookup"><span data-stu-id="9fee0-407">square</span></span> |
| <span data-ttu-id="9fee0-408">upper-alpha</span><span class="sxs-lookup"><span data-stu-id="9fee0-408">upper-alpha</span></span> | &nbsp; |
| <span data-ttu-id="9fee0-409">upper-roman</span><span class="sxs-lookup"><span data-stu-id="9fee0-409">upper-roman</span></span> | &nbsp; |
 
<span data-ttu-id="9fee0-410">Вы можете применять глобальные стили для списка в элементе **ol** или **ul** входных данных HTML, но стили возвращаются в элементах **li**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-410">You can apply global styles for a list on the **ol** or **ul** element in the input HTML, but styles are returned on the **li** elements.</span></span>

#### <a name="homogenous-list-style"></a><span data-ttu-id="9fee0-411">Однородный стиль списка</span><span class="sxs-lookup"><span data-stu-id="9fee0-411">Homogenous list style</span></span>

<span data-ttu-id="9fee0-412">В этом примере показан входной HTML-код, который задает тип стиля списка в элементе **ol** и стили CSS для отдельных элементов списка.</span><span class="sxs-lookup"><span data-stu-id="9fee0-412">This example shows input HTML that sets the list style type on the **ol** element and CSS styles on individual list items.</span></span>

```html
<ol style="list-style-type:upper-roman;color:blue">
    <li style="font-weight:bold">Jacksonville</li>
    <li style="text-decoration:line-through">Orlando</li>
    <li style="font-family:Courier">Naples</li>
</ol>
``` 

<span data-ttu-id="9fee0-p138">Ниже приводятся выходные данные HTML. Обратите внимание, что стили возвращаются встроенными в отдельные элементы **li** или **span**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-p138">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ol>
    <li style="list-style-type:upper-roman"><span style="color:blue;font-weight:bold">Jacksonville</span></li>
    <li style="list-style-type:upper-roman"><span style="color:blue;text-decoration:line-through">Orlando</span></li>
    <li style="list-style-type:upper-roman"><span style="font-family:Courier;color:blue">Naples</span></li>
</ol>
``` 

#### <a name="variable-list-styles"></a><span data-ttu-id="9fee0-415">Переменные стили списков</span><span class="sxs-lookup"><span data-stu-id="9fee0-415">Variable list styles</span></span>

<span data-ttu-id="9fee0-416">В этом примере показан входной HTML-код, который задает разные типы стилей списков в элементах **li**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-416">This example shows input HTML that sets different list style types on the **li** elements.</span></span>

```html
<ul style="font-style:italic">
    <li style="list-style-type:square">square style</li>
    <li style="list-style-type:circle">circle style</li>
    <li style="list-style-type:disc">disc style (default)</li>
</ul>
``` 

<span data-ttu-id="9fee0-p139">Ниже приводятся выходные данные HTML. Обратите внимание, что стили возвращаются встроенными в отдельные элементы **li** или **span**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-p139">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ul>
    <li style="list-style-type:square"><span style="font-style:italic">square style</span></li>
    <li style="list-style-type:circle"><span style="font-style:italic">circle style</span></li>
    <li><span style="font-style:italic">disc style (default)</span></li>
</ul>
``` 


## <a name="tables"></a><span data-ttu-id="9fee0-419">Таблицы</span><span class="sxs-lookup"><span data-stu-id="9fee0-419">Tables</span></span>

<span data-ttu-id="9fee0-p140">Таблицы представляются как элементы **table**, которые могут содержать элементы **tr** и **td**. Поддерживаются вложенные таблицы.</span><span class="sxs-lookup"><span data-stu-id="9fee0-p140">Tables are represented as **table** elements that can contain **tr** and **td** elements. Nested tables are supported.</span></span>

<span data-ttu-id="9fee0-422">Входной и выходной HTML-код для таблиц может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="9fee0-422">Tables can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="9fee0-423">API OneNote не поддерживают атрибуты **rowspan** и **colspan**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-423">The OneNote APIs do not support **rowspan** or **colspan** attributes.</span></span> 

#### <a name="input-attributes"></a><span data-ttu-id="9fee0-424">Входные атрибуты</span><span class="sxs-lookup"><span data-stu-id="9fee0-424">Input attributes</span></span>

|<span data-ttu-id="9fee0-425">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="9fee0-425">Input attribute</span></span>|<span data-ttu-id="9fee0-426">Описание</span><span class="sxs-lookup"><span data-stu-id="9fee0-426">Description</span></span>|
|:------|:------|
| <span data-ttu-id="9fee0-427">data-id</span><span class="sxs-lookup"><span data-stu-id="9fee0-427">data-id</span></span> | <span data-ttu-id="9fee0-428">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="9fee0-428">A reference for the element.</span></span><br/><br/><span data-ttu-id="9fee0-429">Используется для [обновления содержимого страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-429">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="9fee0-430">стиль</span><span class="sxs-lookup"><span data-stu-id="9fee0-430">style</span></span> | <span data-ttu-id="9fee0-431">Свойства CSS [style](#styles) для элемента, а также:</span><span class="sxs-lookup"><span data-stu-id="9fee0-431">The CSS [style](#styles) properties of the element, and also:</span></span><br/> <span data-ttu-id="9fee0-432">- **border**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-432">- **border**.</span></span> <span data-ttu-id="9fee0-433">Допустимые значения — 0px и 1px.</span><span class="sxs-lookup"><span data-stu-id="9fee0-433">Can be either 0px or 1px.</span></span><br/> <span data-ttu-id="9fee0-434">- **width**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-434">- **width**.</span></span> <span data-ttu-id="9fee0-435">Поддерживается в элементах **table** и **td** как количество пикселей или процент от ширины страницы.</span><span class="sxs-lookup"><span data-stu-id="9fee0-435">Supported by **table** and **td** as pixels or percentage of page width.</span></span><br/><br/><span data-ttu-id="9fee0-436">Пример: `width="100px"` или `width="60%"`</span><span class="sxs-lookup"><span data-stu-id="9fee0-436">Example: `width="100px"` or `width="60%"`</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="9fee0-437">Выходные атрибуты</span><span class="sxs-lookup"><span data-stu-id="9fee0-437">Output attributes</span></span>

|<span data-ttu-id="9fee0-438">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="9fee0-438">Output attribute</span></span>|<span data-ttu-id="9fee0-439">Описание</span><span class="sxs-lookup"><span data-stu-id="9fee0-439">Description</span></span>|
|:------|:------|
| <span data-ttu-id="9fee0-440">data-id</span><span class="sxs-lookup"><span data-stu-id="9fee0-440">data-id</span></span> | <span data-ttu-id="9fee0-441">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="9fee0-441">A reference for the element.</span></span><br/><br/><span data-ttu-id="9fee0-442">Используется для [обновления содержимого страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-442">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="9fee0-443">идентификатор</span><span class="sxs-lookup"><span data-stu-id="9fee0-443">id</span></span> | <span data-ttu-id="9fee0-444">Уникальный сгенерированный ИД элемента.</span><span class="sxs-lookup"><span data-stu-id="9fee0-444">A unique, generated ID for the element.</span></span> <span data-ttu-id="9fee0-445">Возвращается [запросами GET к конечной точке *content* страницы](../api-reference/v1.0/api/page_get.md) при использовании параметра запроса `includeIDs=true`.</span><span class="sxs-lookup"><span data-stu-id="9fee0-445">Returned by [GET requests to a page's *content* endpoint](../api-reference/v1.0/api/page_get.md) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="9fee0-446">Используется для [обновления содержимого страницы](onenote_update_page.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-446">Used to [update page content](onenote_update_page.md).</span></span> |
| <span data-ttu-id="9fee0-447">стиль</span><span class="sxs-lookup"><span data-stu-id="9fee0-447">style</span></span> | <span data-ttu-id="9fee0-448">Свойства CSS [style](#styles) для элемента.</span><span class="sxs-lookup"><span data-stu-id="9fee0-448">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="9fee0-449">В приведенных ниже примерах показан входной HTML-код, где используются разные способы определения стилей для таблиц, и возвращаемый выходной HTML-код.</span><span class="sxs-lookup"><span data-stu-id="9fee0-449">The following examples show input HTML that uses different ways to define styles on tables and the output HTML that's returned.</span></span>

#### <a name="input-html-with-optional-settings-at-different-levels"></a><span data-ttu-id="9fee0-450">Входной HTML-код с необязательными параметрами на разных уровнях</span><span class="sxs-lookup"><span data-stu-id="9fee0-450">Input HTML with optional settings at different levels.</span></span>

```html
<table style="border:0px;width:500px;background-color:green">
    <tr> 
        <td>Cell 1</td> 
        <td>Cell 2</td> 
        <td>Cell 3</td> 
    </tr> 
    <tr style="background-color:blue"> 
        <td style="text-align:right;background-color:red">Left</td> 
        <td style="text-align:center">Middle</td> 
        <td>Right</td> 
    </tr> 
</table>
```
 
#### <a name="output-html-with-css-styles-returned-inline-on-the-td-elements"></a><span data-ttu-id="9fee0-451">Выходной HTML-код со стилями CSS, которые возвращаются встроенными в элементы td</span><span class="sxs-lookup"><span data-stu-id="9fee0-451">Output HTML with CSS styles returned inline on the td elements.</span></span>

```html
<table style="border:0px">
    <tr>
        <td style="background-color:green;width:166;border:0px">Cell 1</td>
        <td style="background-color:green;width:166;border:0px">Cell 2</td>
        <td style="background-color:green;width:166;border:0px">Cell 3</td>
    </tr>
    <tr>
        <td style="background-color:red;width:166;border:0px;text-align:right">Left</td>
        <td style="background-color:blue;width:166;border:0px;text-align:center">Middle</td>
        <td style="background-color:blue;width:166;border:0px">Right</td>
    </tr>
</table>
``` 


## <a name="styles"></a><span data-ttu-id="9fee0-452">Стили</span><span class="sxs-lookup"><span data-stu-id="9fee0-452">Styles</span></span>

<span data-ttu-id="9fee0-453">API OneNote в Microsoft Graph поддерживают перечисленные ниже встроенные свойства CSS **style** для элементов основного текста страницы, например **body**, **div**, **p**, **li** и **span**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-453">OneNote APIs in Microsoft Graph support the following inline CSS **style** properties for elements in the page body, such as **body**, **div**, **p**, **li**, and **span**.</span></span>

|<span data-ttu-id="9fee0-454">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fee0-454">Property</span></span>|<span data-ttu-id="9fee0-455">Пример</span><span class="sxs-lookup"><span data-stu-id="9fee0-455">Example</span></span>|
|:------|:------|
| <span data-ttu-id="9fee0-456">background-color (цвет фона)</span><span class="sxs-lookup"><span data-stu-id="9fee0-456">background-color</span></span> | <span data-ttu-id="9fee0-457">`style="background-color:#66cc66"` (по умолчанию задан белый цвет)</span><span class="sxs-lookup"><span data-stu-id="9fee0-457">`style="background-color:#66cc66"` (defaults to white)</span></span><br/><br/><span data-ttu-id="9fee0-458">Поддерживаются как шестнадцатеричный формат, так и именованные цвета.</span><span class="sxs-lookup"><span data-stu-id="9fee0-458">Both hexadecimal format and named colors are supported.</span></span> |
| <span data-ttu-id="9fee0-459">color (цвет)</span><span class="sxs-lookup"><span data-stu-id="9fee0-459">color</span></span> | <span data-ttu-id="9fee0-460">`style="color:#ffffff"` (по умолчанию задан черный цвет)</span><span class="sxs-lookup"><span data-stu-id="9fee0-460">`style="color:#ffffff"` (defaults to black)</span></span> |
| <span data-ttu-id="9fee0-461">font-family (семейство шрифтов)</span><span class="sxs-lookup"><span data-stu-id="9fee0-461">font-family</span></span> | <span data-ttu-id="9fee0-462">`style="font-family:Courier"` (по умолчанию задан шрифт Calibri)</span><span class="sxs-lookup"><span data-stu-id="9fee0-462">`style="font-family:Courier"` (defaults to Calibri)</span></span> |
| <span data-ttu-id="9fee0-463">font-size (размер шрифта)</span><span class="sxs-lookup"><span data-stu-id="9fee0-463">font-size</span></span> | <span data-ttu-id="9fee0-464">`style="font-size:10pt"` (по умолчанию задан размер 11 точек)</span><span class="sxs-lookup"><span data-stu-id="9fee0-464">`style="font-size:10pt"` (defaults to 11pt)</span></span><br/><br/><span data-ttu-id="9fee0-465">API принимают размер шрифта в единицах *pt* или *px*, но единицы *px* преобразуются в *pt*.</span><span class="sxs-lookup"><span data-stu-id="9fee0-465">The APIs accept font size in *pt* or *px*, but converts *px* to *pt*.</span></span> <span data-ttu-id="9fee0-466">Десятичные значения округляются до ближайшего значения n,0 или n,5 точек.</span><span class="sxs-lookup"><span data-stu-id="9fee0-466">Decimal values are rounded to the nearest n.0pt or n.5pt.</span></span> |
| <span data-ttu-id="9fee0-467">font-style (стиль шрифта)</span><span class="sxs-lookup"><span data-stu-id="9fee0-467">font-style</span></span> | <span data-ttu-id="9fee0-468">`style="font-style:italic"` (обычный или только курсив)</span><span class="sxs-lookup"><span data-stu-id="9fee0-468">`style="font-style:italic"` (normal or italic only)</span></span> |
| <span data-ttu-id="9fee0-469">font-weight (толщина шрифта)</span><span class="sxs-lookup"><span data-stu-id="9fee0-469">font-weight</span></span> | <span data-ttu-id="9fee0-470">`style="font-weight:bold"` (обычный или только полужирный)</span><span class="sxs-lookup"><span data-stu-id="9fee0-470">`style="font-weight:bold"` (normal or bold only)</span></span> |
| <span data-ttu-id="9fee0-471">strike-through (зачеркнутый)</span><span class="sxs-lookup"><span data-stu-id="9fee0-471">strike-through</span></span> | `style="text-decoration:line-through"` |
| <span data-ttu-id="9fee0-472">text-align (выравнивание текста)</span><span class="sxs-lookup"><span data-stu-id="9fee0-472">text-align</span></span> | <span data-ttu-id="9fee0-473">`style="text-align:center"` (только для блочных элементов)</span><span class="sxs-lookup"><span data-stu-id="9fee0-473">`style="text-align:center"` (for block elements only)</span></span> |
| <span data-ttu-id="9fee0-474">text-decoration (оформление текста)</span><span class="sxs-lookup"><span data-stu-id="9fee0-474">text-decoration</span></span> | <span data-ttu-id="9fee0-475">`style="text-decoration:underline"` (без оформления или только подчеркивание)</span><span class="sxs-lookup"><span data-stu-id="9fee0-475">`style="text-decoration:underline"` (none or underline only)</span></span> |
 

<span data-ttu-id="9fee0-476">Кроме того, поддерживаются следующие встроенные стили знаков:</span><span class="sxs-lookup"><span data-stu-id="9fee0-476">The following inline character styles and are also supported:</span></span>

<table id="simpletable">
<tr>
<td id="simplecell"><span data-ttu-id="9fee0-477">&lt;b&gt;</span><span class="sxs-lookup"><span data-stu-id="9fee0-477">&lt;b&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="9fee0-478">&lt;i&gt;</span><span class="sxs-lookup"><span data-stu-id="9fee0-478">&lt;i&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="9fee0-479">&lt;u&gt;</span><span class="sxs-lookup"><span data-stu-id="9fee0-479">&lt;u&gt;</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="9fee0-480">&lt;em&gt;</span><span class="sxs-lookup"><span data-stu-id="9fee0-480">&lt;em&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="9fee0-481">&lt;strong&gt;</span><span class="sxs-lookup"><span data-stu-id="9fee0-481">&lt;strong&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="9fee0-482">&lt;strike&gt;</span><span class="sxs-lookup"><span data-stu-id="9fee0-482">&lt;strike&gt;</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="9fee0-483">&lt;sup&gt;</span><span class="sxs-lookup"><span data-stu-id="9fee0-483">&lt;sup&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="9fee0-484">&lt;sub&gt;</span><span class="sxs-lookup"><span data-stu-id="9fee0-484">&lt;sub&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="9fee0-485">&lt;del&gt;</span><span class="sxs-lookup"><span data-stu-id="9fee0-485">&lt;del&gt;</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="9fee0-486">&lt;cite&gt;</span><span class="sxs-lookup"><span data-stu-id="9fee0-486">&lt;cite&gt;</span></span></td>
<td id="simplecell">&nbsp;</td>
<td id="simplecell">&nbsp;</td>
</tr>
</table>

 
## <a name="input-and-output-html-example"></a><span data-ttu-id="9fee0-487">Пример входного и выходного HTML-кода</span><span class="sxs-lookup"><span data-stu-id="9fee0-487">Input and output HTML example</span></span>

<span data-ttu-id="9fee0-488">На приведенном ниже рисунке показана простая страница, созданная с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9fee0-488">The following image shows a simple page that was created with Microsoft Graph.</span></span>

![Изображение страницы OneNote с учебными заметками по материалам из Википедии](images/onenote-sample-image.png)

<span data-ttu-id="9fee0-490">Ниже показан входной HTML-код, отправляемый в тексте сообщения для создания страницы.</span><span class="sxs-lookup"><span data-stu-id="9fee0-490">This is the input HTML sent in the message body to create the page.</span></span>

```html
<html lang="en-US">
    <head>
        <title>Sample Study Notes</title>
        <meta name="created" content="2015-01-01T01:01"/>
    </head>
    <body>
        <h1>Aurora Borealis</h1>
        <p>Dancing lights in the sky. Also called <i>Northern Lights</i>. Caused by solar radiation.</p>
        <br />
        <p><b>Intersting facts</b></p>
        <table>
            <tr>
                <td>Neil Armstrong</td>
                <td>Commander</td>
            </tr>
            <tr>
                <td>Buzz Aldrin</td>
                <td>LM Pilot</td>
            </tr>
            <tr>
                <td>Michael Collins</td>
                <td>Command Module Pilot</td>
            </tr>
        </table>
        <img alt="Apollo 11 commemorative stamp." src="http://upload.wikimedia.org/wikipedia/commons/a/a4/First_Man_on_Moon_1969_Issue-10c.jpg"  width="400"/>
        <p>References:</p>
        <p><a href="http://en.wikipedia.org/wiki/Apollo_11">http://en.wikipedia.org/wiki/Apollo_11</a></p>
        <p><a href="http://www.nasa.gov/mission_pages/apollo/missions/apollo11.html">http://www.nasa.gov/mission_pages/apollo/missions/apollo11.html</a></p>
    </body>
</html>
``` 

<br/>

<span data-ttu-id="9fee0-491">Ниже показан выходной HTML-код, который Microsoft Graph возвращает при [получении содержимого страницы](onenote-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="9fee0-491">This is the output HTML that Microsoft Graph returns when you [get page content](onenote-get-content.md).</span></span>

> <span data-ttu-id="9fee0-492">**Примечание.** При [создании страницы](onenote-create-page.md) или [получении метаданных страницы](../api-reference/v1.0/api/page_get.md) API возвращает URL-адрес конечной точки *content* для страницы в свойстве **contentUrl**.</span><span class="sxs-lookup"><span data-stu-id="9fee0-492">**Note:** When you [create a page](onenote-create-page.md) or [get page metadata](../api-reference/v1.0/api/page_get.md), the API returns the *content* endpoint URL of the page in the **contentUrl** property.</span></span>

```html
<html htmlns="http://www.w3.org/1999/xhtml" lang="en-US">
    <head>
        <title>Sample Study Notes</title>
    </head>
    <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11pt">
        <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
            <h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">American History 101: Moon Landing</h1>
            <p>First moon landing - July 20, 1969 with Apollo 11 (Eagle)</p>
            <br />
            <p><span style="font-weight:bold">Apollo 11 Astronauts</span></p>
            <table style="border:0px">
                <tr>
                    <td style="border:0px">Neil Armstrong</td>
                    <td style="border:0px">Commander</td>
                </tr>
                <tr>
                    <td style="border:0px">Buzz Aldrin</td>
                    <td style="border:0px">LM Pilot</td>
                </tr>
                <tr>
                    <td style="border:0px">Michael Collins</td>
                    <td style="border:0px">Command Module Pilot</td>
                </tr>
            </table>
            <br />
            <img alt="Apollo 11 commemorative stamp." width="400" height="248" src="https://graph.microsoft.com/v1.0/me/onenote/resources/0-f717b5fa5eaa454da7ecdf72a8c137fe!1-73DBAF9B7E5C4B4C!10456/$value"
                 data-src-type="image/jpeg" data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/0-f717b5fa5eaa454da7ecdf72a8c137fe!1-73DBAF9B7E5C4B4C!10456/$value" data-fullres-src-type="image/jpeg" />
            <p>References:</p>
            <p><a href="http://en.wikipedia.org/wiki/Apollo_11">http://en.wikipedia.org/wiki/Apollo_11</a></p>
            <p><a href="http://www.nasa.gov/mission_pages/apollo/missions/apollo11.html">http://www.nasa.gov/mission_pages/apollo/missions/apollo11.html</a></p>
        </div>
    </body>
</html>
``` 

## <a name="see-also"></a><span data-ttu-id="9fee0-493">См. также</span><span class="sxs-lookup"><span data-stu-id="9fee0-493">See also</span></span>

- [<span data-ttu-id="9fee0-494">Получение содержимого и структуры OneNote</span><span class="sxs-lookup"><span data-stu-id="9fee0-494">Get OneNote content and structure</span></span>](onenote-get-content.md)
- [<span data-ttu-id="9fee0-495">Создание страниц OneNote</span><span class="sxs-lookup"><span data-stu-id="9fee0-495">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="9fee0-496">Обновление содержимого страницы OneNote</span><span class="sxs-lookup"><span data-stu-id="9fee0-496">Update OneNote page content</span></span>](onenote_update_page.md)
- [<span data-ttu-id="9fee0-497">Добавление изображений, видео и файлов</span><span class="sxs-lookup"><span data-stu-id="9fee0-497">Add images, videos, and files</span></span>](onenote_images_files.md)
