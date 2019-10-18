---
title: Входной и выходной HTML-код на страницах OneNote
description: 'HTML-код, определяющий содержимое и структуру страницы при создании или обновлении страницы OneNote, называется *входным HTML-кодом*. '
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: fcb4a8127b633ba309212a7160c9e5548836466c
ms.sourcegitcommit: 6720736406f21e40914b27ba28387adedf97fa56
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2019
ms.locfileid: "35639222"
---
# <a name="input-and-output-html-in-onenote-pages"></a><span data-ttu-id="b4742-103">Входной и выходной HTML-код на страницах OneNote</span><span class="sxs-lookup"><span data-stu-id="b4742-103">Input and output HTML in OneNote pages</span></span>

<span data-ttu-id="b4742-104">HTML-код, определяющий содержимое и структуру страницы при [создании](onenote-create-page.md) или [обновлении](onenote-update-page.md) страницы OneNote, называется *входным HTML-кодом*.</span><span class="sxs-lookup"><span data-stu-id="b4742-104">The HTML that defines the page content and structure when you [create](onenote-create-page.md) or [update](onenote-update-page.md) a OneNote page is called *input HTML*.</span></span> 

<span data-ttu-id="b4742-105">HTML-код, возвращаемый при [получении содержимого страницы](onenote-get-content.md), называется *выходным HTML-кодом*.</span><span class="sxs-lookup"><span data-stu-id="b4742-105">The HTML that's returned when you [get page content](onenote-get-content.md) is called *output HTML*.</span></span> <span data-ttu-id="b4742-106">Выходной HTML-код не совпадает со входным.</span><span class="sxs-lookup"><span data-stu-id="b4742-106">Output HTML won't be the same as input HTML.</span></span>

