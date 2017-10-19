# <a name="input-and-output-html-in-onenote-pages"></a><span data-ttu-id="06c71-101">Входной и выходной HTML-код на страницах OneNote</span><span class="sxs-lookup"><span data-stu-id="06c71-101">Input and output HTML for OneNote pages</span></span>

<span data-ttu-id="06c71-102">HTML-код, определяющий содержимое и структуру страницы при [создании](../api-reference/v1.0/api/section_post_pages.md) или [обновлении](../api-reference/v1.0/api/page_update.md) страницы OneNote, называется *входным HTML-кодом*.</span><span class="sxs-lookup"><span data-stu-id="06c71-102">The HTML that defines the page content and structure when you [create](../api-reference/v1.0/api/section_post_pages.md) or [update](../api-reference/v1.0/api/page_update.md) a OneNote page is called *input HTML*.</span></span> 

<span data-ttu-id="06c71-103">HTML-код, возвращаемый при [получении содержимого страницы](../api-reference/v1.0/api/page_get.md), называется *выходным HTML-кодом*.</span><span class="sxs-lookup"><span data-stu-id="06c71-103">The HTML that's returned when you [get page content](../api-reference/v1.0/api/page_get.md) is called *output HTML*.</span></span> <span data-ttu-id="06c71-104">Выходной HTML-код не совпадает со входным.</span><span class="sxs-lookup"><span data-stu-id="06c71-104">Output HTML won't be the same as input HTML.</span></span>