<span data-ttu-id="b4742-107">API OneNote в Microsoft Graph сохраняют семантическое содержимое и базовую структуру входного HTML-кода, но преобразовывают ее в набор [поддерживаемых элементов HTML и свойств CSS](onenote-create-page.md#supported-html-and-css-for-onenote-pages).</span><span class="sxs-lookup"><span data-stu-id="b4742-107">The OneNote APIs in Microsoft Graph preserve the semantic content and basic structure of the input HTML, but convert it to a set of [supported HTML elements and CSS properties](onenote-create-page.md#supported-html-and-css-for-onenote-pages).</span></span> <span data-ttu-id="b4742-108">API также добавляют настраиваемые атрибуты, поддерживающие функции OneNote.</span><span class="sxs-lookup"><span data-stu-id="b4742-108">The APIs also add custom attributes that support OneNote features.</span></span>
 
<span data-ttu-id="b4742-109">В этой статье описываются основные элементы и атрибуты входного и выходного HTML-кода.</span><span class="sxs-lookup"><span data-stu-id="b4742-109">This article describes the principal elements and attributes of input and output HTML.</span></span> <span data-ttu-id="b4742-110">Разбираться во входном HTML-коде полезно при создании и обновлении содержимого страницы, а в выходном — при анализе возвращаемого содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="b4742-110">It can be helpful to understand input HTML when you're creating or updating page content, and output HTML when you're parsing returned page content.</span></span> 

## <a name="body-element"></a><span data-ttu-id="b4742-111">Элемент body</span><span class="sxs-lookup"><span data-stu-id="b4742-111">body element</span></span>

<span data-ttu-id="b4742-112">HTML-содержимое в тексте страницы представляет ее содержимое и структуру, в том числе ресурсы изображений и файлов.</span><span class="sxs-lookup"><span data-stu-id="b4742-112">The HTML content in the page body represents the page content and structure, including image and file resources.</span></span> <span data-ttu-id="b4742-113">Входной и выходной HTML-код для элемента **body** может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="b4742-113">The **body** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="b4742-114">Входные атрибуты</span><span class="sxs-lookup"><span data-stu-id="b4742-114">Input attributes</span></span>

|<span data-ttu-id="b4742-115">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="b4742-115">Input attribute</span></span>|<span data-ttu-id="b4742-116">Описание</span><span class="sxs-lookup"><span data-stu-id="b4742-116">Description</span></span>|
|:------|:------|
| <span data-ttu-id="b4742-117">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="b4742-117">data-absolute-enabled</span></span> | <span data-ttu-id="b4742-118">Указывает, поддерживают ли во входном тексте элементы с [абсолютным положением](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-118">Indicates whether the input body supports [absolute positioned](onenote-abs-pos.md) elements.</span></span> |
| <span data-ttu-id="b4742-119">style</span><span class="sxs-lookup"><span data-stu-id="b4742-119">style</span></span> | <p><span data-ttu-id="b4742-120">Свойства CSS [style](#styles) для основного текста.</span><span class="sxs-lookup"><span data-stu-id="b4742-120">The CSS [style](#styles) properties of the body.</span></span> <span data-ttu-id="b4742-121">В выходном HTML-коде входные параметры могут быть встроены в соответствующие дочерние элементы.</span><span class="sxs-lookup"><span data-stu-id="b4742-121">In the output HTML, input settings might be returned inline on appropriate child elements.</span></span></p><p><span data-ttu-id="b4742-122">В настоящее время цвет фона не поддерживается для элемента **body**.</span><span class="sxs-lookup"><span data-stu-id="b4742-122">Background color is not currently supported for the **body** element.</span></span></p> |
 

#### <a name="output-attributes"></a><span data-ttu-id="b4742-123">Выходные атрибуты</span><span class="sxs-lookup"><span data-stu-id="b4742-123">Output attributes</span></span>

|<span data-ttu-id="b4742-124">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="b4742-124">Output attribute</span></span>|<span data-ttu-id="b4742-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b4742-125">Description</span></span>|
|:------|:------|
| <span data-ttu-id="b4742-126">data-absolute-enabled</span><span class="sxs-lookup"><span data-stu-id="b4742-126">data-absolute-enabled</span></span> | <span data-ttu-id="b4742-127">Указывает, поддерживаются ли в тексте элементы с [абсолютным положением](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-127">Indicates whether the body supports [absolute positioned](onenote-abs-pos.md) elements.</span></span> <span data-ttu-id="b4742-128">В выходном HTML-коде всегда задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="b4742-128">Always **true** in output HTML.</span></span> |
| <span data-ttu-id="b4742-129">style</span><span class="sxs-lookup"><span data-stu-id="b4742-129">style</span></span> | <span data-ttu-id="b4742-130">Свойства **font-family** и **font-size** основного текста.</span><span class="sxs-lookup"><span data-stu-id="b4742-130">The **font-family** and **font-size** properties of the body.</span></span> |


## <a name="div-elements"></a><span data-ttu-id="b4742-131">Элементы div</span><span class="sxs-lookup"><span data-stu-id="b4742-131">div elements</span></span>

<span data-ttu-id="b4742-132">Элементы **div** содержат текст, изображения и другой контент.</span><span class="sxs-lookup"><span data-stu-id="b4742-132">**Div** elements contain text, images, and other content.</span></span> <span data-ttu-id="b4742-133">Входной и выходной HTML-код для элемента **div** может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="b4742-133">A **div** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="b4742-134">Входные атрибуты</span><span class="sxs-lookup"><span data-stu-id="b4742-134">Input attributes</span></span>

|<span data-ttu-id="b4742-135">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="b4742-135">Input attribute</span></span>|<span data-ttu-id="b4742-136">Описание</span><span class="sxs-lookup"><span data-stu-id="b4742-136">Description</span></span>|
|:------|:------|
| <span data-ttu-id="b4742-137">data-id</span><span class="sxs-lookup"><span data-stu-id="b4742-137">data-id</span></span> | <span data-ttu-id="b4742-138">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="b4742-138">A reference for the element.</span></span><br/><br/><span data-ttu-id="b4742-139">Используется для [обновления содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-139">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="b4742-140">data-render-fallback</span><span class="sxs-lookup"><span data-stu-id="b4742-140">data-render-fallback</span></span> | <span data-ttu-id="b4742-141">Резервное действие в случае ошибки [извлечения](onenote-extract-data.md): **render** (по умолчанию) или **none**</span><span class="sxs-lookup"><span data-stu-id="b4742-141">The fallback action if the [extraction](onenote-extract-data.md) fails: **render** (default) or **none**</span></span> |
| <span data-ttu-id="b4742-142">data-render-method</span><span class="sxs-lookup"><span data-stu-id="b4742-142">data-render-method</span></span> | <span data-ttu-id="b4742-143">Выполняемый метод [извлечения](onenote-extract-data.md), например</span><span class="sxs-lookup"><span data-stu-id="b4742-143">The [extraction](onenote-extract-data.md) method to perform, for example:</span></span><br/><span data-ttu-id="b4742-144">`extract.businesscard` или `extract.recipe`</span><span class="sxs-lookup"><span data-stu-id="b4742-144">`extract.businesscard` or `extract.recipe`</span></span> |
| <span data-ttu-id="b4742-145">data-render-src</span><span class="sxs-lookup"><span data-stu-id="b4742-145">data-render-src</span></span> | <span data-ttu-id="b4742-146">Источник контента для [извлечения](onenote-extract-data.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-146">The content source for the [extraction](onenote-extract-data.md).</span></span> |
| <span data-ttu-id="b4742-147">style</span><span class="sxs-lookup"><span data-stu-id="b4742-147">style</span></span> | <span data-ttu-id="b4742-148">Свойства положения, размера, шрифта и цвета для элемента div:</span><span class="sxs-lookup"><span data-stu-id="b4742-148">The position, size, font, and color properties for the div:</span></span> <ul><li><span data-ttu-id="b4742-149">**position** (только значение **absolute**), **left**, **top** и **width** (высота элементов Div настраивается автоматически).</span><span class="sxs-lookup"><span data-stu-id="b4742-149">**position** (**absolute** only), **left**, **top**, and **width** (height is auto-configured for divs)</span></span><br/><br/><span data-ttu-id="b4742-150">Используется для создания элемента div с [абсолютным положением](onenote-abs-pos.md), только если он является непосредственным дочерним элементом основного текста, для которого задан атрибут `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="b4742-150">Used to create an [absolute positioned](onenote-abs-pos.md) div, only if the div is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="b4742-151">Пример: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="b4742-151">Example: `<div style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span></li><li><span data-ttu-id="b4742-p108">Свойства CSS [style](#styles) элемента. В выходных данных HTML эти значения возвращаются встроенными в соответствующие дочерние элементы.</span><span class="sxs-lookup"><span data-stu-id="b4742-p108">The CSS [style](#styles) properties of the element. In the output HTML, these values are returned inline on appropriate child elements.</span></span></li></ul> |
 

<span data-ttu-id="b4742-154">API OneNote в Microsoft Graph заключают все содержимое основного текста по крайней мере в один элемент div.</span><span class="sxs-lookup"><span data-stu-id="b4742-154">The OneNote APIs in Microsoft Graph wrap all body content in at least one div.</span></span> <span data-ttu-id="b4742-155">API создает разделитель по умолчанию (с атрибутом `data-id="_default"`) для содержимого основного текста, если:</span><span class="sxs-lookup"><span data-stu-id="b4742-155">The API creates a default div (attributed with `data-id="_default"`) to contain the body content if:</span></span>

- <span data-ttu-id="b4742-156">Входной атрибут **data-absolute-enabled** элемента body пропущен или для него задано значение **false**.</span><span class="sxs-lookup"><span data-stu-id="b4742-156">The input body element's **data-absolute-enabled** attribute is omitted or set to **false**.</span></span> <span data-ttu-id="b4742-157">В этом случае все содержимое основного текста помещается в разделитель по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b4742-157">In this case, all body content is put in the default div.</span></span>

- <span data-ttu-id="b4742-158">Для входного атрибута **data-absolute-enabled** элемента body задано значение **true**, но входной HTML-код содержит непосредственные дочерние элементы&nbsp;**div**, **img** или **object** без [абсолютного положения](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-158">The input body element's **data-absolute-enabled** attribute is **true**, but the input HTML contains direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements.</span></span> <span data-ttu-id="b4742-159">В этом случае непосредственные дочерние элементы &nbsp;**div**, **img** или **object** без [абсолютного положения](onenote-abs-pos.md) помещаются в элементы div по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b4742-159">In this case, direct children that aren't [absolute positioned](onenote-abs-pos.md)&nbsp;**div**, **img**, or **object** elements are put in the default div.</span></span>


#### <a name="output-attributes"></a><span data-ttu-id="b4742-160">Выходные атрибуты</span><span class="sxs-lookup"><span data-stu-id="b4742-160">Output attributes</span></span>

|<span data-ttu-id="b4742-161">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="b4742-161">Output attribute</span></span>|<span data-ttu-id="b4742-162">Описание</span><span class="sxs-lookup"><span data-stu-id="b4742-162">Description</span></span>|
|:------|:------|
| <span data-ttu-id="b4742-163">data-id</span><span class="sxs-lookup"><span data-stu-id="b4742-163">data-id</span></span> | <span data-ttu-id="b4742-164">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="b4742-164">A reference for the element.</span></span><br/><br/><span data-ttu-id="b4742-165">Используется для [обновления содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-165">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="b4742-166">id</span><span class="sxs-lookup"><span data-stu-id="b4742-166">id</span></span> | <span data-ttu-id="b4742-167">Уникальный сгенерированный ИД элемента.</span><span class="sxs-lookup"><span data-stu-id="b4742-167">A unique, generated ID for the element.</span></span> <span data-ttu-id="b4742-168">Возвращается [запросами GET к конечной точке *content* страницы](/graph/api/page-get?view=graph-rest-1.0) при использовании параметра запроса `includeIDs=true`.</span><span class="sxs-lookup"><span data-stu-id="b4742-168">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="b4742-169">Используется для [обновления содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-169">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="b4742-170">style</span><span class="sxs-lookup"><span data-stu-id="b4742-170">style</span></span> | <span data-ttu-id="b4742-171">Свойства позиции и размера разделителя.</span><span class="sxs-lookup"><span data-stu-id="b4742-171">The position and size properties of the div.</span></span> |
 
### <a name="non-contributing-divs"></a><span data-ttu-id="b4742-172">Вспомогательные разделители</span><span class="sxs-lookup"><span data-stu-id="b4742-172">Non-contributing divs</span></span>

<span data-ttu-id="b4742-173">Если элемент **div** во входных данных HTML не входит в структуру страницы и не переносит сведения, используемые приложением OneNote, API перемещает содержимое разделителя в родительский или используемый по умолчанию разделитель.</span><span class="sxs-lookup"><span data-stu-id="b4742-173">When a **div** element in the input HTML does not contribute to the page structure or carry information that OneNote uses, the API moves the div's content into the parent or default div.</span></span> <span data-ttu-id="b4742-174">Этот процесс показан в приведенных ниже примерах.</span><span class="sxs-lookup"><span data-stu-id="b4742-174">This is illustrated in the following examples.</span></span>

#### <a name="input-html"></a><span data-ttu-id="b4742-175">Входной HTML-код</span><span class="sxs-lookup"><span data-stu-id="b4742-175">Input HTML</span></span>

<span data-ttu-id="b4742-176">Содержит вспомогательный вложенный разделитель.</span><span class="sxs-lookup"><span data-stu-id="b4742-176">Contains a non-contributing, nested div.</span></span>

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

#### <a name="output-html"></a><span data-ttu-id="b4742-177">Выходной HTML-код</span><span class="sxs-lookup"><span data-stu-id="b4742-177">Output HTML</span></span>

> <span data-ttu-id="b4742-178">**Примечание.** Содержимое разделителя было перемещено в родительский разделитель, а вложенные теги `<div>` удалены.</span><span class="sxs-lookup"><span data-stu-id="b4742-178">**Note:** The div's content was moved to the parent div and the nested `<div>` tags have been removed.</span></span> <span data-ttu-id="b4742-179">Элемент div был бы сохранен, если бы в нем были определены какие-либо семантические сведения, такие как **data-id** (пример: `<div data-id="keep-me">`).</span><span class="sxs-lookup"><span data-stu-id="b4742-179">The div would have been preserved if it defined any semantic information, such as a **data-id** (example: `<div data-id="keep-me">`).</span></span>

```html
<html htmlns="https://www.w3.org/1999/xhtml" lang="en-US">
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


## <a name="img-elements"></a><span data-ttu-id="b4742-180">Элементы img</span><span class="sxs-lookup"><span data-stu-id="b4742-180">img elements</span></span>

<span data-ttu-id="b4742-181">Для представления изображений на страницах OneNote используются элементы **img**.</span><span class="sxs-lookup"><span data-stu-id="b4742-181">Images on OneNote pages are represented by **img** elements.</span></span> <span data-ttu-id="b4742-182">Входной и выходной HTML-код для элемента **img** может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="b4742-182">An **img** element can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="b4742-183">Входные атрибуты</span><span class="sxs-lookup"><span data-stu-id="b4742-183">Input attributes</span></span>

|<span data-ttu-id="b4742-184">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="b4742-184">Input attribute</span></span>|<span data-ttu-id="b4742-185">Описание</span><span class="sxs-lookup"><span data-stu-id="b4742-185">Description</span></span>|
|:------|:------|
| <span data-ttu-id="b4742-186">alt</span><span class="sxs-lookup"><span data-stu-id="b4742-186">alt</span></span> | <span data-ttu-id="b4742-187">Предоставленный замещающий текст для изображения.</span><span class="sxs-lookup"><span data-stu-id="b4742-187">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="b4742-188">data-id</span><span class="sxs-lookup"><span data-stu-id="b4742-188">data-id</span></span> | <span data-ttu-id="b4742-189">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="b4742-189">A reference for the element.</span></span><br/><br/><span data-ttu-id="b4742-190">Используется для [обновления содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-190">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="b4742-191">data-render-src</span><span class="sxs-lookup"><span data-stu-id="b4742-191">data-render-src</span></span> |<span data-ttu-id="b4742-192">Должно было задано значение **data-render-src** или **src**.</span><span class="sxs-lookup"><span data-stu-id="b4742-192">Either **data-render-src** or **src** is required.</span></span><br/><br/><span data-ttu-id="b4742-193">Веб-страница, которая будет отображаться в виде битового изображения на странице OneNote:</span><span class="sxs-lookup"><span data-stu-id="b4742-193">The webpage to render as a bit-mapped image on the OneNote page:</span></span><br/><br/> <span data-ttu-id="b4742-194">- `data-render-src="https://..."` для общедоступного URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="b4742-194">- `data-render-src="https://..."` for a public URL.</span></span><br/><br/> <span data-ttu-id="b4742-195">- `data-render-src="name:BlockName"` для части изображения в блоке Presentation [составного запроса](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span><span class="sxs-lookup"><span data-stu-id="b4742-195">- `data-render-src="name:BlockName"` for an image part in the "Presentation" block of a [multipart request](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span></span><br/><br/><span data-ttu-id="b4742-196">Этот метод удобно использовать, если веб-страница слишком сложна для достоверного отображения в OneNote или для использования страницы необходимы учетные данные.</span><span class="sxs-lookup"><span data-stu-id="b4742-196">This method is useful when the webpage is more complex than the OneNote page can faithfully render, or when the page requires login credentials.</span></span>|
| <span data-ttu-id="b4742-197">data-tag</span><span class="sxs-lookup"><span data-stu-id="b4742-197">data-tag</span></span> | <span data-ttu-id="b4742-198">[Тег заметки](onenote-note-tags.md) для элемента.</span><span class="sxs-lookup"><span data-stu-id="b4742-198">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="b4742-199">style</span><span class="sxs-lookup"><span data-stu-id="b4742-199">style</span></span> |<span data-ttu-id="b4742-200">Свойства положения и размера изображения: **position** (только **absolute**), **left**, **top**, **width** и **height**.</span><span class="sxs-lookup"><span data-stu-id="b4742-200">The position and size properties for the image: **position** (**absolute** only), **left**, **top**, **width**, and **height**.</span></span><br/><br/><span data-ttu-id="b4742-201">Размер можно задать для любого изображения.</span><span class="sxs-lookup"><span data-stu-id="b4742-201">Size can be set on any image.</span></span><br/><br/><span data-ttu-id="b4742-202">Свойства положения используются для создания изображения с [абсолютным положением](onenote-abs-pos.md), только если изображение является непосредственным дочерним элементом основного текста, для которого задан атрибут `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="b4742-202">Position properties are used to create an [absolute positioned](onenote-abs-pos.md) image, only if the image is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="b4742-203">Пример: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="b4742-203">Example: `<img style="position:absolute;width:360px;top:350px;left:300px" ... />`</span></span><br/><br/><span data-ttu-id="b4742-204">В выходном HTML-коде размеры изображения возвращаются по отдельности через атрибуты **width** и **height**.</span><span class="sxs-lookup"><span data-stu-id="b4742-204">In the output HTML, the image size is returned separately in **width** and **height** attributes.</span></span> |
| <span data-ttu-id="b4742-205">src</span><span class="sxs-lookup"><span data-stu-id="b4742-205">src</span></span> |<span data-ttu-id="b4742-206">Должно было задано значение **src** или **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="b4742-206">Either **src** or **data-render-src** is required.</span></span><br/><br/><span data-ttu-id="b4742-207">Изображение, отображаемое на странице OneNote:</span><span class="sxs-lookup"><span data-stu-id="b4742-207">The image to render on the OneNote page:</span></span><br/><br/><span data-ttu-id="b4742-208">- `src="https://..."`: URL-адрес общедоступного изображения в Интернете.</span><span class="sxs-lookup"><span data-stu-id="b4742-208">- `src="https://..."` for a URL to a publicly available image on the Internet.</span></span><br/><br/> <span data-ttu-id="b4742-209">- `src="name:BlockName"`: именованная часть составного запроса, представляющая изображение.</span><span class="sxs-lookup"><span data-stu-id="b4742-209">- `src="name:BlockName"` for a named part in a multipart request that represents the image.</span></span>|
| <span data-ttu-id="b4742-210">width, height</span><span class="sxs-lookup"><span data-stu-id="b4742-210">width, height</span></span> | <span data-ttu-id="b4742-211">Ширина и высота изображения в пикселях, но без обозначения px.</span><span class="sxs-lookup"><span data-stu-id="b4742-211">The width or height of the image, in pixels but without the px.</span></span> <span data-ttu-id="b4742-212">Пример: `width="400"`</span><span class="sxs-lookup"><span data-stu-id="b4742-212">Example: `width="400"`</span></span> |
 
> <span data-ttu-id="b4742-213">**Примечание.** API OneNote автоматически определяют тип входного изображения и возвращают его в качестве атрибута **data-fullres-src-type** в выходном HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="b4742-213">**Note:** The OneNote APIs automatically detect the input image type, and return it as the **data-fullres-src-type** in the output HTML.</span></span> <span data-ttu-id="b4742-214">API также возвращает тип оптимизированного изображения в атрибуте **data-src-type**.</span><span class="sxs-lookup"><span data-stu-id="b4742-214">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 

#### <a name="output-attributes"></a><span data-ttu-id="b4742-215">Выходные атрибуты</span><span class="sxs-lookup"><span data-stu-id="b4742-215">Output attributes</span></span>

|<span data-ttu-id="b4742-216">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="b4742-216">Output attribute</span></span>|<span data-ttu-id="b4742-217">Описание</span><span class="sxs-lookup"><span data-stu-id="b4742-217">Description</span></span>|
|:------|:------|
| <span data-ttu-id="b4742-218">alt</span><span class="sxs-lookup"><span data-stu-id="b4742-218">alt</span></span> | <span data-ttu-id="b4742-219">Предоставленный замещающий текст для изображения.</span><span class="sxs-lookup"><span data-stu-id="b4742-219">The supplied alt text for the image.</span></span> |
| <span data-ttu-id="b4742-220">data-id</span><span class="sxs-lookup"><span data-stu-id="b4742-220">data-id</span></span> | <span data-ttu-id="b4742-221">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="b4742-221">A reference for the element.</span></span><br/><br/><span data-ttu-id="b4742-222">Используется для [обновления содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-222">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="b4742-223">data-index</span><span class="sxs-lookup"><span data-stu-id="b4742-223">data-index</span></span> | <span data-ttu-id="b4742-p118">Положение изображения. Для поддержки [разделения изображений](#split-images).</span><span class="sxs-lookup"><span data-stu-id="b4742-p118">The position of the image. For [split image](#split-images) support.</span></span> |
| <span data-ttu-id="b4742-226">data-fullres-src</span><span class="sxs-lookup"><span data-stu-id="b4742-226">data-fullres-src</span></span> | <span data-ttu-id="b4742-227">Конечная точка версии изображения, которая была изначально внедрена на странице.</span><span class="sxs-lookup"><span data-stu-id="b4742-227">The endpoint for the version of the image resource that was originally embedded in the page.</span></span> |
| <span data-ttu-id="b4742-228">data-fullres-src-type</span><span class="sxs-lookup"><span data-stu-id="b4742-228">data-fullres-src-type</span></span> | <span data-ttu-id="b4742-229">Тип мультимедиа для ресурса **data-fullres-src**, например `image/png` или `image/jpeg`.</span><span class="sxs-lookup"><span data-stu-id="b4742-229">The media type of the **data-fullres-src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="b4742-230">data-options</span><span class="sxs-lookup"><span data-stu-id="b4742-230">data-options</span></span> | <span data-ttu-id="b4742-p119">Тип источника: **printout** для PDF-файлов или **splitimage** для всех остальных. Применяется только к [разделенным изображениям](#split-images), созданным с помощью атрибута **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="b4742-p119">The source type: **printout** for PDF files or **splitimage** for all others. Applies only to [split images](#split-images) created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="b4742-233">data-render-original-src</span><span class="sxs-lookup"><span data-stu-id="b4742-233">data-render-original-src</span></span> | <span data-ttu-id="b4742-234">Исходный URL-адрес источника изображения, если исходное изображение находится в общедоступной части Интернета и создано с использованием атрибута **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="b4742-234">The original source URL of the image, if the source image is from the public internet and was created with the **data-render-src** attribute.</span></span> |
| <span data-ttu-id="b4742-235">data-src-type</span><span class="sxs-lookup"><span data-stu-id="b4742-235">data-src-type</span></span> | <span data-ttu-id="b4742-236">Тип мультимедиа для ресурса **src**, например `image/png` или `image/jpeg`.</span><span class="sxs-lookup"><span data-stu-id="b4742-236">The media type of the **src** resource, for example: `image/png` or `image/jpeg`.</span></span> |
| <span data-ttu-id="b4742-237">data-tag</span><span class="sxs-lookup"><span data-stu-id="b4742-237">data-tag</span></span> | <span data-ttu-id="b4742-238">[Тег заметки](onenote-note-tags.md) для элемента.</span><span class="sxs-lookup"><span data-stu-id="b4742-238">A [note tag](onenote-note-tags.md) on the element.</span></span> |
| <span data-ttu-id="b4742-239">id</span><span class="sxs-lookup"><span data-stu-id="b4742-239">id</span></span> | <span data-ttu-id="b4742-240">Уникальный сгенерированный ИД элемента.</span><span class="sxs-lookup"><span data-stu-id="b4742-240">A unique, generated ID for the element.</span></span> <span data-ttu-id="b4742-241">Возвращается [запросами GET к конечной точке *content* страницы](/graph/api/page-get?view=graph-rest-1.0) при использовании параметра запроса `includeIDs=true`.</span><span class="sxs-lookup"><span data-stu-id="b4742-241">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="b4742-242">Используется для [обновления содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-242">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="b4742-243">src</span><span class="sxs-lookup"><span data-stu-id="b4742-243">src</span></span> | <span data-ttu-id="b4742-244">Конечная точка версии изображения, оптимизированного для веб-браузеров, а также мобильных телефонов и планшетов.</span><span class="sxs-lookup"><span data-stu-id="b4742-244">The endpoint for the version of the image resource that has been optimized for web browsers and mobile and tablet form factors.</span></span> |
| <span data-ttu-id="b4742-245">style</span><span class="sxs-lookup"><span data-stu-id="b4742-245">style</span></span> | <span data-ttu-id="b4742-246">Свойства позиции изображения.</span><span class="sxs-lookup"><span data-stu-id="b4742-246">The position properties of the image.</span></span> |
| <span data-ttu-id="b4742-247">width, height</span><span class="sxs-lookup"><span data-stu-id="b4742-247">width, height</span></span> | <span data-ttu-id="b4742-248">Ширина или высота изображения в пикселях.</span><span class="sxs-lookup"><span data-stu-id="b4742-248">The width or height of the image, in pixels.</span></span> |
 

### <a name="output-html-examples-for-images"></a><span data-ttu-id="b4742-249">Примеры выходного HTML-кода для изображений</span><span class="sxs-lookup"><span data-stu-id="b4742-249">Output HTML examples for images</span></span>

<span data-ttu-id="b4742-250">Выходные элементы **img** содержат конечные точки для ресурсов файлов изображений и типа изображения, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="b4742-250">Output **img** elements contain endpoints for image file resources and the image type, as shown below.</span></span> <span data-ttu-id="b4742-251">Вы можете отправлять отдельные [запросы GET к конечным точкам ресурсов изображений](/graph/api/resource-get?view=graph-rest-1.0), чтобы получать их двоичное содержимое.</span><span class="sxs-lookup"><span data-stu-id="b4742-251">You can make separate [GET requests to image resource endpoints](/graph/api/resource-get?view=graph-rest-1.0) to retrieve their binary contents.</span></span>

```html
<img 
    src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://graph.microsoft.com/v1.0/me/onenote/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

<span data-ttu-id="b4742-252">В приведенных ниже примерах показаны сведения, которые может содержать элемент **img** в выходном HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="b4742-252">The following examples show the information an **img** element might contain in the output HTML.</span></span>

#### <a name="image-with-web-ready-and-high-resolution-resources"></a><span data-ttu-id="b4742-253">Изображение с ресурсами высокого разрешения для Интернета</span><span class="sxs-lookup"><span data-stu-id="b4742-253">Image with web-ready and high resolution resources</span></span>

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

#### <a name="image-created-by-using-the-data-render-src-attribute"></a><span data-ttu-id="b4742-254">Изображение, созданное с использованием атрибута *data-render-src*</span><span class="sxs-lookup"><span data-stu-id="b4742-254">Image created by using the *data-render-src* attribute</span></span>

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

### <a name="split-images"></a><span data-ttu-id="b4742-255">Разделенные изображения</span><span class="sxs-lookup"><span data-stu-id="b4742-255">Split images</span></span>

<span data-ttu-id="b4742-256">Изображения, созданные с использованием атрибута **data-render-src** (из URL-адреса страницы или именованной части), могут быть разделены на несколько компонентов для повышения производительности и удобства отрисовки.</span><span class="sxs-lookup"><span data-stu-id="b4742-256">Images that are created using the **data-render-src** attribute (from a webpage URL or a named part) might be split into multiple component images for performance and rendering reasons.</span></span> <span data-ttu-id="b4742-257">Всем компонентам изображения назначается одно и то же значение **data-id**.</span><span class="sxs-lookup"><span data-stu-id="b4742-257">Component images are all assigned the same **data-id** value.</span></span> <span data-ttu-id="b4742-258">У каждого компонента изображения есть атрибут data-index с отсчетом от нуля, определяющий исходную вертикальную компоновку.</span><span class="sxs-lookup"><span data-stu-id="b4742-258">Each component image has a zero-based data-index attribute that defines the original vertical layout.</span></span>

#### <a name="split-image-with-three-component-images"></a><span data-ttu-id="b4742-259">Разделенное изображение с тремя компонентами</span><span class="sxs-lookup"><span data-stu-id="b4742-259">Split image with three component images</span></span>

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

<span data-ttu-id="b4742-260">Так как пользователи могут перемещать изображения на странице, индексы могут возвращаться в измененном порядке.</span><span class="sxs-lookup"><span data-stu-id="b4742-260">Because users can move the images on the page, the returned indexes might be out of order.</span></span> <span data-ttu-id="b4742-261">Сортировка должна выполняться сверху вниз, а затем слева направо (если возникнут конфликты при вертикальной сортировке).</span><span class="sxs-lookup"><span data-stu-id="b4742-261">Ordering should be in top to bottom y-order, and then left to right x-order if there are y-order conflicts.</span></span>

## <a name="iframe-elements"></a><span data-ttu-id="b4742-262">Элементы iframe</span><span class="sxs-lookup"><span data-stu-id="b4742-262">iframe elements</span></span>

<span data-ttu-id="b4742-263">Страницы OneNote могут содержать внедренные видео, представленные элементами **iframe**.</span><span class="sxs-lookup"><span data-stu-id="b4742-263">OneNote pages can contain embedded videos represented by **iframe** elements.</span></span> 

> <span data-ttu-id="b4742-264">**Примечание.** Вы также можете [вложить видеофайл с помощью элемента **object**](onenote-images-files.md#adding-files).</span><span class="sxs-lookup"><span data-stu-id="b4742-264">**Note:** You can also [attach a video file using an **object** element](onenote-images-files.md#adding-files).</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="b4742-265">Входные атрибуты</span><span class="sxs-lookup"><span data-stu-id="b4742-265">Input attributes</span></span>

|<span data-ttu-id="b4742-266">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="b4742-266">Input attribute</span></span>|<span data-ttu-id="b4742-267">Описание</span><span class="sxs-lookup"><span data-stu-id="b4742-267">Description</span></span>|
|:------|:------|
| <span data-ttu-id="b4742-268">data-original-src</span><span class="sxs-lookup"><span data-stu-id="b4742-268">data-original-src</span></span> | <span data-ttu-id="b4742-269">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4742-269">Required.</span></span> <span data-ttu-id="b4742-270">URL-адрес источника видео.</span><span class="sxs-lookup"><span data-stu-id="b4742-270">The URL of the video source.</span></span> <span data-ttu-id="b4742-271">См. [список поддерживаемых источников видео](onenote-images-files.md#adding-videos).</span><span class="sxs-lookup"><span data-stu-id="b4742-271">See the [list of supported video sources](onenote-images-files.md#adding-videos).</span></span> <br/><br/><span data-ttu-id="b4742-272">Пример: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="b4742-272">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span> |
| <span data-ttu-id="b4742-273">width, height</span><span class="sxs-lookup"><span data-stu-id="b4742-273">width, height</span></span> | <span data-ttu-id="b4742-274">Ширина или высота элемента iframe в пикселях.</span><span class="sxs-lookup"><span data-stu-id="b4742-274">The width or height of the iframe, in pixels.</span></span> <span data-ttu-id="b4742-275">Пример: `width=300`</span><span class="sxs-lookup"><span data-stu-id="b4742-275">Example: `width=300`</span></span> |

#### <a name="output-attributes"></a><span data-ttu-id="b4742-276">Выходные атрибуты</span><span class="sxs-lookup"><span data-stu-id="b4742-276">Output attributes</span></span>

|<span data-ttu-id="b4742-277">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="b4742-277">Output attribute</span></span>|<span data-ttu-id="b4742-278">Описание</span><span class="sxs-lookup"><span data-stu-id="b4742-278">Description</span></span>|
|:------|:------|
| <span data-ttu-id="b4742-279">data-original-src</span><span class="sxs-lookup"><span data-stu-id="b4742-279">data-original-src</span></span> | <span data-ttu-id="b4742-280">URL-адрес источника видео.</span><span class="sxs-lookup"><span data-stu-id="b4742-280">The URL of the video source.</span></span> |
| <span data-ttu-id="b4742-281">src</span><span class="sxs-lookup"><span data-stu-id="b4742-281">src</span></span> | <span data-ttu-id="b4742-282">Ссылка на видео, внедренное в страницу OneNote.</span><span class="sxs-lookup"><span data-stu-id="b4742-282">A link to the video that is embedded in the OneNote page.</span></span> |
| <span data-ttu-id="b4742-283">width, height</span><span class="sxs-lookup"><span data-stu-id="b4742-283">width, height</span></span> | <span data-ttu-id="b4742-284">Ширина или высота элемента iframe в пикселях.</span><span class="sxs-lookup"><span data-stu-id="b4742-284">The width or height of the iframe, in pixels.</span></span><br/><br/><span data-ttu-id="b4742-285">Пример: `width=300`</span><span class="sxs-lookup"><span data-stu-id="b4742-285">Example: `width=300`</span></span> |
 
### <a name="output-html-example-for-videos"></a><span data-ttu-id="b4742-286">Пример выходного HTML-кода для видео</span><span class="sxs-lookup"><span data-stu-id="b4742-286">Output HTML example for videos</span></span>

<span data-ttu-id="b4742-287">Выходные элементы **iframe** содержат конечные точки, ссылающиеся на исходную страницу и видео, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="b4742-287">Output **iframe** elements contain endpoints that link to the source page and video, as shown.</span></span> 

```html
<iframe 
    width="340" height="280" 
    data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" 
    src="https://www.youtube.com/embed/3Ztr44aKmQ8?feature=oembed&autoplay=true" />
``` 

## <a name="object-elements"></a><span data-ttu-id="b4742-288">Элементы object</span><span class="sxs-lookup"><span data-stu-id="b4742-288">object elements</span></span>

<span data-ttu-id="b4742-289">Страницы OneNote могут содержать вложения, представленные элементами **object**.</span><span class="sxs-lookup"><span data-stu-id="b4742-289">OneNote pages can contain file attachments represented by **object** elements.</span></span> <span data-ttu-id="b4742-290">Входной и выходной HTML-код для элемента **object** может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="b4742-290">An **object** element can contain the following attributes in the input and output HTML.</span></span>

> <span data-ttu-id="b4742-291">**Примечание.** API OneNote также может отображать содержимое файлов в виде изображений на странице, если файл отправлен как изображение и использует атрибут **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="b4742-291">**Note:** The OneNote APIs can also render file content as images in a page when the file is sent as an image and uses the **data-render-src** attribute.</span></span>
> <span data-ttu-id="b4742-292">Пример: `<img data-render-src="name:part-name" ... />`</span><span class="sxs-lookup"><span data-stu-id="b4742-292">Example: `<img data-render-src="name:part-name" ... />`</span></span>
 

#### <a name="input-attributes"></a><span data-ttu-id="b4742-293">Входные атрибуты</span><span class="sxs-lookup"><span data-stu-id="b4742-293">Input attributes</span></span>

|<span data-ttu-id="b4742-294">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="b4742-294">Input attribute</span></span>|<span data-ttu-id="b4742-295">Описание</span><span class="sxs-lookup"><span data-stu-id="b4742-295">Description</span></span>|
|:------|:------|
| <span data-ttu-id="b4742-296">data</span><span class="sxs-lookup"><span data-stu-id="b4742-296">data</span></span> | <span data-ttu-id="b4742-297">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4742-297">Required.</span></span> <span data-ttu-id="b4742-298">Имя части, которая представляет файл в [составном запросе](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span><span class="sxs-lookup"><span data-stu-id="b4742-298">The name of the part that represents the file in the [multipart request](/graph/api/section-post-pages?view=graph-rest-1.0#example).</span></span> |
| <span data-ttu-id="b4742-299">data-attachment</span><span class="sxs-lookup"><span data-stu-id="b4742-299">data-attachment</span></span> | <span data-ttu-id="b4742-p129">Обязательный параметр. Имя файла.</span><span class="sxs-lookup"><span data-stu-id="b4742-p129">Required. The file name.</span></span> |
| <span data-ttu-id="b4742-302">data-id</span><span class="sxs-lookup"><span data-stu-id="b4742-302">data-id</span></span> | <span data-ttu-id="b4742-303">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="b4742-303">A reference for the element.</span></span><br/><br/><span data-ttu-id="b4742-304">Используется для [обновления содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-304">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="b4742-305">style</span><span class="sxs-lookup"><span data-stu-id="b4742-305">style</span></span> | <span data-ttu-id="b4742-306">Свойства положения и размера объекта: **position** (только **absolute**), **left**, **top** и **width**.</span><span class="sxs-lookup"><span data-stu-id="b4742-306">The position and size properties for the object: **position** (**absolute** only), **left**, **top**, and **width**.</span></span><br/><br/><span data-ttu-id="b4742-307">Используется для создания объекта с [абсолютным положением](onenote-abs-pos.md), только если объект является непосредственным дочерним элементом основного текста, для которого задан атрибут `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="b4742-307">Used to create an [absolute positioned](onenote-abs-pos.md) object, only if the object is a direct child of the body when the body sets `data-absolute-enabled="true"`.</span></span><br/><br/><span data-ttu-id="b4742-308">Пример: `<object style="position:absolute;top:350px;left:300px" ... />`</span><span class="sxs-lookup"><span data-stu-id="b4742-308">Example: `<object style="position:absolute;top:350px;left:300px" ... />`</span></span> |
| <span data-ttu-id="b4742-309">type</span><span class="sxs-lookup"><span data-stu-id="b4742-309">type</span></span> | <span data-ttu-id="b4742-310">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4742-310">Required.</span></span><br/><br/><span data-ttu-id="b4742-311">Стандартный тип файла мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="b4742-311">The standard media file type.</span></span> <span data-ttu-id="b4742-312">Для файлов известных типов на странице OneNote отображается значок, связанный с типом файла.</span><span class="sxs-lookup"><span data-stu-id="b4742-312">Known file types display the icon associated with the file type on the OneNote page.</span></span> <span data-ttu-id="b4742-313">Для файлов неизвестных типов отображается универсальный значок файла.</span><span class="sxs-lookup"><span data-stu-id="b4742-313">Unknown file types display a generic file icon.</span></span> |
<!--todo: add link to known file types--> 

#### <a name="output-attributes"></a><span data-ttu-id="b4742-314">Выходные атрибуты</span><span class="sxs-lookup"><span data-stu-id="b4742-314">Output attributes</span></span>

|<span data-ttu-id="b4742-315">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="b4742-315">Output attribute</span></span>|<span data-ttu-id="b4742-316">Описание</span><span class="sxs-lookup"><span data-stu-id="b4742-316">Description</span></span>|
|:------|:------|
| <span data-ttu-id="b4742-317">data</span><span class="sxs-lookup"><span data-stu-id="b4742-317">data</span></span> | <span data-ttu-id="b4742-318">Конечная точка файлового ресурса.</span><span class="sxs-lookup"><span data-stu-id="b4742-318">The endpoint for the file resource.</span></span> |
| <span data-ttu-id="b4742-319">data-attachment</span><span class="sxs-lookup"><span data-stu-id="b4742-319">data-attachment</span></span> | <span data-ttu-id="b4742-320">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="b4742-320">The file name.</span></span> |
| <span data-ttu-id="b4742-321">data-id</span><span class="sxs-lookup"><span data-stu-id="b4742-321">data-id</span></span> | <span data-ttu-id="b4742-322">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="b4742-322">A reference for the element.</span></span><br/><br/><span data-ttu-id="b4742-323">Используется для [обновления содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-323">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="b4742-324">id</span><span class="sxs-lookup"><span data-stu-id="b4742-324">id</span></span> | <span data-ttu-id="b4742-325">Уникальный сгенерированный ИД элемента.</span><span class="sxs-lookup"><span data-stu-id="b4742-325">A unique, generated ID for the element.</span></span> <span data-ttu-id="b4742-326">Возвращается [запросами GET к конечной точке *content* страницы](/graph/api/page-get?view=graph-rest-1.0) при использовании параметра запроса `includeIDs=true`.</span><span class="sxs-lookup"><span data-stu-id="b4742-326">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="b4742-327">Используется для [обновления содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-327">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="b4742-328">style</span><span class="sxs-lookup"><span data-stu-id="b4742-328">style</span></span> | <span data-ttu-id="b4742-329">Свойства позиции объекта.</span><span class="sxs-lookup"><span data-stu-id="b4742-329">The position properties of the object.</span></span> |
| <span data-ttu-id="b4742-330">type</span><span class="sxs-lookup"><span data-stu-id="b4742-330">type</span></span> | <span data-ttu-id="b4742-331">Стандартный тип файла мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="b4742-331">The standard media file type.</span></span> |
 

#### <a name="output-html-example-for-objects"></a><span data-ttu-id="b4742-332">Пример выходных данных HTML для объектов</span><span class="sxs-lookup"><span data-stu-id="b4742-332">Output HTML example for objects</span></span>

<span data-ttu-id="b4742-333">Выходные элементы **object** содержат конечные точки, ссылающиеся на файловые ресурсы со страницы, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="b4742-333">Output **object** elements contain endpoints that link to the file resources in the page, as shown.</span></span> <span data-ttu-id="b4742-334">Вы можете отправлять отдельные [запросы GET к конечным точкам файловых ресурсов](/graph/api/resource-get?view=graph-rest-1.0), чтобы получать их двоичное содержимое.</span><span class="sxs-lookup"><span data-stu-id="b4742-334">You can make separate [GET requests to file resource endpoints](/graph/api/resource-get?view=graph-rest-1.0) to retrieve their binary contents.</span></span>

```html
<object
    data="https://graph.microsoft.com/v1.0/me/onenote/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" 
    [style="..."] />
``` 

## <a name="paragraphs-and-headings"></a><span data-ttu-id="b4742-335">Абзацы и заголовки</span><span class="sxs-lookup"><span data-stu-id="b4742-335">Paragraphs and headings</span></span>

<span data-ttu-id="b4742-336">Входной и выходной HTML-код для абзацев, заголовков и других текстовых контейнеров может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="b4742-336">Paragraphs, headings, and other text containers can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="b4742-337">Входные атрибуты</span><span class="sxs-lookup"><span data-stu-id="b4742-337">Input attributes</span></span>

|<span data-ttu-id="b4742-338">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="b4742-338">Input attribute</span></span>|<span data-ttu-id="b4742-339">Описание</span><span class="sxs-lookup"><span data-stu-id="b4742-339">Description</span></span>|
|:------|:------|
| <span data-ttu-id="b4742-340">data-id</span><span class="sxs-lookup"><span data-stu-id="b4742-340">data-id</span></span> | <span data-ttu-id="b4742-341">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="b4742-341">A reference for the element.</span></span><br/><br/><span data-ttu-id="b4742-342">Используется для [обновления содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-342">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="b4742-343">data-tag</span><span class="sxs-lookup"><span data-stu-id="b4742-343">data-tag</span></span> | <span data-ttu-id="b4742-344">[Тег заметки](onenote-note-tags.md) для элемента **p** или **h1** - **h6**.</span><span class="sxs-lookup"><span data-stu-id="b4742-344">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="b4742-345">style</span><span class="sxs-lookup"><span data-stu-id="b4742-345">style</span></span> | <span data-ttu-id="b4742-346">Свойства CSS [style](#styles) для элемента.</span><span class="sxs-lookup"><span data-stu-id="b4742-346">The CSS [style](#styles) properties of the element.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="b4742-347">Выходные атрибуты</span><span class="sxs-lookup"><span data-stu-id="b4742-347">Output attributes</span></span>

|<span data-ttu-id="b4742-348">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="b4742-348">Output attribute</span></span>|<span data-ttu-id="b4742-349">Описание</span><span class="sxs-lookup"><span data-stu-id="b4742-349">Description</span></span>|
|:------|:------|
| <span data-ttu-id="b4742-350">data-id</span><span class="sxs-lookup"><span data-stu-id="b4742-350">data-id</span></span> | <span data-ttu-id="b4742-351">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="b4742-351">A reference for the element.</span></span><br/><br/><span data-ttu-id="b4742-352">Используется для [обновления содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-352">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="b4742-353">data-tag</span><span class="sxs-lookup"><span data-stu-id="b4742-353">data-tag</span></span> | <span data-ttu-id="b4742-354">[Тег заметки](onenote-note-tags.md) для элемента **p** или **h1** - **h6**.</span><span class="sxs-lookup"><span data-stu-id="b4742-354">A [note tag](onenote-note-tags.md) on a **p** or **h1** - **h6** element.</span></span> |
| <span data-ttu-id="b4742-355">id</span><span class="sxs-lookup"><span data-stu-id="b4742-355">id</span></span> | <span data-ttu-id="b4742-356">Уникальный сгенерированный ИД элемента.</span><span class="sxs-lookup"><span data-stu-id="b4742-356">A unique, generated ID for the element.</span></span> <span data-ttu-id="b4742-357">Возвращается [запросами GET к конечной точке *content* страницы](/graph/api/page-get?view=graph-rest-1.0) при использовании параметра запроса `includeIDs=true`.</span><span class="sxs-lookup"><span data-stu-id="b4742-357">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="b4742-358">Используется для [обновления содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-358">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="b4742-359">style</span><span class="sxs-lookup"><span data-stu-id="b4742-359">style</span></span> | <span data-ttu-id="b4742-360">Свойства CSS [style](#styles) для элемента.</span><span class="sxs-lookup"><span data-stu-id="b4742-360">The CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="b4742-361">В выходном HTML-коде эти значения могут быть встроены в элементы **span** или соответствующие дочерние элементы.</span><span class="sxs-lookup"><span data-stu-id="b4742-361">In the output HTML, these values may be returned inline on appropriate child elements or on **span** elements.</span></span> |
 

<span data-ttu-id="b4742-362">В приведенных ниже примерах показан входной HTML-код, где используются разные способы определения стилей в текстовых контейнерах, и возвращаемый выходной HTML-код.</span><span class="sxs-lookup"><span data-stu-id="b4742-362">The following examples show input HTML that uses different ways to define styles on text containers and the output HTML that's returned.</span></span>

#### <a name="input-html-with-styles-defined-using-inline-character-styles-in-the-start-tag-and-within-a-span-element"></a><span data-ttu-id="b4742-363">Входной HTML-код со стилями, определенными с помощью встроенных стилей знаков, в начальном теге внутри элемента span.</span><span class="sxs-lookup"><span data-stu-id="b4742-363">Input HTML with styles defined using inline character styles, in the start tag, and within a span element.</span></span>

```html
<h1>Heading <i>One</i> text</h1>
<p style="font-size:8pt;color:green;font-family:Courier;text-align:center">Some text</p>
<p>Some <span  style="font-size:16px;color:#ff0000;font-family:Segoe UI Black">more</span> text</p>
``` 

#### <a name="output-html-with-the-i-character-style-and-the-font-settings-in-the-p-start-tag-returned-as-inline-css-styles-on-span-elements"></a><span data-ttu-id="b4742-364">Выходной HTML-код со стилем знака `<i>` и параметрами шрифта в начальном теге `<p>`, возвращаемыми в виде встроенных стилей CSS в элементах span.</span><span class="sxs-lookup"><span data-stu-id="b4742-364">Output HTML with the `<i>` character style and the font settings in the `<p>` start tag returned as inline CSS styles on span elements.</span></span>

```html
<h1 style="font-size:16pt;color:#1e4e79;margin-top:11pt;margin-bottom:11pt">Heading <span style="font-style:italic">One</span> text</h1>
<p style="text-align:center"><span style="font-family:Courier;font-size:8pt;color:green">Some text</span></p>
<p>Some <span style="font-family:Segoe UI Black;font-size:12pt;color:red">more</span> text</p>
``` 


## <a name="lists"></a><span data-ttu-id="b4742-365">Списки</span><span class="sxs-lookup"><span data-stu-id="b4742-365">Lists</span></span>

<span data-ttu-id="b4742-366">Для представления списков используются элементы **ol** или **ul**, которые содержат элементы списка, представленные элементами **li**.</span><span class="sxs-lookup"><span data-stu-id="b4742-366">Lists are represented as **ol** or **ul** elements that contain list items represented as **li** elements.</span></span>

<span data-ttu-id="b4742-367">Входной и выходной HTML-код списков и их элементов может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="b4742-367">Lists and list items can contain the following attributes in the input and output HTML.</span></span>

#### <a name="input-attributes"></a><span data-ttu-id="b4742-368">Входные атрибуты</span><span class="sxs-lookup"><span data-stu-id="b4742-368">Input attributes</span></span>

|<span data-ttu-id="b4742-369">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="b4742-369">Input attribute</span></span>|<span data-ttu-id="b4742-370">Описание</span><span class="sxs-lookup"><span data-stu-id="b4742-370">Description</span></span>|
|:------|:------|
| <span data-ttu-id="b4742-371">data-id</span><span class="sxs-lookup"><span data-stu-id="b4742-371">data-id</span></span> | <span data-ttu-id="b4742-372">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="b4742-372">A reference for the element.</span></span><br/><br/><span data-ttu-id="b4742-373">Используется для [обновления содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-373">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="b4742-374">data-tag</span><span class="sxs-lookup"><span data-stu-id="b4742-374">data-tag</span></span> | <span data-ttu-id="b4742-375">[Тег заметки](onenote-note-tags.md) в элементе **ul**, **ol** или **li**.</span><span class="sxs-lookup"><span data-stu-id="b4742-375">A [note tag](onenote-note-tags.md) on a **ul**, **ol**, or **li** element.</span></span> |
| <span data-ttu-id="b4742-376">style</span><span class="sxs-lookup"><span data-stu-id="b4742-376">style</span></span> | <span data-ttu-id="b4742-377">Свойство **list-style-type** и свойство CSS [style](#styles) для списка или его элемента.</span><span class="sxs-lookup"><span data-stu-id="b4742-377">The **list-style-type** and the CSS [style](#styles) properties for the list or list item.</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="b4742-378">Выходные атрибуты</span><span class="sxs-lookup"><span data-stu-id="b4742-378">Output attributes</span></span>

|<span data-ttu-id="b4742-379">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="b4742-379">Output attribute</span></span>|<span data-ttu-id="b4742-380">Описание</span><span class="sxs-lookup"><span data-stu-id="b4742-380">Description</span></span>|
|:------|:------|
| <span data-ttu-id="b4742-381">data-id</span><span class="sxs-lookup"><span data-stu-id="b4742-381">data-id</span></span> | <span data-ttu-id="b4742-382">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="b4742-382">A reference for the element.</span></span><br/><br/><span data-ttu-id="b4742-383">Используется для [обновления содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-383">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="b4742-384">data-tag</span><span class="sxs-lookup"><span data-stu-id="b4742-384">data-tag</span></span> |  <span data-ttu-id="b4742-385">[Тег заметки](onenote-note-tags.md) в элементе span внутри элемента **li**.</span><span class="sxs-lookup"><span data-stu-id="b4742-385">A [note tag](onenote-note-tags.md) on a span in an **li** element.</span></span> |
| <span data-ttu-id="b4742-386">id</span><span class="sxs-lookup"><span data-stu-id="b4742-386">id</span></span> | <span data-ttu-id="b4742-387">Уникальный сгенерированный ИД элемента.</span><span class="sxs-lookup"><span data-stu-id="b4742-387">A unique, generated ID for the element.</span></span> <span data-ttu-id="b4742-388">Возвращается [запросами GET к конечной точке *content* страницы](/graph/api/page-get?view=graph-rest-1.0) при использовании параметра запроса `includeIDs=true`.</span><span class="sxs-lookup"><span data-stu-id="b4742-388">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="b4742-389">Используется для [обновления содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-389">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="b4742-390">style</span><span class="sxs-lookup"><span data-stu-id="b4742-390">style</span></span> | <span data-ttu-id="b4742-391">Свойство **list-style-type** и свойство CSS [style](#styles) для элемента.</span><span class="sxs-lookup"><span data-stu-id="b4742-391">The **list-style-type** and CSS [style](#styles) properties of the element.</span></span> <span data-ttu-id="b4742-392">В выходном HTML-коде параметры на уровне списка возвращаются в элементах списка.</span><span class="sxs-lookup"><span data-stu-id="b4742-392">In the output HTML, list-level settings are returned on list items.</span></span> <span data-ttu-id="b4742-393">Свойства по умолчанию не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="b4742-393">Default properties are not returned.</span></span> |
 
### <a name="list-styles"></a><span data-ttu-id="b4742-394">Стили списков</span><span class="sxs-lookup"><span data-stu-id="b4742-394">List styles</span></span>

<span data-ttu-id="b4742-395">API OneNote в Microsoft Graph поддерживают следующие стили списков:</span><span class="sxs-lookup"><span data-stu-id="b4742-395">The OneNote APIs in Microsoft Graph support the following list styles:</span></span>

|<span data-ttu-id="b4742-396">Упорядоченный список</span><span class="sxs-lookup"><span data-stu-id="b4742-396">Ordered list</span></span>|<span data-ttu-id="b4742-397">Неупорядоченный список</span><span class="sxs-lookup"><span data-stu-id="b4742-397">Unordered list</span></span>|
|:------|:------|
| <span data-ttu-id="b4742-398">none</span><span class="sxs-lookup"><span data-stu-id="b4742-398">none</span></span> | <span data-ttu-id="b4742-399">none</span><span class="sxs-lookup"><span data-stu-id="b4742-399">none</span></span> |
| <span data-ttu-id="b4742-400">
decimal (по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="b4742-400">decimal (default)</span></span> | <span data-ttu-id="b4742-401">
disc (по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="b4742-401">disc (default)</span></span> |
| <span data-ttu-id="b4742-402">
lower-alpha</span><span class="sxs-lookup"><span data-stu-id="b4742-402">lower-alpha</span></span> | <span data-ttu-id="b4742-403">
circle</span><span class="sxs-lookup"><span data-stu-id="b4742-403">circle</span></span> |
| <span data-ttu-id="b4742-404">
lower-roman</span><span class="sxs-lookup"><span data-stu-id="b4742-404">lower-roman</span></span> | <span data-ttu-id="b4742-405">

square</span><span class="sxs-lookup"><span data-stu-id="b4742-405">square</span></span> |
| <span data-ttu-id="b4742-406">
upper-alpha</span><span class="sxs-lookup"><span data-stu-id="b4742-406">upper-alpha</span></span> | &nbsp; |
| <span data-ttu-id="b4742-407">upper-roman</span><span class="sxs-lookup"><span data-stu-id="b4742-407">upper-roman</span></span> | &nbsp; |
 
<span data-ttu-id="b4742-408">Вы можете применять глобальные стили для списка в элементе **ol** или **ul** входных данных HTML, но стили возвращаются в элементах **li**.</span><span class="sxs-lookup"><span data-stu-id="b4742-408">You can apply global styles for a list on the **ol** or **ul** element in the input HTML, but styles are returned on the **li** elements.</span></span>

#### <a name="homogenous-list-style"></a><span data-ttu-id="b4742-409">Однородный стиль списка</span><span class="sxs-lookup"><span data-stu-id="b4742-409">Homogenous list style</span></span>

<span data-ttu-id="b4742-410">В этом примере показан входной HTML-код, который задает тип стиля списка в элементе **ol** и стили CSS для отдельных элементов списка.</span><span class="sxs-lookup"><span data-stu-id="b4742-410">This example shows input HTML that sets the list style type on the **ol** element and CSS styles on individual list items.</span></span>

```html
<ol style="list-style-type:upper-roman;color:blue">
    <li style="font-weight:bold">Jacksonville</li>
    <li style="text-decoration:line-through">Orlando</li>
    <li style="font-family:Courier">Naples</li>
</ol>
``` 

<span data-ttu-id="b4742-p137">Ниже приводятся выходные данные HTML. Обратите внимание, что стили возвращаются встроенными в отдельные элементы **li** или **span**.</span><span class="sxs-lookup"><span data-stu-id="b4742-p137">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ol>
    <li style="list-style-type:upper-roman"><span style="color:blue;font-weight:bold">Jacksonville</span></li>
    <li style="list-style-type:upper-roman"><span style="color:blue;text-decoration:line-through">Orlando</span></li>
    <li style="list-style-type:upper-roman"><span style="font-family:Courier;color:blue">Naples</span></li>
</ol>
``` 

#### <a name="variable-list-styles"></a><span data-ttu-id="b4742-413">Переменные стили списков</span><span class="sxs-lookup"><span data-stu-id="b4742-413">Variable list styles</span></span>

<span data-ttu-id="b4742-414">В этом примере показан входной HTML-код, который задает разные типы стилей списков в элементах **li**.</span><span class="sxs-lookup"><span data-stu-id="b4742-414">This example shows input HTML that sets different list style types on the **li** elements.</span></span>

```html
<ul style="font-style:italic">
    <li style="list-style-type:square">square style</li>
    <li style="list-style-type:circle">circle style</li>
    <li style="list-style-type:disc">disc style (default)</li>
</ul>
``` 

<span data-ttu-id="b4742-p138">Ниже приводятся выходные данные HTML. Обратите внимание, что стили возвращаются встроенными в отдельные элементы **li** или **span**.</span><span class="sxs-lookup"><span data-stu-id="b4742-p138">This is the output HTML. Notice that styles are returned inline on the individual **li** or **span** elements.</span></span>

```html
<ul>
    <li style="list-style-type:square"><span style="font-style:italic">square style</span></li>
    <li style="list-style-type:circle"><span style="font-style:italic">circle style</span></li>
    <li><span style="font-style:italic">disc style (default)</span></li>
</ul>
``` 


## <a name="tables"></a><span data-ttu-id="b4742-417">таблицы;</span><span class="sxs-lookup"><span data-stu-id="b4742-417">Tables</span></span>

<span data-ttu-id="b4742-p139">Таблицы представляются как элементы **table**, которые могут содержать элементы **tr** и **td**. Поддерживаются вложенные таблицы.</span><span class="sxs-lookup"><span data-stu-id="b4742-p139">Tables are represented as **table** elements that can contain **tr** and **td** elements. Nested tables are supported.</span></span>

<span data-ttu-id="b4742-420">Входной и выходной HTML-код для таблиц может содержать перечисленные ниже атрибуты.</span><span class="sxs-lookup"><span data-stu-id="b4742-420">Tables can contain the following attributes in the input and output HTML.</span></span> <span data-ttu-id="b4742-421">API OneNote не поддерживают атрибуты **rowspan** и **colspan**.</span><span class="sxs-lookup"><span data-stu-id="b4742-421">The OneNote APIs do not support **rowspan** or **colspan** attributes.</span></span> 

#### <a name="input-attributes"></a><span data-ttu-id="b4742-422">Входные атрибуты</span><span class="sxs-lookup"><span data-stu-id="b4742-422">Input attributes</span></span>

|<span data-ttu-id="b4742-423">Входной атрибут</span><span class="sxs-lookup"><span data-stu-id="b4742-423">Input attribute</span></span>|<span data-ttu-id="b4742-424">Описание</span><span class="sxs-lookup"><span data-stu-id="b4742-424">Description</span></span>|
|:------|:------|
| <span data-ttu-id="b4742-425">data-id</span><span class="sxs-lookup"><span data-stu-id="b4742-425">data-id</span></span> | <span data-ttu-id="b4742-426">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="b4742-426">A reference for the element.</span></span><br/><br/><span data-ttu-id="b4742-427">Используется для [обновления содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-427">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="b4742-428">style</span><span class="sxs-lookup"><span data-stu-id="b4742-428">style</span></span> | <span data-ttu-id="b4742-429">Свойства CSS [style](#styles) для элемента, а также:</span><span class="sxs-lookup"><span data-stu-id="b4742-429">The CSS [style](#styles) properties of the element, and also:</span></span><br/> <span data-ttu-id="b4742-430">- **border**.</span><span class="sxs-lookup"><span data-stu-id="b4742-430">- **border**.</span></span> <span data-ttu-id="b4742-431">Допустимые значения — 0px и 1px.</span><span class="sxs-lookup"><span data-stu-id="b4742-431">Can be either 0px or 1px.</span></span><br/> <span data-ttu-id="b4742-432">- **width**.</span><span class="sxs-lookup"><span data-stu-id="b4742-432">- **width**.</span></span> <span data-ttu-id="b4742-433">Поддерживается в элементах **table** и **td** как количество пикселей или процент от ширины страницы.</span><span class="sxs-lookup"><span data-stu-id="b4742-433">Supported by **table** and **td** as pixels or percentage of page width.</span></span><br/><br/><span data-ttu-id="b4742-434">Пример: `width="100px"` или `width="60%"`</span><span class="sxs-lookup"><span data-stu-id="b4742-434">Example: `width="100px"` or `width="60%"`</span></span> |
 

#### <a name="output-attributes"></a><span data-ttu-id="b4742-435">Выходные атрибуты</span><span class="sxs-lookup"><span data-stu-id="b4742-435">Output attributes</span></span>

|<span data-ttu-id="b4742-436">Выходной атрибут</span><span class="sxs-lookup"><span data-stu-id="b4742-436">Output attribute</span></span>|<span data-ttu-id="b4742-437">Описание</span><span class="sxs-lookup"><span data-stu-id="b4742-437">Description</span></span>|
|:------|:------|
| <span data-ttu-id="b4742-438">data-id</span><span class="sxs-lookup"><span data-stu-id="b4742-438">data-id</span></span> | <span data-ttu-id="b4742-439">Ссылка на элемент.</span><span class="sxs-lookup"><span data-stu-id="b4742-439">A reference for the element.</span></span><br/><br/><span data-ttu-id="b4742-440">Используется для [обновления содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-440">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="b4742-441">id</span><span class="sxs-lookup"><span data-stu-id="b4742-441">id</span></span> | <span data-ttu-id="b4742-442">Уникальный сгенерированный ИД элемента.</span><span class="sxs-lookup"><span data-stu-id="b4742-442">A unique, generated ID for the element.</span></span> <span data-ttu-id="b4742-443">Возвращается [запросами GET к конечной точке *content* страницы](/graph/api/page-get?view=graph-rest-1.0) при использовании параметра запроса `includeIDs=true`.</span><span class="sxs-lookup"><span data-stu-id="b4742-443">Returned by [GET requests to a page's *content* endpoint](/graph/api/page-get?view=graph-rest-1.0) when the `includeIDs=true` query option is used.</span></span><br/><br/><span data-ttu-id="b4742-444">Используется для [обновления содержимого страницы](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-444">Used to [update page content](onenote-update-page.md).</span></span> |
| <span data-ttu-id="b4742-445">style</span><span class="sxs-lookup"><span data-stu-id="b4742-445">style</span></span> | <span data-ttu-id="b4742-446">Свойства CSS [style](#styles) для элемента.</span><span class="sxs-lookup"><span data-stu-id="b4742-446">The CSS [style](#styles) properties of the element.</span></span> |
 

<span data-ttu-id="b4742-447">В приведенных ниже примерах показан входной HTML-код, где используются разные способы определения стилей для таблиц, и возвращаемый выходной HTML-код.</span><span class="sxs-lookup"><span data-stu-id="b4742-447">The following examples show input HTML that uses different ways to define styles on tables and the output HTML that's returned.</span></span>

#### <a name="input-html-with-optional-settings-at-different-levels"></a><span data-ttu-id="b4742-448">Входной HTML-код с необязательными параметрами на разных уровнях.</span><span class="sxs-lookup"><span data-stu-id="b4742-448">Input HTML with optional settings at different levels</span></span>

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
 
#### <a name="output-html-with-css-styles-returned-inline-on-the-td-elements"></a><span data-ttu-id="b4742-449">Выходной HTML-код со стилями CSS, которые возвращаются встроенными в элементы td.</span><span class="sxs-lookup"><span data-stu-id="b4742-449">Output HTML with CSS styles returned inline on the td elements</span></span>

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


## <a name="styles"></a><span data-ttu-id="b4742-450">Стили</span><span class="sxs-lookup"><span data-stu-id="b4742-450">Styles</span></span>

<span data-ttu-id="b4742-451">API OneNote в Microsoft Graph поддерживают перечисленные ниже встроенные свойства CSS **style** для элементов основного текста страницы, например **body**, **div**, **p**, **li** и **span**.</span><span class="sxs-lookup"><span data-stu-id="b4742-451">OneNote APIs in Microsoft Graph support the following inline CSS **style** properties for elements in the page body, such as **body**, **div**, **p**, **li**, and **span**.</span></span>

|<span data-ttu-id="b4742-452">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4742-452">Property</span></span>|<span data-ttu-id="b4742-453">Пример</span><span class="sxs-lookup"><span data-stu-id="b4742-453">Example</span></span>|
|:------|:------|
| <span data-ttu-id="b4742-454">background-color</span><span class="sxs-lookup"><span data-stu-id="b4742-454">background-color</span></span> | <span data-ttu-id="b4742-455">`style="background-color:#66cc66"` (по умолчанию задан белый цвет)</span><span class="sxs-lookup"><span data-stu-id="b4742-455">`style="background-color:#66cc66"` (defaults to white)</span></span><br/><br/><span data-ttu-id="b4742-456">Поддерживаются как шестнадцатеричный формат, так и именованные цвета.</span><span class="sxs-lookup"><span data-stu-id="b4742-456">Both hexadecimal format and named colors are supported.</span></span> |
| <span data-ttu-id="b4742-457">color</span><span class="sxs-lookup"><span data-stu-id="b4742-457">color</span></span> | <span data-ttu-id="b4742-458">`style="color:#ffffff"` (по умолчанию задан черный цвет)</span><span class="sxs-lookup"><span data-stu-id="b4742-458">`style="color:#ffffff"` (defaults to black)</span></span> |
| <span data-ttu-id="b4742-459">font-family</span><span class="sxs-lookup"><span data-stu-id="b4742-459">font-family</span></span> | <span data-ttu-id="b4742-460">`style="font-family:Courier"` (по умолчанию задан шрифт Calibri)</span><span class="sxs-lookup"><span data-stu-id="b4742-460">`style="font-family:Courier"` (defaults to Calibri)</span></span> |
| <span data-ttu-id="b4742-461">font-size</span><span class="sxs-lookup"><span data-stu-id="b4742-461">font-size</span></span> | <span data-ttu-id="b4742-462">`style="font-size:10pt"` (по умолчанию задан размер 11 точек)</span><span class="sxs-lookup"><span data-stu-id="b4742-462">`style="font-size:10pt"` (defaults to 11pt)</span></span><br/><br/><span data-ttu-id="b4742-463">API принимают размер шрифта в единицах *pt* или *px*, но единицы *px* преобразуются в *pt*.</span><span class="sxs-lookup"><span data-stu-id="b4742-463">The APIs accept font size in *pt* or *px*, but converts *px* to *pt*.</span></span> <span data-ttu-id="b4742-464">Десятичные значения округляются до ближайшего значения n,0 или n,5 точек.</span><span class="sxs-lookup"><span data-stu-id="b4742-464">Decimal values are rounded to the nearest n.0pt or n.5pt.</span></span> |
| <span data-ttu-id="b4742-465">font-style</span><span class="sxs-lookup"><span data-stu-id="b4742-465">font-style</span></span> | <span data-ttu-id="b4742-466">`style="font-style:italic"` (обычный или только курсив)</span><span class="sxs-lookup"><span data-stu-id="b4742-466">`style="font-style:italic"` (normal or italic only)</span></span> |
| <span data-ttu-id="b4742-467">font-weight</span><span class="sxs-lookup"><span data-stu-id="b4742-467">font-weight</span></span> | <span data-ttu-id="b4742-468">`style="font-weight:bold"` (обычный или только полужирный)</span><span class="sxs-lookup"><span data-stu-id="b4742-468">`style="font-weight:bold"` (normal or bold only)</span></span> |
| <span data-ttu-id="b4742-469">strike-through</span><span class="sxs-lookup"><span data-stu-id="b4742-469">strike-through</span></span> | `style="text-decoration:line-through"` |
| <span data-ttu-id="b4742-470">text-align</span><span class="sxs-lookup"><span data-stu-id="b4742-470">text-align</span></span> | <span data-ttu-id="b4742-471">`style="text-align:center"` (только для блочных элементов)</span><span class="sxs-lookup"><span data-stu-id="b4742-471">`style="text-align:center"` (for block elements only)</span></span> |
| <span data-ttu-id="b4742-472">text-decoration</span><span class="sxs-lookup"><span data-stu-id="b4742-472">text-decoration</span></span> | <span data-ttu-id="b4742-473">`style="text-decoration:underline"` (без оформления или только подчеркивание)</span><span class="sxs-lookup"><span data-stu-id="b4742-473">`style="text-decoration:underline"` (none or underline only)</span></span> |
 

<span data-ttu-id="b4742-474">Кроме того, поддерживаются следующие встроенные стили знаков:</span><span class="sxs-lookup"><span data-stu-id="b4742-474">The following inline character styles are also supported:</span></span>

<table id="simpletable">
<tr>
<td id="simplecell"><span data-ttu-id="b4742-475"><b></span><span class="sxs-lookup"><span data-stu-id="b4742-475"><b></span></span></td>
<td id="simplecell"><span data-ttu-id="b4742-476"><i></span><span class="sxs-lookup"><span data-stu-id="b4742-476"><i></span></span></td>
<td id="simplecell"><span data-ttu-id="b4742-477"><u></span><span class="sxs-lookup"><span data-stu-id="b4742-477"><u></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="b4742-478"><em></span><span class="sxs-lookup"><span data-stu-id="b4742-478"><em></span></span></td>
<td id="simplecell"><span data-ttu-id="b4742-479"><strong></span><span class="sxs-lookup"><span data-stu-id="b4742-479"><strong></span></span></td>
<td id="simplecell"><span data-ttu-id="b4742-480"><strike></span><span class="sxs-lookup"><span data-stu-id="b4742-480"><strike></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="b4742-481"><sup></span><span class="sxs-lookup"><span data-stu-id="b4742-481"><sup></span></span></td>
<td id="simplecell"><span data-ttu-id="b4742-482"><sub></span><span class="sxs-lookup"><span data-stu-id="b4742-482"><sub></span></span></td>
<td id="simplecell"><span data-ttu-id="b4742-483"><del></span><span class="sxs-lookup"><span data-stu-id="b4742-483"><del></span></span></td>
</tr>
<tr>
<td id="simplecell"><span data-ttu-id="b4742-484"><cite></span><span class="sxs-lookup"><span data-stu-id="b4742-484"><cite></span></span></td>
<td id="simplecell">&nbsp;</td>
<td id="simplecell">&nbsp;</td>
</tr>
</table>

 
## <a name="input-and-output-html-example"></a><span data-ttu-id="b4742-485">Пример входного и выходного HTML-кода</span><span class="sxs-lookup"><span data-stu-id="b4742-485">Input and output HTML example</span></span>

<span data-ttu-id="b4742-486">На приведенном ниже рисунке показана простая страница, созданная с помощью Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b4742-486">The following image shows a simple page that was created with Microsoft Graph.</span></span>

![Изображение страницы OneNote с учебными заметками по материалам из Википедии](images/onenote-sample-image.png)

<span data-ttu-id="b4742-488">Ниже показан входной HTML-код, отправляемый в тексте сообщения для создания страницы.</span><span class="sxs-lookup"><span data-stu-id="b4742-488">This is the input HTML sent in the message body to create the page.</span></span>

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
        <img alt="Apollo 11 commemorative stamp." src="https://upload.wikimedia.org/wikipedia/commons/a/a4/First_Man_on_Moon_1969_Issue-10c.jpg"  width="400"/>
        <p>References:</p>
        <p><a href="https://en.wikipedia.org/wiki/Apollo_11">https://en.wikipedia.org/wiki/Apollo_11</a></p>
        <p><a href="https://www.nasa.gov/mission_pages/apollo/missions/apollo11.html">https://www.nasa.gov/mission_pages/apollo/missions/apollo11.html</a></p>
    </body>
</html>
``` 

<br/>

<span data-ttu-id="b4742-489">Ниже показан выходной HTML-код, который Microsoft Graph возвращает при [получении содержимого страницы](onenote-get-content.md).</span><span class="sxs-lookup"><span data-stu-id="b4742-489">This is the output HTML that Microsoft Graph returns when you [get page content](onenote-get-content.md).</span></span>

> <span data-ttu-id="b4742-490">**Примечание.** При [создании страницы](onenote-create-page.md) или [получении метаданных страницы](/graph/api/page-get?view=graph-rest-1.0) API возвращает URL-адрес конечной точки *content* для страницы в свойстве **contentUrl**.</span><span class="sxs-lookup"><span data-stu-id="b4742-490">**Note:** When you [create a page](onenote-create-page.md) or [get page metadata](/graph/api/page-get?view=graph-rest-1.0), the API returns the *content* endpoint URL of the page in the **contentUrl** property.</span></span>

```html
<html htmlns="https://www.w3.org/1999/xhtml" lang="en-US">
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
            <p><a href="https://en.wikipedia.org/wiki/Apollo_11">https://en.wikipedia.org/wiki/Apollo_11</a></p>
            <p><a href="https://www.nasa.gov/mission_pages/apollo/missions/apollo11.html">https://www.nasa.gov/mission_pages/apollo/missions/apollo11.html</a></p>
        </div>
    </body>
</html>
``` 

## <a name="see-also"></a><span data-ttu-id="b4742-491">См. также</span><span class="sxs-lookup"><span data-stu-id="b4742-491">See also</span></span>

- [<span data-ttu-id="b4742-492">Получение содержимого и структуры OneNote</span><span class="sxs-lookup"><span data-stu-id="b4742-492">Get OneNote content and structure</span></span>](onenote-get-content.md)
- [<span data-ttu-id="b4742-493">Создание страниц OneNote</span><span class="sxs-lookup"><span data-stu-id="b4742-493">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="b4742-494">Обновление содержимого страницы OneNote</span><span class="sxs-lookup"><span data-stu-id="b4742-494">Update OneNote page content</span></span>](onenote-update-page.md)
- [<span data-ttu-id="b4742-495">Добавление изображений, видео и файлов</span><span class="sxs-lookup"><span data-stu-id="b4742-495">Add images, videos, and files</span></span>](onenote-images-files.md)