<span data-ttu-id="06c71-105">API OneNote в Microsoft Graph сохраняют семантическое содержимое и базовую структуру входного HTML-кода, но преобразовывают ее в набор [поддерживаемых элементов HTML и свойств CSS](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-create-page#supported-html).</span><span class="sxs-lookup"><span data-stu-id="06c71-105">The OneNote APIs in Microsoft Graph preserve the semantic content and basic structure of the input HTML, but convert it to a set of [supported HTML elements and CSS properties](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-create-page#supported-html).</span></span> <span data-ttu-id="06c71-106">API также добавляют настраиваемые атрибуты, поддерживающие функции OneNote.</span><span class="sxs-lookup"><span data-stu-id="06c71-106">The APIs also add custom attributes that support OneNote features.</span></span>
 
<span data-ttu-id="06c71-107">В этой статье описываются основные элементы и атрибуты входного и выходного HTML-кода.</span><span class="sxs-lookup"><span data-stu-id="06c71-107">This article describes the principal elements and attributes of input and output HTML.</span></span> <span data-ttu-id="06c71-108">Разбираться во входном HTML-коде полезно при создании и обновлении содержимого страницы, а в выходном — при анализе возвращаемого содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="06c71-108">It can be helpful to understand input HTML when you're creating or updating page content, and output HTML when you're parsing returned page content.</span></span> 

## <a name="body-element"></a><span data-ttu-id="06c71-109">Элемент Body</span><span class="sxs-lookup"><span data-stu-id="06c71-109">Body element</span></span>
<span data-ttu-id="06c71-110">HTML-содержимое в тексте страницы представляет ее содержимое и структуру, в том числе ресурсы изображений и файлов.</span><span class="sxs-lookup"><span data-stu-id="06c71-110">The HTML content in the page body represents  the page content and structure, including image and file resources. The body element can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="06c71-111">Входной и выходной HTML-код для элемента **body** может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="06c71-111">Lists and list items can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="06c71-112">**Входные атрибуты**</span><span class="sxs-lookup"><span data-stu-id="06c71-112">**Input attributes**</span></span>

|<span data-ttu-id="06c71-113">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="06c71-113">Input attribute</span></span>|<span data-ttu-id="06c71-114">Описание</span><span class="sxs-lookup"><span data-stu-id="06c71-114">Description</span></span>|
|:------|:------|
| <span data-ttu-id="06c71-115">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="06c71-115">data-absolute-enabled</span></span> | <span data-ttu-id="06c71-116">Указывает, поддерживают ли во входном тексте элементы с [абсолютным положением](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos).</span><span class="sxs-lookup"><span data-stu-id="06c71-116">Indicates whether the input body supports [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) elements.</span></span> |
| <span data-ttu-id="06c71-117">style</span><span class="sxs-lookup"><span data-stu-id="06c71-117">style</span></span> | <p><span data-ttu-id="06c71-118">Свойства CSS [style](#styles) для основного текста.</span><span class="sxs-lookup"><span data-stu-id="06c71-118">The CSS [style](#styles) properties of the body.</span></span> <span data-ttu-id="06c71-119">В выходном HTML-коде входные параметры могут быть встроены в соответствующие дочерние элементы.</span><span class="sxs-lookup"><span data-stu-id="06c71-119">In the output HTML, input settings might be returned inline on appropriate child elements.</span></span></p><p><span data-ttu-id="06c71-120">В настоящее время цвет фона не поддерживается для элемента **body**.</span><span class="sxs-lookup"><span data-stu-id="06c71-120">Background color is not currently supported for the **body** element.</span></span></p> |
 

<span data-ttu-id="06c71-121">**Выходные атрибуты**</span><span class="sxs-lookup"><span data-stu-id="06c71-121">**Output attributes**</span></span>

|<span data-ttu-id="06c71-122">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="06c71-122">Output attribute</span></span>|<span data-ttu-id="06c71-123">Описание</span><span class="sxs-lookup"><span data-stu-id="06c71-123">Description</span></span>|
|:------|:------|
| <span data-ttu-id="06c71-124">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="06c71-124">data-absolute-enabled</span></span> | <span data-ttu-id="06c71-125">Указывает, поддерживаются ли в тексте элементы с [абсолютным положением](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos).</span><span class="sxs-lookup"><span data-stu-id="06c71-125">Indicates whether the body supports absolutely positioned elements. Always true in output HTML.</span></span> <span data-ttu-id="06c71-126">В выходном HTML-коде всегда задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="06c71-126">Always **true** in output HTML.</span></span> |
| <span data-ttu-id="06c71-127">style</span><span class="sxs-lookup"><span data-stu-id="06c71-127">style</span></span> | <span data-ttu-id="06c71-128">Свойства **font-family** и **font-size** основного текста.</span><span class="sxs-lookup"><span data-stu-id="06c71-128">The **font-family** and **font-size** properties of the body.</span></span> |


## <a name="div-elements"></a><span data-ttu-id="06c71-129">Элементы Div</span><span class="sxs-lookup"><span data-stu-id="06c71-129">Div elements</span></span>
<span data-ttu-id="06c71-130">Элементы **Div** содержат текст, изображения и другой контент.</span><span class="sxs-lookup"><span data-stu-id="06c71-130">**Div** elements contain text, images, and other content.</span></span> <span data-ttu-id="06c71-131">Входной и выходной HTML-код для элемента **div** может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="06c71-131">Divs contain text, images, and other content. A **div** element can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="06c71-132">**Входные атрибуты**</span><span class="sxs-lookup"><span data-stu-id="06c71-132">**Input attributes**</span></span>

|<span data-ttu-id="06c71-133">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="06c71-133">Input attribute</span></span>|<span data-ttu-id="06c71-134">Описание</span><span class="sxs-lookup"><span data-stu-id="06c71-134">Description</span></span>|
|:------|:------|
| <span data-ttu-id="06c71-135">data-id</span><span class="sxs-lookup"><span data-stu-id="06c71-135">data-id</span></span> | <span data-ttu-id="06c71-136">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="06c71-136">A reference for the element.</span></span> <span data-ttu-id="06c71-137">Используется для [обновления содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="06c71-137">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="06c71-138">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="06c71-138">data-render-fallback</span></span> | <span data-ttu-id="06c71-139">Резервное действие в случае ошибки [извлечения](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data): **render** (по умолчанию) или **none**.</span><span class="sxs-lookup"><span data-stu-id="06c71-139">The fallback action if the [extraction](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data) fails: **render** (default) or **none**.</span></span> |
| <span data-ttu-id="06c71-140">data-render-method</span><span class="sxs-lookup"><span data-stu-id="06c71-140">data-render-method</span></span> | <span data-ttu-id="06c71-141">Выполняемый метод [извлечения](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data), например `extract.businesscard` или `extract.recipe`.</span><span class="sxs-lookup"><span data-stu-id="06c71-141">The [extraction](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data) method to perform, for example: `extract.businesscard`extract.businesscard`extract.recipe`

or extract.recipe.</span></span> |
| <span data-ttu-id="06c71-142">data-render-src</span><span class="sxs-lookup"><span data-stu-id="06c71-142">data-render-src</span></span> | <span data-ttu-id="06c71-143">Источник контента для [извлечения](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data).</span><span class="sxs-lookup"><span data-stu-id="06c71-143">The content source for the [extraction](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data).</span></span> |
| <span data-ttu-id="06c71-144">style</span><span class="sxs-lookup"><span data-stu-id="06c71-144">style</span></span> | <p><span data-ttu-id="06c71-145">Свойства положения, размера, шрифта и цвета для разделителя:</span><span class="sxs-lookup"><span data-stu-id="06c71-145">The position, size, font, and color properties for the div:</span></span></p><p> <span data-ttu-id="06c71-146">- **position** (только **absolute**), **left**, **top** и **width**.</span><span class="sxs-lookup"><span data-stu-id="06c71-146">- **position** (**absolute** only), **left**, **top**, and **width**.</span></span> <span data-ttu-id="06c71-147">Высота разделителей настраивается автоматически.</span><span class="sxs-lookup"><span data-stu-id="06c71-147">(Height is auto-configured for divs.)</span></span><br /><span data-ttu-id="06c71-148">Используется для создания разделителя с [абсолютным положением](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos), только если разделитель является непосредственным дочерним элементом основного текста, для которого задан атрибут `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="06c71-148">Used to create an [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) div, only if the div is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br /><span data-ttu-id="06c71-149">Пример: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="06c71-149">Example`<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span></p><p> <span data-ttu-id="06c71-150">Свойства CSS [style](#styles) для элемента.</span><span class="sxs-lookup"><span data-stu-id="06c71-150">The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="06c71-151">В выходном HTML-коде эти значения встроены в соответствующие дочерние элементы.</span><span class="sxs-lookup"><span data-stu-id="06c71-151">The CSS style properties of the element. In the output HTML, these values are returned inline on appropriate child elements.</span></span></p> |
 

<span data-ttu-id="06c71-152">API OneNote в Microsoft Graph заключают все содержимое основного текста по крайней мере в один разделитель.</span><span class="sxs-lookup"><span data-stu-id="06c71-152">The OneNote APIs in Microsoft Graph wrap all body content in at least one div.</span></span> <span data-ttu-id="06c71-153">API создает разделитель по умолчанию (с атрибутом `data-id="_default"`) для содержимого основного текста, если:</span><span class="sxs-lookup"><span data-stu-id="06c71-153">The API creates a default div (attributed with `data-id="_default"`) to contain the body content if:</span></span>

- <span data-ttu-id="06c71-154">Входной атрибут **data-absolute-enabled** элемента body пропущен или для него задано значение **false**.</span><span class="sxs-lookup"><span data-stu-id="06c71-154">The input body element's data-absolute-enabled attribute is omitted or set to false. In this case, all body content is put in the default div.</span></span> <span data-ttu-id="06c71-155">В этом случае все содержимое основного текста помещается в разделитель по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="06c71-155">The input body element's data-absolute-enabled attribute is omitted or set to false. In this case, all body content is put in the default div.</span></span>

- <span data-ttu-id="06c71-156">Для входного атрибута **data-absolute-enabled** элемента body задано значение **true**, но входной HTML-код содержит непосредственные дочерние элементы&nbsp;**div**, **img** или **object** без [абсолютного положения](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos).</span><span class="sxs-lookup"><span data-stu-id="06c71-156">The input body element's data-absolute-enabled attribute is true, but the input HTML  contains direct children that aren't absolutely positioned div, img, or object elements. In this case, direct children that aren't absolutely positioned div, img, or object elements are put in the default div.</span></span> <span data-ttu-id="06c71-157">В этом случае непосредственные дочерние элементы &nbsp;**div**, **img** или **object** без [абсолютного положения](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) помещаются в разделитель по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="06c71-157">In this case, direct children that aren't [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)&nbsp;**div**, **img**, or **object** elements are put in the default div.</span></span>


<span data-ttu-id="06c71-158">**Выходные атрибуты**</span><span class="sxs-lookup"><span data-stu-id="06c71-158">**Output attributes**</span></span>

|<span data-ttu-id="06c71-159">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="06c71-159">Output attribute</span></span>|<span data-ttu-id="06c71-160">Описание</span><span class="sxs-lookup"><span data-stu-id="06c71-160">Description</span></span>|
|:------|:------|
| <span data-ttu-id="06c71-161">data-id</span><span class="sxs-lookup"><span data-stu-id="06c71-161">data-id</span></span> | <span data-ttu-id="06c71-162">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="06c71-162">A reference for the element.</span></span> <span data-ttu-id="06c71-163">Используется для [обновления содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="06c71-163">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="06c71-164">id</span><span class="sxs-lookup"><span data-stu-id="06c71-164">id</span></span> | <span data-ttu-id="06c71-165">Уникальный сгенерированный ИД элемента.</span><span class="sxs-lookup"><span data-stu-id="06c71-165">A unique ID for the group.</span></span> <span data-ttu-id="06c71-166">Возвращается [запросами GET к конечной точке *content* страницы](../api-reference/v1.0/api/page_get.md) при использовании параметра запроса `includeIDs=true`.</span><span class="sxs-lookup"><span data-stu-id="06c71-166">A unique, generated ID for the element. Returned by GET  requests to  a page's  *content* endpoint when the includeIDs=true`includeIDs=true` query option is used. Used for page updates.</span></span> <span data-ttu-id="06c71-167">Используется для [обновления содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="06c71-167">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="06c71-168">style</span><span class="sxs-lookup"><span data-stu-id="06c71-168">style</span></span> | <span data-ttu-id="06c71-169">Свойства позиции и размера разделителя.</span><span class="sxs-lookup"><span data-stu-id="06c71-169">The position and size properties of the div.</span></span> |
 
### <a name="non-contributing-divs"></a><span data-ttu-id="06c71-170">Вспомогательные разделители</span><span class="sxs-lookup"><span data-stu-id="06c71-170">Non-contributing divs</span></span>
<span data-ttu-id="06c71-171">Если элемент **div** во входных данных HTML не входит в структуру страницы и не переносит сведения, используемые приложением OneNote, API перемещает содержимое разделителя в родительский или используемый по умолчанию разделитель.</span><span class="sxs-lookup"><span data-stu-id="06c71-171">When a div element in the input HTML does not contribute to the page structure or carry information that onnvshort uses,  the API moves the div's content into the parent or default div.</span></span> <span data-ttu-id="06c71-172">Это процесс показан в приведенном ниже примере.</span><span class="sxs-lookup"><span data-stu-id="06c71-172">This is illustrated in the following examples.</span></span>

<span data-ttu-id="06c71-173">**Входной HTML-код**, который содержит вспомогательный вложенный разделитель.</span><span class="sxs-lookup"><span data-stu-id="06c71-173">**Input HTML**  that contains a non-contributing, nested div.</span></span>

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

<span data-ttu-id="06c71-174">**Выходной HTML-код**</span><span class="sxs-lookup"><span data-stu-id="06c71-174">**Output HTML**</span></span>

><span data-ttu-id="06c71-175">**Примечание.** Содержимое разделителя было перемещено в родительский разделитель, а вложенные теги `<div>` были удалены.</span><span class="sxs-lookup"><span data-stu-id="06c71-175">**Note:** The div's content was moved to the parent div and the nested `<div>` tags have been removed.</span></span> <span data-ttu-id="06c71-176">Разделитель был бы сохранен, если бы в нем были определены какие-либо семантические сведения, такие как **data-id** (пример: `<div data-id="keep-me">`).</span><span class="sxs-lookup"><span data-stu-id="06c71-176">The div would have been preserved if it defined any semantic information, such as a **data-id** (example: `<div data-id="keep-me">`).</span></span>

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


## <a name="img-elements"></a><span data-ttu-id="06c71-177">Элементы Img</span><span class="sxs-lookup"><span data-stu-id="06c71-177">Img elements</span></span>
<span data-ttu-id="06c71-178">Для представления изображений на страницах OneNote используются элементы **img**.</span><span class="sxs-lookup"><span data-stu-id="06c71-178">Images on OneNote pages are represented by **img** elements.</span></span> <span data-ttu-id="06c71-179">Входной и выходной HTML-код для элемента **img** может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="06c71-179">Images on onnvshort pages are represented by **img** elements. An img element can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="06c71-180">**Входные атрибуты**</span><span class="sxs-lookup"><span data-stu-id="06c71-180">**Input attributes**</span></span>

|<span data-ttu-id="06c71-181">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="06c71-181">Input attribute</span></span>|<span data-ttu-id="06c71-182">Описание</span><span class="sxs-lookup"><span data-stu-id="06c71-182">Description</span></span>|
|:------|:------|
| <span data-ttu-id="06c71-183">alt</span><span class="sxs-lookup"><span data-stu-id="06c71-183">alt</span></span> | <span data-ttu-id="06c71-184">Предоставленный замещающий текст для изображения.</span><span class="sxs-lookup"><span data-stu-id="06c71-184">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="06c71-185">data-id</span><span class="sxs-lookup"><span data-stu-id="06c71-185">data-id</span></span> | <span data-ttu-id="06c71-186">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="06c71-186">A reference for the element.</span></span> <span data-ttu-id="06c71-187">Используется для [обновления содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="06c71-187">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="06c71-188">data-render-src</span><span class="sxs-lookup"><span data-stu-id="06c71-188">data-render-src</span></span> |<span data-ttu-id="06c71-189">Должно было задано значение **data-render-src** или **src**.</span><span class="sxs-lookup"><span data-stu-id="06c71-189">Either **data-render-src** or **src** is required.</span></span><br/><br/><span data-ttu-id="06c71-190">Веб-страница, которая будет отображаться в виде битового изображения на странице OneNote:</span><span class="sxs-lookup"><span data-stu-id="06c71-190">The webpage to render as a bit-mapped image on the onnvshort page:</span></span><br /> <span data-ttu-id="06c71-191">- `data-render-src="http://..."` для общедоступного URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="06c71-191">- `data-render-src="http://..."` for a public URL.</span></span><br /> <span data-ttu-id="06c71-192">- `data-render-src="name:BlockName"` для части изображения в блоке Presentation [составного запроса](../api-reference/v1.0/api/section_post_pages.md#example).</span><span class="sxs-lookup"><span data-stu-id="06c71-192">- `data-render-src="name:BlockName"` for an image part in the "Presentation" block of a [multipart request](../api-reference/v1.0/api/section_post_pages.md#example).</span></span><br/><br/><span data-ttu-id="06c71-193">Этот метод удобно использовать, если веб-страница слишком сложна для достоверного отображения в OneNote или для использования страницы необходимы учетные данные.</span><span class="sxs-lookup"><span data-stu-id="06c71-193">data-render-src="name:BlockName" for an image part in the Presentation block of a multi-part request. This method is useful when the webpage is more complex than the onnvshort page can faithfully render, or when the page requires login credentials.</span></span>|
| <span data-ttu-id="06c71-194">data-tag</span><span class="sxs-lookup"><span data-stu-id="06c71-194">data-tag</span></span> | <span data-ttu-id="06c71-195">[Тег заметки](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) для элемента.</span><span class="sxs-lookup"><span data-stu-id="06c71-195">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on the element.</span></span> |
| <span data-ttu-id="06c71-196">style</span><span class="sxs-lookup"><span data-stu-id="06c71-196">style</span></span> |<span data-ttu-id="06c71-197">Свойства положения и размера изображения: **position** (только **absolute**), **left**, **top**, **width** и **height**.</span><span class="sxs-lookup"><span data-stu-id="06c71-197">The position and size properties for the image: **position** (**absolute** only), **left**, **top**, **width**, and **height**.</span></span><br/><br/><span data-ttu-id="06c71-198">Размер можно задать для любого изображения.</span><span class="sxs-lookup"><span data-stu-id="06c71-198">Size can be set on any image.</span></span> <span data-ttu-id="06c71-199">Свойства положения используются для создания изображения с [абсолютным положением](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos), только если изображение является непосредственным дочерним элементом основного текста, для которого задан атрибут `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="06c71-199">Position properties are used to create an [absolute positioned](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos) image, only if the image is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br /><span data-ttu-id="06c71-200">Пример: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="06c71-200">Example`<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span><br/><br/><span data-ttu-id="06c71-201">В выходном HTML-коде размеры изображения возвращаются по отдельности через атрибуты **width** и **height**.</span><span class="sxs-lookup"><span data-stu-id="06c71-201">In the output HTML, the image size is returned separately in  **width** and **height** attributes.</span></span> |
| <span data-ttu-id="06c71-202">src</span><span class="sxs-lookup"><span data-stu-id="06c71-202">src</span></span> |<span data-ttu-id="06c71-203">Должно было задано значение **src** или **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="06c71-203">Either **src** or **data-render-src** is required.</span></span><br/><br/><span data-ttu-id="06c71-204">Изображение, отображаемое на странице OneNote:</span><span class="sxs-lookup"><span data-stu-id="06c71-204">The image to render on the onnvshort page:</span></span><br /> <span data-ttu-id="06c71-205">- `src="http://..."`: URL-адрес общедоступного изображения в Интернете.</span><span class="sxs-lookup"><span data-stu-id="06c71-205">src="http://..." for a URL to a publicly available image on the internet.</span></span><br /> <span data-ttu-id="06c71-206">- `src="name:BlockName"`: именованная часть составного запроса, представляющая изображение.</span><span class="sxs-lookup"><span data-stu-id="06c71-206">src="name:BlockName" for a named part in a multi-part request that represents the image.</span></span>|
| <span data-ttu-id="06c71-207">width, height</span><span class="sxs-lookup"><span data-stu-id="06c71-207">width, height</span></span> | <span data-ttu-id="06c71-208">Ширина и высота изображения в пикселях, но без обозначения px.</span><span class="sxs-lookup"><span data-stu-id="06c71-208">The width or height of the image, in pixels but without the px. Example: width="400"</span></span> <span data-ttu-id="06c71-209">Пример: `width="400"`</span><span class="sxs-lookup"><span data-stu-id="06c71-209">Example`width="400"`</span></span> |
 
><span data-ttu-id="06c71-210">**Примечание.** API OneNote автоматически определяют тип входного изображения и возвращают его в качестве атрибута **data-fullres-src-type** во входном HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="06c71-210">**Note:** The OneNote APIs automatically detect the input image type, and returns it as the **data-fullres-src-type** in the output HTML.</span></span> <span data-ttu-id="06c71-211">API также возвращает тип оптимизированного изображения в атрибуте **data-src-type**.</span><span class="sxs-lookup"><span data-stu-id="06c71-211">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 

<span data-ttu-id="06c71-212">**Выходные атрибуты**</span><span class="sxs-lookup"><span data-stu-id="06c71-212">**Output attributes**</span></span>

|<span data-ttu-id="06c71-213">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="06c71-213">Output attribute</span></span>|<span data-ttu-id="06c71-214">Описание</span><span class="sxs-lookup"><span data-stu-id="06c71-214">Description</span></span>|
|:------|:------|
| <span data-ttu-id="06c71-215">alt</span><span class="sxs-lookup"><span data-stu-id="06c71-215">alt</span></span> | <span data-ttu-id="06c71-216">Предоставленный замещающий текст для изображения.</span><span class="sxs-lookup"><span data-stu-id="06c71-216">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="06c71-217">data-id</span><span class="sxs-lookup"><span data-stu-id="06c71-217">data-id</span></span> | <span data-ttu-id="06c71-218">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="06c71-218">A reference for the element.</span></span> <span data-ttu-id="06c71-219">Используется для [обновления содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="06c71-219">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="06c71-220">data-index</span><span class="sxs-lookup"><span data-stu-id="06c71-220">data-index</span></span> | <span data-ttu-id="06c71-221">Положение изображения.</span><span class="sxs-lookup"><span data-stu-id="06c71-221">The position properties of the image.</span></span> <span data-ttu-id="06c71-222">Для поддержки [разделенных изображений](#split-images).</span><span class="sxs-lookup"><span data-stu-id="06c71-222">For [split image](#split-images) support.</span></span> |
| <span data-ttu-id="06c71-223">data-fullres-src</span><span class="sxs-lookup"><span data-stu-id="06c71-223">data-fullres-src</span></span> | <span data-ttu-id="06c71-224">Конечная точка версии изображения, которая была изначально внедрена на странице.</span><span class="sxs-lookup"><span data-stu-id="06c71-224">The endpoint for the version of the image resource that was originally embedded in the page.</span></span> |
| <span data-ttu-id="06c71-225">data-fullres-src-type</span><span class="sxs-lookup"><span data-stu-id="06c71-225">data-fullres-src-type</span></span> | <span data-ttu-id="06c71-226">Тип мультимедиа для ресурса **data-fullres-src**, например `image/png` или `image/jpeg`.</span><span class="sxs-lookup"><span data-stu-id="06c71-226">The MIME type of the **data-fullres-src** resource, for example: image/png`image/png` or image/jpeg`image/jpeg`.</span></span> |
| <span data-ttu-id="06c71-227">data-options</span><span class="sxs-lookup"><span data-stu-id="06c71-227">data-options</span></span> | <span data-ttu-id="06c71-228">Тип источника: **printout** для PDF-файлов или **splitimage** для всех остальных.</span><span class="sxs-lookup"><span data-stu-id="06c71-228">The source type: **printout** for PDF files or **splitimage** for all others. Applies only to split images created with the data-render-src attribute.</span></span> <span data-ttu-id="06c71-229">Применяется только к [разделенным изображениям](#split-images), созданным с использованием атрибута **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="06c71-229">The source type: **printout** for PDF files or splitimage for all others. Applies only to [split images](#split-images) created with the data-render-src attribute.</span></span> |
| <span data-ttu-id="06c71-230">data-render-original-src</span><span class="sxs-lookup"><span data-stu-id="06c71-230">data-render-original-src</span></span> | <span data-ttu-id="06c71-231">Исходный URL-адрес источника изображения, если исходное изображение находится в общедоступной части Интернета и создано с использованием атрибута **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="06c71-231">The original source URL of the image, if the source image  is from the public internet and was created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="06c71-232">data-src-type</span><span class="sxs-lookup"><span data-stu-id="06c71-232">data-src-type</span></span> | <span data-ttu-id="06c71-233">Тип мультимедиа для ресурса **src**, например `image/png` или `image/jpeg`.</span><span class="sxs-lookup"><span data-stu-id="06c71-233">The MIME type of the **src** resource, for example: image/png`image/png` or image/jpeg`image/jpeg`.</span></span> |
| <span data-ttu-id="06c71-234">data-tag</span><span class="sxs-lookup"><span data-stu-id="06c71-234">data-tag</span></span> | <span data-ttu-id="06c71-235">[Тег заметки](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) для элемента.</span><span class="sxs-lookup"><span data-stu-id="06c71-235">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on the element.</span></span> |
| <span data-ttu-id="06c71-236">id</span><span class="sxs-lookup"><span data-stu-id="06c71-236">id</span></span> | <span data-ttu-id="06c71-237">Уникальный сгенерированный ИД элемента.</span><span class="sxs-lookup"><span data-stu-id="06c71-237">A unique ID for the group.</span></span> <span data-ttu-id="06c71-238">Возвращается [запросами GET к конечной точке *content* страницы](../api-reference/v1.0/api/page_get.md) при использовании параметра запроса `includeIDs=true`.</span><span class="sxs-lookup"><span data-stu-id="06c71-238">A unique, generated ID for the element. Returned by GET  requests to  a page's  *content* endpoint when the includeIDs=true`includeIDs=true` query option is used. Used for page updates.</span></span> <span data-ttu-id="06c71-239">Используется для [обновления содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="06c71-239">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="06c71-240">src</span><span class="sxs-lookup"><span data-stu-id="06c71-240">src</span></span> | <span data-ttu-id="06c71-241">Конечная точка версии изображения, оптимизированного для веб-браузеров, а также мобильных телефонов и планшетов.</span><span class="sxs-lookup"><span data-stu-id="06c71-241">The endpoint for the version of the image resource that has been optimized for web browsers and mobile and tablet form factors.</span></span> |
| <span data-ttu-id="06c71-242">style</span><span class="sxs-lookup"><span data-stu-id="06c71-242">style</span></span> | <span data-ttu-id="06c71-243">Свойства позиции изображения.</span><span class="sxs-lookup"><span data-stu-id="06c71-243">The position properties of the image.</span></span> |
| <span data-ttu-id="06c71-244">width, height</span><span class="sxs-lookup"><span data-stu-id="06c71-244">width, height</span></span> | <span data-ttu-id="06c71-245">Ширина или высота изображения в пикселях.</span><span class="sxs-lookup"><span data-stu-id="06c71-245">The width or height of the image, in pixels.</span></span> |
 

### <a name="output-html-examples-for-images"></a><span data-ttu-id="06c71-246">Примеры выходного HTML-кода для изображений</span><span class="sxs-lookup"><span data-stu-id="06c71-246">Output HTML examples for images</span></span>
<span data-ttu-id="06c71-247">Выходные элементы **img** содержат конечные точки для ресурсов файлов изображений и типа изображения, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="06c71-247">Output **img** elements contain endpoints for image file resources and the image type, as shown below.</span></span> <span data-ttu-id="06c71-248">Вы можете отправлять отдельные [запросы GET к конечным точкам ресурсов изображений](../api-reference/v1.0/api/resource_get.md), чтобы получать их двоичное содержимое.</span><span class="sxs-lookup"><span data-stu-id="06c71-248">Output object elements  contain  endpoints that link to the file resources in the page. You can make separate GET requests to these resource endpoints to retrieve their binary contents.</span></span>

```http
<img 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="06c71-249">По умолчанию изображения не отображаются непосредственно в браузере, так как они являются личными и для их получения необходимо пройти проверку подлинности, как и для другого содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="06c71-249">Images won’t render directly in a browser because they are private and require authorization to retrieve them, like the rest of the page contents.</span></span> <span data-ttu-id="06c71-250">Чтобы получить общедоступные URL-адреса ресурсов изображений на странице, включите параметр **preAuthenticated=true** в строку запроса при получении содержимого страницы (пример: `GET ../pages/{page-id}/content?preAuthenticated=true`).</span><span class="sxs-lookup"><span data-stu-id="06c71-250">To get public URLs to the image resources on a page, include **preAuthenticated=true** in the query string when you retrieve the page content (example: `GET ../pages/{page-id}/content?preAuthenticated=true`).</span></span> <span data-ttu-id="06c71-251">Возвращаемые общедоступные URL-адреса действительны в течение одного часа.</span><span class="sxs-lookup"><span data-stu-id="06c71-251">The public URLs that are returned are valid for one hour.</span></span> 

<span data-ttu-id="06c71-252">**Изображение с общедоступным URL-адресом (в запрос включен параметр _preAuthenticated=true_)**</span><span class="sxs-lookup"><span data-stu-id="06c71-252">**Image with public URL when _preAuthenticated=true_ is included in the request**</span></span>

```html
<img 
    width="170" height="128" 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-src-type="image/{type}" 
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/content?publicAuth=true&mimeType=image/jpeg" 
    data-fullres-src-type="image/{type}" />
```

<span data-ttu-id="06c71-253">В приведенных ниже примерах показаны сведения, которые может содержать элемент **img** в выходном HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="06c71-253">The following examples show the information an **img** element might contain in the output HTML.</span></span>

<span data-ttu-id="06c71-254">**Изображение с ресурсами высокого разрешения для Интернета**</span><span class="sxs-lookup"><span data-stu-id="06c71-254">**Image with web-ready and high resolution resources**</span></span>

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

<span data-ttu-id="06c71-255">**Изображение, созданное с использованием атрибута *data-render-src***</span><span class="sxs-lookup"><span data-stu-id="06c71-255">**Image created by using the *data-render-src* attribute**</span></span>

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

### <a name="split-images"></a><span data-ttu-id="06c71-256">Разделенные изображения</span><span class="sxs-lookup"><span data-stu-id="06c71-256">Split images</span></span>

<span data-ttu-id="06c71-257">Изображения, созданные с использованием атрибута **data-render-src** (из URL-адреса страницы или именованной части), могут быть разделены на несколько компонентов для повышения производительности и удобства отрисовки.</span><span class="sxs-lookup"><span data-stu-id="06c71-257">Images that are created using the **data-render-src** attribute from a webpage URL or a named part might be split into multiple component images for performance and rendering reasons. Component images are all assigned the same data-id value.  Each component image has a zero-based data-index attribute that defines the  original vertical layout.</span></span> <span data-ttu-id="06c71-258">Всем компонентам изображения назначается одно и то же значение **data-id**.</span><span class="sxs-lookup"><span data-stu-id="06c71-258">Component images are all assigned the same **data-id** value.</span></span> <span data-ttu-id="06c71-259">У каждого компонента изображения есть атрибут data-index с отсчетом от нуля, определяющий исходную вертикальную компоновку.</span><span class="sxs-lookup"><span data-stu-id="06c71-259">Each component image has a zero-based data-index attribute that defines the original vertical layout.</span></span>

<span data-ttu-id="06c71-260">**Разделенное изображение с тремя компонентами**</span><span class="sxs-lookup"><span data-stu-id="06c71-260">**Split image with three component images**</span></span>

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

<span data-ttu-id="06c71-261">Так как пользователи могут перемещать изображения на странице, индексы могут возвращаться в измененном порядке.</span><span class="sxs-lookup"><span data-stu-id="06c71-261">Because users can move the images on the page, the returned indexes might be out of order.
Ordering should be in top to bottom y-order, then left to right x-order if there are y-order conflicts.</span></span> <span data-ttu-id="06c71-262">Сортировка должна выполняться сверху вниз, а затем слева направо (если возникнут конфликты при вертикальной сортировке).</span><span class="sxs-lookup"><span data-stu-id="06c71-262">Because users can move the images on the page, the returned indexes might be out of order.
Ordering should be in top to bottom y-order, then left to right x-order if there are y-order conflicts.</span></span>

## <a name="iframe-elements"></a><span data-ttu-id="06c71-263">Элементы iframe</span><span class="sxs-lookup"><span data-stu-id="06c71-263">iframe elements</span></span>
<span data-ttu-id="06c71-264">Страницы OneNote могут содержать внедренные видео, представленные элементами **iframe**.</span><span class="sxs-lookup"><span data-stu-id="06c71-264">OneNote pages can contain embedded videos represented by **iframe** elements.</span></span> 

><span data-ttu-id="06c71-265">**Примечание.** Вы также можете [вложить видеофайл с помощью элемента **object**](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#files).</span><span class="sxs-lookup"><span data-stu-id="06c71-265">**Note:** You can also [attach a video file using an **object** element](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#files).</span></span>

<span data-ttu-id="06c71-266">**Входные атрибуты**</span><span class="sxs-lookup"><span data-stu-id="06c71-266">**Input attributes**</span></span>

|<span data-ttu-id="06c71-267">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="06c71-267">Input attribute</span></span>|<span data-ttu-id="06c71-268">Описание</span><span class="sxs-lookup"><span data-stu-id="06c71-268">Description</span></span>|
|:------|:------|
| <span data-ttu-id="06c71-269">data-original-src</span><span class="sxs-lookup"><span data-stu-id="06c71-269">data-original-src</span></span> | <span data-ttu-id="06c71-270">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06c71-270">Required.</span></span> <span data-ttu-id="06c71-271">URL-адрес источника видео.</span><span class="sxs-lookup"><span data-stu-id="06c71-271">The URL of the video source.</span></span> <span data-ttu-id="06c71-272">См. [список поддерживаемых источников видео](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#videos).</span><span class="sxs-lookup"><span data-stu-id="06c71-272">See the [list of supported video sources](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#videos).</span></span> <span data-ttu-id="06c71-273">Пример: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="06c71-273">Example`data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span> |
| <span data-ttu-id="06c71-274">width, height</span><span class="sxs-lookup"><span data-stu-id="06c71-274">width, height</span></span> | <span data-ttu-id="06c71-275">Ширина или высота элемента iframe в пикселях.</span><span class="sxs-lookup"><span data-stu-id="06c71-275">The width or height of the image, in pixels.</span></span> <span data-ttu-id="06c71-276">Пример: `width=300`</span><span class="sxs-lookup"><span data-stu-id="06c71-276">Example`width=300`</span></span> |

<span data-ttu-id="06c71-277">**Выходные атрибуты**</span><span class="sxs-lookup"><span data-stu-id="06c71-277">**Output attributes**</span></span>

|<span data-ttu-id="06c71-278">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="06c71-278">Output attribute</span></span>|<span data-ttu-id="06c71-279">Описание</span><span class="sxs-lookup"><span data-stu-id="06c71-279">Description</span></span>|
|:------|:------|
| <span data-ttu-id="06c71-280">data-original-src</span><span class="sxs-lookup"><span data-stu-id="06c71-280">data-original-src</span></span> | <span data-ttu-id="06c71-281">URL-адрес источника видео.</span><span class="sxs-lookup"><span data-stu-id="06c71-281">The URL of the video source.</span></span> |
| <span data-ttu-id="06c71-282">src</span><span class="sxs-lookup"><span data-stu-id="06c71-282">src</span></span> | <span data-ttu-id="06c71-283">Ссылка на видео, внедренное в страницу OneNote.</span><span class="sxs-lookup"><span data-stu-id="06c71-283">A link to the video that is embedded in the OneNote page.</span></span> |
| <span data-ttu-id="06c71-284">width, height</span><span class="sxs-lookup"><span data-stu-id="06c71-284">width, height</span></span> | <span data-ttu-id="06c71-285">Ширина или высота элемента iframe в пикселях.</span><span class="sxs-lookup"><span data-stu-id="06c71-285">The width or height of the image, in pixels.</span></span> <span data-ttu-id="06c71-286">Пример: `width=300`</span><span class="sxs-lookup"><span data-stu-id="06c71-286">Example`width=300`</span></span> |
 
<span data-ttu-id="06c71-287">Пример **выходного HTML-кода** для видео</span><span class="sxs-lookup"><span data-stu-id="06c71-287">Output HTML example for objects</span></span>

<span data-ttu-id="06c71-288">Выходные элементы **iframe** содержат конечные точки, ссылающиеся на исходную страницу и видео, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="06c71-288">Output **iframe** elements contain endpoints that link to the source page and video, as shown.</span></span> 

```html
<iframe 
    width="340" height="280" 
    data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" 
    src="https://www.youtube.com/embed/3Ztr44aKmQ8?feature=oembed&autoplay=true" />
``` 

## <a name="object-elements"></a><span data-ttu-id="06c71-289">Элементы Object</span><span class="sxs-lookup"><span data-stu-id="06c71-289">Object elements</span></span>
<span data-ttu-id="06c71-290">Страницы OneNote могут содержать вложения, представленные элементами **object**.</span><span class="sxs-lookup"><span data-stu-id="06c71-290">OneNote pages can contain file attachments represented by **object** elements.</span></span> <span data-ttu-id="06c71-291">Входной и выходной HTML-код для элемента **object** может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="06c71-291">onnvshort pages can contain file attachments  represented by **object** elements. An object element can contain the following attributes in the input and output HTML.</span></span>

><span data-ttu-id="06c71-292">**Примечание.** API OneNote также может отображать содержимое файлов в виде изображений на странице, если файл отправлен как изображение и использует атрибут **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="06c71-292">The onnvshort API can also render file content as images in a page when the file is sent as an image and uses the data-render-src attribute.  Example: <img data-render-src="name:BlockName" ... /></span></span> <span data-ttu-id="06c71-293">Пример: `<img data-render-src="name:part-name" ... />`</span><span class="sxs-lookup"><span data-stu-id="06c71-293">Example`<img data-render-src="name:part-name" ... />`</span></span>
 

<span data-ttu-id="06c71-294">**Входные атрибуты**</span><span class="sxs-lookup"><span data-stu-id="06c71-294">**Input attributes**</span></span>

|<span data-ttu-id="06c71-295">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="06c71-295">Input attribute</span></span>|<span data-ttu-id="06c71-296">Описание</span><span class="sxs-lookup"><span data-stu-id="06c71-296">Description</span></span>|
|:------|:------|
| <span data-ttu-id="06c71-297">data</span><span class="sxs-lookup"><span data-stu-id="06c71-297">data</span></span> | <span data-ttu-id="06c71-298">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06c71-298">Required.</span></span> <span data-ttu-id="06c71-299">Имя части, которая представляет файл в [составном запросе](../api-reference/v1.0/api/section_post_pages.md#example).</span><span class="sxs-lookup"><span data-stu-id="06c71-299">Required. The name of the part that represents the file in the multi-part request.</span></span> |
| <span data-ttu-id="06c71-300">data-attachment</span><span class="sxs-lookup"><span data-stu-id="06c71-300">data-attachment</span></span> | <span data-ttu-id="06c71-p137">Обязательный параметр. Имя файла.</span><span class="sxs-lookup"><span data-stu-id="06c71-p137">Required. The file name.</span></span> |
| <span data-ttu-id="06c71-303">data-id</span><span class="sxs-lookup"><span data-stu-id="06c71-303">data-id</span></span> | <span data-ttu-id="06c71-304">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="06c71-304">A reference for the element.</span></span> <span data-ttu-id="06c71-305">Используется для [обновления содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="06c71-305">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="06c71-306">style</span><span class="sxs-lookup"><span data-stu-id="06c71-306">style</span></span> | <p><span data-ttu-id="06c71-307">Свойства положения и размера объекта: **position** (только **absolute**), **left**, **top** и **width**.</span><span class="sxs-lookup"><span data-stu-id="06c71-307">The position and size properties for the object: **position** (**absolute** only), **left**, **top**, and **width**.</span></span></p><p><span data-ttu-id="06c71-308">Используется для создания объекта с [абсолютным положением](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos), только если объект является непосредственным дочерним элементом основного текста, для которого задан атрибут `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="06c71-308">position (absolute only), left, top, and width properties. Used to create an absolutely positioned object, only if the object is a direct child of the body when the  body sets data-absolute-enabled="true". Learn more about absolutely positioned elements. Example: <object style="position:absolute;top:350px;left:300px" ... /></span></span><br /><span data-ttu-id="06c71-309">Пример: `<object style="position:absolute;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="06c71-309">Example`<object style="position:absolute;top:350px;left:300px" ... />`</span></span></p> |
| <span data-ttu-id="06c71-310">type</span><span class="sxs-lookup"><span data-stu-id="06c71-310">type</span></span> | <span data-ttu-id="06c71-311">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06c71-311">Required.</span></span> <span data-ttu-id="06c71-312">Стандартный тип файла мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="06c71-312">The standard MIME file type.</span></span> <span data-ttu-id="06c71-313">Для файлов известных типов на странице OneNote отображается значок, связанный с типом файла.</span><span class="sxs-lookup"><span data-stu-id="06c71-313">Required. The standard MIME file type.  Known file types display the icon associated with the file type on the onnvshort page. Unknown file types display a generic file icon.</span></span> <span data-ttu-id="06c71-314">Для файлов неизвестных типов отображается универсальный значок файла.</span><span class="sxs-lookup"><span data-stu-id="06c71-314">Unknown file types display a generic file icon.</span></span> |
<!--todo: add link to known file types--> 

<span data-ttu-id="06c71-315">**Выходные атрибуты**</span><span class="sxs-lookup"><span data-stu-id="06c71-315">**Output attributes**</span></span>

|<span data-ttu-id="06c71-316">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="06c71-316">Output attribute</span></span>|<span data-ttu-id="06c71-317">Описание</span><span class="sxs-lookup"><span data-stu-id="06c71-317">Description</span></span>|
|:------|:------|
| <span data-ttu-id="06c71-318">data</span><span class="sxs-lookup"><span data-stu-id="06c71-318">data</span></span> | <span data-ttu-id="06c71-319">Конечная точка файлового ресурса.</span><span class="sxs-lookup"><span data-stu-id="06c71-319">The endpoint for the file resource.</span></span> |
| <span data-ttu-id="06c71-320">data-attachment</span><span class="sxs-lookup"><span data-stu-id="06c71-320">data-attachment</span></span> | <span data-ttu-id="06c71-321">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="06c71-321">The file name.</span></span> |
| <span data-ttu-id="06c71-322">data-id</span><span class="sxs-lookup"><span data-stu-id="06c71-322">data-id</span></span> | <span data-ttu-id="06c71-323">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="06c71-323">A reference for the element.</span></span> <span data-ttu-id="06c71-324">Используется для [обновления содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="06c71-324">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="06c71-325">id</span><span class="sxs-lookup"><span data-stu-id="06c71-325">id</span></span> | <span data-ttu-id="06c71-326">Уникальный сгенерированный ИД элемента.</span><span class="sxs-lookup"><span data-stu-id="06c71-326">A unique ID for the group.</span></span> <span data-ttu-id="06c71-327">Возвращается [запросами GET к конечной точке *content* страницы](../api-reference/v1.0/api/page_get.md) при использовании параметра запроса `includeIDs=true`.</span><span class="sxs-lookup"><span data-stu-id="06c71-327">A unique, generated ID for the element. Returned by GET  requests to  a page's  *content* endpoint when the includeIDs=true`includeIDs=true` query option is used. Used for page updates.</span></span> <span data-ttu-id="06c71-328">Используется для [обновления содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="06c71-328">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="06c71-329">style</span><span class="sxs-lookup"><span data-stu-id="06c71-329">style</span></span> | <span data-ttu-id="06c71-330">Свойства позиции объекта.</span><span class="sxs-lookup"><span data-stu-id="06c71-330">The position properties of the object.</span></span> |
| <span data-ttu-id="06c71-331">type</span><span class="sxs-lookup"><span data-stu-id="06c71-331">type</span></span> | <span data-ttu-id="06c71-332">Стандартный тип файла мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="06c71-332">The standard MIME file type.</span></span> |
 

<span data-ttu-id="06c71-333">Пример **выходного HTML-кода** для объектов</span><span class="sxs-lookup"><span data-stu-id="06c71-333">Output HTML example for objects</span></span>

<span data-ttu-id="06c71-334">Выходные элементы **object** содержат конечные точки, ссылающиеся на файловые ресурсы со страницы, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="06c71-334">Output **object** elements contain endpoints that link to the file resources in the page, as shown.</span></span> <span data-ttu-id="06c71-335">Вы можете отправлять отдельные [запросы GET к конечным точкам файловых ресурсов](../api-reference/v1.0/api/resource_get.md), чтобы получать их двоичное содержимое.</span><span class="sxs-lookup"><span data-stu-id="06c71-335">Output object elements  contain  endpoints that link to the file resources in the page. You can make separate GET requests to these resource endpoints to retrieve their binary contents.</span></span>

```html
<object
    data="https://graph.microsoft.com/v1.0/me/onenote/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" 
    [style="..."] />
``` 

## <a name="paragraphs-and-headings"></a><span data-ttu-id="06c71-336">Абзацы и заголовки</span><span class="sxs-lookup"><span data-stu-id="06c71-336">Paragraphs and headings</span></span>

<span data-ttu-id="06c71-337">Входной и выходной HTML-код для абзацев, заголовков и других текстовых контейнеров может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="06c71-337">Paragraphs, headings, and other text containers can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="06c71-338">**Входные атрибуты**</span><span class="sxs-lookup"><span data-stu-id="06c71-338">**Input attributes**</span></span>

|<span data-ttu-id="06c71-339">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="06c71-339">Input attribute</span></span>|<span data-ttu-id="06c71-340">Описание</span><span class="sxs-lookup"><span data-stu-id="06c71-340">Description</span></span>|
|:------|:------|
| <span data-ttu-id="06c71-341">data-id</span><span class="sxs-lookup"><span data-stu-id="06c71-341">data-id</span></span> | <span data-ttu-id="06c71-342">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="06c71-342">A reference for the element.</span></span> <span data-ttu-id="06c71-343">Используется для [обновления содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="06c71-343">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="06c71-344">data-tag</span><span class="sxs-lookup"><span data-stu-id="06c71-344">data-tag</span></span> | <span data-ttu-id="06c71-345">[Тег заметки](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) для элемента **p** или **h1** - **h6**.</span><span class="sxs-lookup"><span data-stu-id="06c71-345">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="06c71-346">style</span><span class="sxs-lookup"><span data-stu-id="06c71-346">style</span></span> | <span data-ttu-id="06c71-347">Свойства CSS [style](#styles) для элемента.</span><span class="sxs-lookup"><span data-stu-id="06c71-347">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="06c71-348">**Выходные атрибуты**</span><span class="sxs-lookup"><span data-stu-id="06c71-348">**Output attributes**</span></span>

|<span data-ttu-id="06c71-349">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="06c71-349">Output attribute</span></span>|<span data-ttu-id="06c71-350">Описание</span><span class="sxs-lookup"><span data-stu-id="06c71-350">Description</span></span>|
|:------|:------|
| <span data-ttu-id="06c71-351">data-id</span><span class="sxs-lookup"><span data-stu-id="06c71-351">data-id</span></span> | <span data-ttu-id="06c71-352">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="06c71-352">A reference for the element.</span></span> <span data-ttu-id="06c71-353">Используется для [обновления содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="06c71-353">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="06c71-354">data-tag</span><span class="sxs-lookup"><span data-stu-id="06c71-354">data-tag</span></span> | <span data-ttu-id="06c71-355">[Тег заметки](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) для элемента **p** или **h1** - **h6**.</span><span class="sxs-lookup"><span data-stu-id="06c71-355">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="06c71-356">id</span><span class="sxs-lookup"><span data-stu-id="06c71-356">id</span></span> | <span data-ttu-id="06c71-357">Уникальный сгенерированный ИД элемента.</span><span class="sxs-lookup"><span data-stu-id="06c71-357">A unique ID for the group.</span></span> <span data-ttu-id="06c71-358">Возвращается [запросами GET к конечной точке *content* страницы](../api-reference/v1.0/api/page_get.md) при использовании параметра запроса `includeIDs=true`.</span><span class="sxs-lookup"><span data-stu-id="06c71-358">A unique, generated ID for the element. Returned by GET  requests to  a page's  *content* endpoint when the includeIDs=true`includeIDs=true` query option is used. Used for page updates.</span></span> <span data-ttu-id="06c71-359">Используется для [обновления содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="06c71-359">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="06c71-360">style</span><span class="sxs-lookup"><span data-stu-id="06c71-360">style</span></span> | <span data-ttu-id="06c71-361">Свойства CSS [style](#styles) для элемента.</span><span class="sxs-lookup"><span data-stu-id="06c71-361">The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="06c71-362">В выходном HTML-коде эти значения могут быть встроены в элементы **span** или соответствующие дочерние элементы.</span><span class="sxs-lookup"><span data-stu-id="06c71-362">The CSS style properties of the element. In the output HTML, these values may be returned on inline on appropriate child elements or span elements.</span></span> |
 

<span data-ttu-id="06c71-363">В приведенных ниже примерах показан входной HTML-код, где используются разные способы определения стилей в текстовых контейнерах, и возвращаемый выходной HTML-код.</span><span class="sxs-lookup"><span data-stu-id="06c71-363">The following examples show input HTML that uses different ways to define styles on text containers and the output HTML that's returned.</span></span>

<span data-ttu-id="06c71-364">**Входной HTML-код** со стилями, определенными с помощью встроенных стилей знаков, в начальном теге внутри элемента **span**.</span><span class="sxs-lookup"><span data-stu-id="06c71-364">**Input HTML** with styles defined using inline character styles, in the start tag,  and within a **span** element.</span></span>

```html
<h1>Heading <i>One</i> text</h1>
<p style="font-size:8pt;color:green;font-family:Courier;text-align:center">Some text</p>
<p>Some <span  style="font-size:16px;color:#ff0000;font-family:Segoe UI Black">more</span> text</p>
``` 

<span data-ttu-id="06c71-365">**Выходной HTML-код** со стилем знака `<i>` и параметрами шрифта в начальном теге `<p>`, возвращаемыми в виде встроенных стилей CSS в элементах **span**.</span><span class="sxs-lookup"><span data-stu-id="06c71-365">**Output HTML** with the **<i>`<i>` character style and the font settings in the <p>`<p>` start tag returned as inline CSS styles on span** elements.</span></span>

```html
<h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">Heading <span style="font-style:italic">One</span> text</h1>
<p style="text-align:center"><span style="font-family:Courier;font-size:8pt;color:green">Some text</span></p>
<p>Some <span style="font-family:Segoe UI Black;font-size:12pt;color:red">more</span> text</p>
``` 


## <a name="lists"></a><span data-ttu-id="06c71-366">Списки</span><span class="sxs-lookup"><span data-stu-id="06c71-366">Lists</span></span>
<span data-ttu-id="06c71-367">Для представления списков используются элементы **ol** или **ul**, которые содержат элементы списка, представленные элементами **li**.</span><span class="sxs-lookup"><span data-stu-id="06c71-367">
 


Lists are represented as ol or ul elements that can contain li elements.</span></span>

<span data-ttu-id="06c71-368">Входной и выходной HTML-код списков и их элементов может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="06c71-368">Lists and list items can contain the following attributes in the input and output HTML.</span></span>

<span data-ttu-id="06c71-369">**Входные атрибуты**</span><span class="sxs-lookup"><span data-stu-id="06c71-369">**Input attributes**</span></span>

|<span data-ttu-id="06c71-370">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="06c71-370">Input attribute</span></span>|<span data-ttu-id="06c71-371">Описание</span><span class="sxs-lookup"><span data-stu-id="06c71-371">Description</span></span>|
|:------|:------|
| <span data-ttu-id="06c71-372">data-id</span><span class="sxs-lookup"><span data-stu-id="06c71-372">data-id</span></span> | <span data-ttu-id="06c71-373">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="06c71-373">A reference for the element.</span></span> <span data-ttu-id="06c71-374">Используется для [обновления содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="06c71-374">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="06c71-375">data-tag</span><span class="sxs-lookup"><span data-stu-id="06c71-375">data-tag</span></span> | <span data-ttu-id="06c71-376">[Тег заметки](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) в элементе **ul**, **ol** или **li**.</span><span class="sxs-lookup"><span data-stu-id="06c71-376">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on a **ul**, **ol**, or **li** element.</span></span> |
| <span data-ttu-id="06c71-377">style</span><span class="sxs-lookup"><span data-stu-id="06c71-377">style</span></span> | <span data-ttu-id="06c71-378">Свойство **list-style-type** и свойство CSS [style](#styles) для списка или его элемента.</span><span class="sxs-lookup"><span data-stu-id="06c71-378">The **list-style-type** and the  CSS [style](#styles) properties for the list or list item.</span></span> |
 

<span data-ttu-id="06c71-379">**Выходные атрибуты**</span><span class="sxs-lookup"><span data-stu-id="06c71-379">**Output attributes**</span></span>

|<span data-ttu-id="06c71-380">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="06c71-380">Output attribute</span></span>|<span data-ttu-id="06c71-381">Описание</span><span class="sxs-lookup"><span data-stu-id="06c71-381">Description</span></span>|
|:------|:------|
| <span data-ttu-id="06c71-382">data-id</span><span class="sxs-lookup"><span data-stu-id="06c71-382">data-id</span></span> | <span data-ttu-id="06c71-383">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="06c71-383">A reference for the element.</span></span> <span data-ttu-id="06c71-384">Используется для [обновления содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="06c71-384">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="06c71-385">data-tag</span><span class="sxs-lookup"><span data-stu-id="06c71-385">data-tag</span></span> |  <span data-ttu-id="06c71-386">[Тег заметки](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) в элементе span внутри элемента **li**.</span><span class="sxs-lookup"><span data-stu-id="06c71-386">A [note tag](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags) on a **span** in a li element.</span></span> |
| <span data-ttu-id="06c71-387">id</span><span class="sxs-lookup"><span data-stu-id="06c71-387">id</span></span> | <span data-ttu-id="06c71-388">Уникальный сгенерированный ИД элемента.</span><span class="sxs-lookup"><span data-stu-id="06c71-388">A unique ID for the group.</span></span> <span data-ttu-id="06c71-389">Возвращается [запросами GET к конечной точке *content* страницы](../api-reference/v1.0/api/page_get.md) при использовании параметра запроса `includeIDs=true`.</span><span class="sxs-lookup"><span data-stu-id="06c71-389">A unique, generated ID for the element. Returned by GET  requests to  a page's  *content* endpoint when the includeIDs=true`includeIDs=true` query option is used. Used for page updates.</span></span> <span data-ttu-id="06c71-390">Используется для [обновления содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="06c71-390">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="06c71-391">style</span><span class="sxs-lookup"><span data-stu-id="06c71-391">style</span></span> | <span data-ttu-id="06c71-392">Свойство **list-style-type** и свойство CSS [style](#styles) для элемента.</span><span class="sxs-lookup"><span data-stu-id="06c71-392">The CSS [style](#styles) properties of the element, and also:</span></span> <span data-ttu-id="06c71-393">В выходном HTML-коде параметры на уровне списка возвращаются в элементах списка.</span><span class="sxs-lookup"><span data-stu-id="06c71-393">In the output HTML, list-level settings are returned on list items.</span></span> <span data-ttu-id="06c71-394">Свойства по умолчанию не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="06c71-394">The following properties are not returned:</span></span> |
 

<span data-ttu-id="06c71-395">API OneNote в Microsoft Graph поддерживают следующие стили списков:</span><span class="sxs-lookup"><span data-stu-id="06c71-395">The OneNote APIs in Microsoft Graph support the following list styles:</span></span>

|<span data-ttu-id="06c71-396">Упорядоченный список</span><span class="sxs-lookup"><span data-stu-id="06c71-396">Ordered list</span></span>|<span data-ttu-id="06c71-397">Неупорядоченный список</span><span class="sxs-lookup"><span data-stu-id="06c71-397">Unordered list</span></span>|
|:------|:------|
| <span data-ttu-id="06c71-398">none</span><span class="sxs-lookup"><span data-stu-id="06c71-398">none</span></span> | <span data-ttu-id="06c71-399">none</span><span class="sxs-lookup"><span data-stu-id="06c71-399">none</span></span> |
| <span data-ttu-id="06c71-400">
decimal (по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="06c71-400">decimal (default)</span></span> | <span data-ttu-id="06c71-401">
disc (по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="06c71-401">disc (default)</span></span> |
| <span data-ttu-id="06c71-402">
lower-alpha</span><span class="sxs-lookup"><span data-stu-id="06c71-402">lower-alpha</span></span> | <span data-ttu-id="06c71-403">
circle</span><span class="sxs-lookup"><span data-stu-id="06c71-403">circle</span></span> |
| <span data-ttu-id="06c71-404">
lower-roman</span><span class="sxs-lookup"><span data-stu-id="06c71-404">lower-roman</span></span> | <span data-ttu-id="06c71-405">

square</span><span class="sxs-lookup"><span data-stu-id="06c71-405">square</span></span> |
| <span data-ttu-id="06c71-406">
upper-alpha</span><span class="sxs-lookup"><span data-stu-id="06c71-406">upper-alpha</span></span> | &nbsp; |
| <span data-ttu-id="06c71-407">upper-roman</span><span class="sxs-lookup"><span data-stu-id="06c71-407">upper-roman</span></span> | &nbsp; |
 
<span data-ttu-id="06c71-408">Вы можете применять глобальные стили для списка в элементе **ol** или **ul** входных данных HTML, но стили возвращаются в элементах **li**.</span><span class="sxs-lookup"><span data-stu-id="06c71-408">You can apply global styles for a list on the **ol** or **ul** element in the input HTML, but styles are returned on the **li** elements.</span></span>

<span data-ttu-id="06c71-409">**Однородный стиль списка**</span><span class="sxs-lookup"><span data-stu-id="06c71-409">**Homogenous list style**</span></span>

<span data-ttu-id="06c71-410">В этом примере показан входной HTML-код, который задает тип стиля списка в элементе **ol** и стили CSS для отдельных элементов списка.</span><span class="sxs-lookup"><span data-stu-id="06c71-410">This example shows input HTML that sets the list style type on the **ol** element and CSS styles on individual list items.</span></span>

```html
<ol style="list-style-type:upper-roman;color:blue">
    <li style="font-weight:bold">Jacksonville</li>
    <li style="text-decoration:line-through">Orlando</li>
    <li style="font-family:Courier">Naples</li>
</ol>
``` 

<span data-ttu-id="06c71-411">Ниже представлен выходной HTML-код.</span><span class="sxs-lookup"><span data-stu-id="06c71-411">This is the output HTML.</span></span> <span data-ttu-id="06c71-412">Обратите внимание, что стили возвращаются встроенными в отдельные элементы **li** или **span**.</span><span class="sxs-lookup"><span data-stu-id="06c71-412">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ol>
    <li style="list-style-type:upper-roman"><span style="color:blue;font-weight:bold">Jacksonville</span></li>
    <li style="list-style-type:upper-roman"><span style="color:blue;text-decoration:line-through">Orlando</span></li>
    <li style="list-style-type:upper-roman"><span style="font-family:Courier;color:blue">Naples</span></li>
</ol>
``` 

<span data-ttu-id="06c71-413">**Переменные стили списков**</span><span class="sxs-lookup"><span data-stu-id="06c71-413">**Variable list styles**</span></span>

<span data-ttu-id="06c71-414">В этом примере показан входной HTML-код, который задает разные типы стилей списков в элементах **li**.</span><span class="sxs-lookup"><span data-stu-id="06c71-414">This example shows input HTML that sets different list style types on the **li** elements.</span></span>

```html
<ul style="font-style:italic">
    <li style="list-style-type:square">square style</li>
    <li style="list-style-type:circle">circle style</li>
    <li style="list-style-type:disc">disc style (default)</li>
</ul>
``` 

<span data-ttu-id="06c71-415">Ниже представлен выходной HTML-код.</span><span class="sxs-lookup"><span data-stu-id="06c71-415">This is the output HTML.</span></span> <span data-ttu-id="06c71-416">Обратите внимание, что стили возвращаются встроенными в отдельные элементы **li** или **span**.</span><span class="sxs-lookup"><span data-stu-id="06c71-416">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ul>
    <li style="list-style-type:square"><span style="font-style:italic">square style</span></li>
    <li style="list-style-type:circle"><span style="font-style:italic">circle style</span></li>
    <li><span style="font-style:italic">disc style (default)</span></li>
</ul>
``` 


## <a name="tables"></a><span data-ttu-id="06c71-417">Таблицы</span><span class="sxs-lookup"><span data-stu-id="06c71-417">Tables</span></span>
<span data-ttu-id="06c71-418">Таблицы представляются как элементы **table**, которые могут содержать элементы **tr** и **td**.</span><span class="sxs-lookup"><span data-stu-id="06c71-418">Tables are represented as **table** elements that can contain **tr** and **td** elements. Nested tables are supported.</span></span> <span data-ttu-id="06c71-419">Поддерживаются вложенные таблицы.</span><span class="sxs-lookup"><span data-stu-id="06c71-419">Nested tables are supported.</span></span>

<span data-ttu-id="06c71-420">Входной и выходной HTML-код для таблиц может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="06c71-420">Lists and list items can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="06c71-421">API OneNote не поддерживают атрибуты **rowspan** и **colspan**.</span><span class="sxs-lookup"><span data-stu-id="06c71-421">The OneNote APIs do not support **rowspan** or **colspan** attributes.</span></span> 

<span data-ttu-id="06c71-422">**Входные атрибуты**</span><span class="sxs-lookup"><span data-stu-id="06c71-422">**Input attributes**</span></span>

|<span data-ttu-id="06c71-423">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="06c71-423">Input attribute</span></span>|<span data-ttu-id="06c71-424">Описание</span><span class="sxs-lookup"><span data-stu-id="06c71-424">Description</span></span>|
|:------|:------|
| <span data-ttu-id="06c71-425">data-id</span><span class="sxs-lookup"><span data-stu-id="06c71-425">data-id</span></span> | <span data-ttu-id="06c71-426">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="06c71-426">A reference for the element.</span></span> <span data-ttu-id="06c71-427">Используется для [обновления содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="06c71-427">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="06c71-428">style</span><span class="sxs-lookup"><span data-stu-id="06c71-428">style</span></span> | <span data-ttu-id="06c71-429">Свойства CSS [style](#styles) для элемента, а также:</span><span class="sxs-lookup"><span data-stu-id="06c71-429">The CSS [style](#styles) properties of the element, and also:</span></span><br/> <span data-ttu-id="06c71-430">- **border**.</span><span class="sxs-lookup"><span data-stu-id="06c71-430">Border</span></span> <span data-ttu-id="06c71-431">Допустимые значения — 0px и 1px.</span><span class="sxs-lookup"><span data-stu-id="06c71-431">border. Can be either 0px or 1px.</span></span><br /> <span data-ttu-id="06c71-432">- **width**.</span><span class="sxs-lookup"><span data-stu-id="06c71-432">width</span></span> <span data-ttu-id="06c71-433">Поддерживается в элементах **table** и **td** как количество пикселей или процент от ширины страницы.</span><span class="sxs-lookup"><span data-stu-id="06c71-433">**width**. Supported by **table** and td as pixels or percentage of page width. Example: width="100px" or width="60%"</span></span><br /><span data-ttu-id="06c71-434">Пример: `width="100px"` или `width="60%"`</span><span class="sxs-lookup"><span data-stu-id="06c71-434">Example: `width="100px"` or `width="60%"`</span></span> |
 

<span data-ttu-id="06c71-435">**Выходные атрибуты**</span><span class="sxs-lookup"><span data-stu-id="06c71-435">**Output attributes**</span></span>

|<span data-ttu-id="06c71-436">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="06c71-436">Output attribute</span></span>|<span data-ttu-id="06c71-437">Описание</span><span class="sxs-lookup"><span data-stu-id="06c71-437">Description</span></span>|
|:------|:------|
| <span data-ttu-id="06c71-438">data-id</span><span class="sxs-lookup"><span data-stu-id="06c71-438">data-id</span></span> | <span data-ttu-id="06c71-439">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="06c71-439">A reference for the element.</span></span> <span data-ttu-id="06c71-440">Используется для [обновления содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="06c71-440">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="06c71-441">id</span><span class="sxs-lookup"><span data-stu-id="06c71-441">id</span></span> | <span data-ttu-id="06c71-442">Уникальный сгенерированный ИД элемента.</span><span class="sxs-lookup"><span data-stu-id="06c71-442">A unique ID for the group.</span></span> <span data-ttu-id="06c71-443">Возвращается [запросами GET к конечной точке *content* страницы](../api-reference/v1.0/api/page_get.md) при использовании параметра запроса `includeIDs=true`.</span><span class="sxs-lookup"><span data-stu-id="06c71-443">A unique, generated ID for the element. Returned by GET  requests to  a page's  *content* endpoint when the includeIDs=true`includeIDs=true` query option is used. Used for page updates.</span></span> <span data-ttu-id="06c71-444">Используется для [обновления содержимого страницы](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="06c71-444">Used to [update page content](../api-reference/v1.0/api/page_update.md).</span></span> |
| <span data-ttu-id="06c71-445">style</span><span class="sxs-lookup"><span data-stu-id="06c71-445">style</span></span> | <span data-ttu-id="06c71-446">Свойства CSS [style](#styles) для элемента.</span><span class="sxs-lookup"><span data-stu-id="06c71-446">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="06c71-447">В приведенных ниже примерах показан входной HTML-код, где используются разные способы определения стилей для таблиц, и возвращаемый выходной HTML-код.</span><span class="sxs-lookup"><span data-stu-id="06c71-447">The following examples show input HTML that uses different ways to define styles on tables and the output HTML that's returned.</span></span>

<span data-ttu-id="06c71-448">**Входной HTML-код** с необязательными параметрами на разных уровнях.</span><span class="sxs-lookup"><span data-stu-id="06c71-448">**Input HTML** with optional settings at different levels.</span></span>

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
 
<span data-ttu-id="06c71-449">**Выходной HTML-код** со стилями CSS, которые возвращаются встроенными в элементы **td**.</span><span class="sxs-lookup"><span data-stu-id="06c71-449">**Output HTML** with CSS styles returned inline on the **td** elements.</span></span>

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


## <a name="styles"></a><span data-ttu-id="06c71-450">Стили</span><span class="sxs-lookup"><span data-stu-id="06c71-450">Styles</span></span>
<span data-ttu-id="06c71-451">API OneNote в Microsoft Graph поддерживают перечисленные ниже встроенные свойства CSS **style** для элементов основного текста страницы, например **body**, **div**, **p**, **li** и **span**.</span><span class="sxs-lookup"><span data-stu-id="06c71-451">The onnvshort API supports the following inline CSS style properties for elements in the page body, such as body, div, p, li, and span.</span></span>

|<span data-ttu-id="06c71-452">Свойство</span><span class="sxs-lookup"><span data-stu-id="06c71-452">Property</span></span>|<span data-ttu-id="06c71-453">Пример</span><span class="sxs-lookup"><span data-stu-id="06c71-453">Example</span></span>|
|:------|:------|
| <span data-ttu-id="06c71-454">background-color</span><span class="sxs-lookup"><span data-stu-id="06c71-454">background-color</span></span> | <span data-ttu-id="06c71-455">`style="background-color:#66cc66"` (по умолчанию задан белый цвет)</span><span class="sxs-lookup"><span data-stu-id="06c71-455">style="background-color:#66cc66"`style="background-color:#66cc66"` (defaults to  white)</span></span><br /><span data-ttu-id="06c71-456">Поддерживаются как шестнадцатеричный формат, так и именованные цвета.</span><span class="sxs-lookup"><span data-stu-id="06c71-456">Both hexadecimal format and named colors are supported.</span></span> |
| <span data-ttu-id="06c71-457">color</span><span class="sxs-lookup"><span data-stu-id="06c71-457">color</span></span> | <span data-ttu-id="06c71-458">`style="color:#ffffff"` (по умолчанию задан черный цвет)</span><span class="sxs-lookup"><span data-stu-id="06c71-458">style="color:#ffffff"`style="color:#ffffff"` (defaults to black)</span></span> |
| <span data-ttu-id="06c71-459">font-family</span><span class="sxs-lookup"><span data-stu-id="06c71-459">font-family</span></span> | <span data-ttu-id="06c71-460">`style="font-family:Courier"` (по умолчанию задан шрифт Calibri)</span><span class="sxs-lookup"><span data-stu-id="06c71-460">style="font-family:Courier"`style="font-family:Courier"` (defaults to Calibri)</span></span> |
| <span data-ttu-id="06c71-461">font-size</span><span class="sxs-lookup"><span data-stu-id="06c71-461">font-size</span></span> | <span data-ttu-id="06c71-462">`style="font-size:10pt"` (по умолчанию задан размер 11 точек)</span><span class="sxs-lookup"><span data-stu-id="06c71-462">style="font-size:10pt"`style="font-size:10pt"` (defaults to 11pt)</span></span><br /><span data-ttu-id="06c71-463">API принимают размер шрифта в единицах *pt* или *px*, но единицы *px* преобразуются в *pt*.</span><span class="sxs-lookup"><span data-stu-id="06c71-463">The APIs accept font size in *pt* or *px*, but converts *px* to *pt*.</span></span> <span data-ttu-id="06c71-464">Десятичные значения округляются до ближайшего значения n,0 или n,5 точек.</span><span class="sxs-lookup"><span data-stu-id="06c71-464">The onnvshort API accepts font size in pt or px, but converts px to pt. Decimal values are rounded to the nearest n.0pt or n.5pt.</span></span> |
| <span data-ttu-id="06c71-465">font-style</span><span class="sxs-lookup"><span data-stu-id="06c71-465">font-style</span></span> | <span data-ttu-id="06c71-466">`style="font-style:italic"` (обычный или только курсив)</span><span class="sxs-lookup"><span data-stu-id="06c71-466">style="font-style:italic"`style="font-style:italic"` (normal or italic only)</span></span> |
| <span data-ttu-id="06c71-467">font-weight</span><span class="sxs-lookup"><span data-stu-id="06c71-467">font-weight</span></span> | <span data-ttu-id="06c71-468">`style="font-weight:bold"` (обычный или только полужирный)</span><span class="sxs-lookup"><span data-stu-id="06c71-468">style="font-weight:bold"`style="font-weight:bold"` (normal or bold only)</span></span> |
| <span data-ttu-id="06c71-469">strike-through</span><span class="sxs-lookup"><span data-stu-id="06c71-469">strike-through</span></span> | `style="text-decoration:line-through"` |
| <span data-ttu-id="06c71-470">text-align</span><span class="sxs-lookup"><span data-stu-id="06c71-470">text-align</span></span> | <span data-ttu-id="06c71-471">`style="text-align:center"` (только для блочных элементов)</span><span class="sxs-lookup"><span data-stu-id="06c71-471">style="text-align:center"`style="text-align:center"` (for block elements only)</span></span> |
| <span data-ttu-id="06c71-472">text-decoration</span><span class="sxs-lookup"><span data-stu-id="06c71-472">text-decoration</span></span> | <span data-ttu-id="06c71-473">`style="text-decoration:underline"` (без оформления или только подчеркивание)</span><span class="sxs-lookup"><span data-stu-id="06c71-473">style="text-decoration:underline"`style="text-decoration:underline"` (none or underline only)</span></span> |
 

<span data-ttu-id="06c71-474">Кроме того, поддерживаются следующие встроенные стили знаков:</span><span class="sxs-lookup"><span data-stu-id="06c71-474">The following inline character styles and are also supported:</span></span>

<table id="simpletable">
<tr>
<td id="simplecell"><span data-ttu-id="06c71-475">&lt;b&gt;</span><span class="sxs-lookup"><span data-stu-id="06c71-475">b.</span></span></td>
<td id="simplecell"><span data-ttu-id="06c71-476">&lt;i&gt;</span><span class="sxs-lookup"><span data-stu-id="06c71-476">I</span></span></td>
<td id="simplecell"><span data-ttu-id="06c71-477">&lt;u&gt;</span><span class="sxs-lookup"><span data-stu-id="06c71-477">U</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="06c71-478">&lt;em&gt;</span><span class="sxs-lookup"><span data-stu-id="06c71-478">&lt;em&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="06c71-479">&lt;strong&gt;</span><span class="sxs-lookup"><span data-stu-id="06c71-479">&lt;strong&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="06c71-480">&lt;strike&gt;</span><span class="sxs-lookup"><span data-stu-id="06c71-480">&lt;strike&gt;</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="06c71-481">&lt;sup&gt;</span><span class="sxs-lookup"><span data-stu-id="06c71-481">&lt;sup&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="06c71-482">&lt;sub&gt;</span><span class="sxs-lookup"><span data-stu-id="06c71-482">&lt;Sub&gt;</span></span></td>
<td id="simplecell"><span data-ttu-id="06c71-483">&lt;del&gt;</span><span class="sxs-lookup"><span data-stu-id="06c71-483">&lt;del&gt;</span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="06c71-484">&lt;cite&gt;</span><span class="sxs-lookup"><span data-stu-id="06c71-484">&lt;cite&gt;</span></span></td>
<td id="simplecell">&nbsp;</td>
<td id="simplecell">&nbsp;</td>
</tr>
</table>

 
## <a name="input-and-output-html-example"></a><span data-ttu-id="06c71-485">Пример входного и выходного HTML-кода</span><span class="sxs-lookup"><span data-stu-id="06c71-485">Input and output HTML example</span></span>
<span data-ttu-id="06c71-486">На приведенном ниже рисунке показана простая страница, созданная с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="06c71-486">The following image shows a simple page that was created with the onnvshort API.</span></span>

![Изображение страницы OneNote с учебными заметками по материалам из Википедии](images/onenote-sample-image.png)

<span data-ttu-id="06c71-488">Ниже показан входной HTML-код, отправляемый в тексте сообщения для создания страницы.</span><span class="sxs-lookup"><span data-stu-id="06c71-488">This is the input HTML that was sent in the request body to create the page.</span></span>

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

<span data-ttu-id="06c71-489">Ниже показан выходной HTML-код, который Microsoft Graph возвращает при [получении содержимого страницы](../api-reference/v1.0/api/page_get.md).</span><span class="sxs-lookup"><span data-stu-id="06c71-489">This is the output HTML that the onnvshort API returns when you get the page content.</span></span>

><span data-ttu-id="06c71-490">**Примечание.** При [создании страницы](../api-reference/v1.0/api/section_post_pages.md) или [получении метаданных страницы](../api-reference/v1.0/api/page_get.md) API возвращает URL-адрес конечной точки *content* для страницы в свойстве **contentUrl**.</span><span class="sxs-lookup"><span data-stu-id="06c71-490">**Note:** When you [create a page](../api-reference/v1.0/api/section_post_pages.md) or [get page metadata](../api-reference/v1.0/api/page_get.md), the API returns the *content* endpoint URL of the page in the **contentUrl** property.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="06c71-491">См. также</span><span class="sxs-lookup"><span data-stu-id="06c71-491">See also</span></span>

- [<span data-ttu-id="06c71-492">Получение содержимого и структуры OneNote</span><span class="sxs-lookup"><span data-stu-id="06c71-492">Get OneNote content and structure</span></span>](../api-reference/v1.0/api/page_get.md)
- [<span data-ttu-id="06c71-493">Создание страниц OneNote</span><span class="sxs-lookup"><span data-stu-id="06c71-493">Create OneNote pages</span></span>](../api-reference/v1.0/api/section_post_pages.md)
- [<span data-ttu-id="06c71-494">Обновление содержимого страницы OneNote</span><span class="sxs-lookup"><span data-stu-id="06c71-494">Update page content</span></span>](../api-reference/v1.0/api/page_update.md)
- [<span data-ttu-id="06c71-495">Добавление изображений и файлов</span><span class="sxs-lookup"><span data-stu-id="06c71-495">Add images and files</span></span>](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags)
