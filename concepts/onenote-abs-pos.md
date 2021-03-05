---
title: Создание элементов с абсолютным положением на страницах OneNote
description: В тексте страницы OneNote может содержаться много прямых (`div`, `img`) и дочерних (`object`) элементов, которые можно разместить независимо друг от друга на странице.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: e21ad3fb97b807bc91ecf6a993483f3bb83c82b8
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472841"
---
# <a name="create-absolute-positioned-elements-in-onenote-pages"></a><span data-ttu-id="e64e9-103">Создание элементов с абсолютным положением на страницах OneNote</span><span class="sxs-lookup"><span data-stu-id="e64e9-103">Create absolute positioned elements in OneNote pages</span></span>

<span data-ttu-id="e64e9-104">В тексте страницы OneNote может содержаться много прямых (`div`, `img`) и дочерних (`object`) элементов, которые можно разместить независимо друг от друга на странице.</span><span class="sxs-lookup"><span data-stu-id="e64e9-104">The body of a OneNote page can contain multiple direct `div`, `img`, and `object` child elements that can be positioned independently on the page.</span></span>

<a name="attributes"></a>

## <a name="attributes-and-positioning-behavior"></a><span data-ttu-id="e64e9-105">Атрибуты и поведение при расположении</span><span class="sxs-lookup"><span data-stu-id="e64e9-105">Attributes and positioning behavior</span></span>

<span data-ttu-id="e64e9-106">Чтобы создать элементы с абсолютным положением на странице, используйте атрибуты `data-absolute-enabled` и [`style`](#supported-css-style-attributes), как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="e64e9-106">Use the `data-absolute-enabled` and [`style`](#supported-css-style-attributes) attributes to create absolute positioned elements on a page, as follows:</span></span>

- <span data-ttu-id="e64e9-107">Элемент body должен указывать `data-absolute-enabled="true"`.</span><span class="sxs-lookup"><span data-stu-id="e64e9-107">The body element must specify `data-absolute-enabled="true"`.</span></span> <span data-ttu-id="e64e9-108">Если он опущен или имеет значение `false`, весь контент в элементе body отображается в элементе `_default` с абсолютным положением, созданным API, и все параметры положения будут проигнорированы.</span><span class="sxs-lookup"><span data-stu-id="e64e9-108">If omitted or set to `false`, all body content is rendered inside a `_default` absolute positioned div that the API creates, and all position settings are ignored.</span></span>

- <span data-ttu-id="e64e9-109">Только элементы `div`, `img` и `object` могут иметь абсолютное положение.</span><span class="sxs-lookup"><span data-stu-id="e64e9-109">Only `div`, `img`, and `object` elements can be absolute positioned elements.</span></span> 

- <span data-ttu-id="e64e9-110">Для элементов с абсолютным положением должен быть задан параметр `style="position:absolute"`.</span><span class="sxs-lookup"><span data-stu-id="e64e9-110">Absolute positioned elements must specify `style="position:absolute"`.</span></span>

- <span data-ttu-id="e64e9-111">Элементы с абсолютным положением должны быть прямыми дочерними элементами элемента `body`.</span><span class="sxs-lookup"><span data-stu-id="e64e9-111">Absolute positioned elements must be direct children of the `body` element.</span></span> <span data-ttu-id="e64e9-112">Любой прямой дочерний элемент элемента body, не являющийся элементом `div`, `img` или `object` с абсолютным положением, отображается в виде статичного контента внутри элемента div `_default` с абсолютным положением.</span><span class="sxs-lookup"><span data-stu-id="e64e9-112">Any direct children of the body that aren't absolute positioned `div`, `img`, or `object` elements are rendered as static content inside the absolute positioned `_default` div.</span></span>

- <span data-ttu-id="e64e9-113">Элементы с абсолютным положением размещаются согласно указанным для них координатам левого верхнего угла относительно начального положения 0:0, соответствующего левому верхнему углу страницы над областью заголовка.</span><span class="sxs-lookup"><span data-stu-id="e64e9-113">Absolute positioned elements are positioned at their specified top and left coordinates, relative to the 0:0 starting position at the top, left corner of the page above the title area.</span></span>

- <span data-ttu-id="e64e9-114">Если у элемента с абсолютным положением опущена верхняя или левая координата, для этой координаты применяется соответствующее значение, используемое по умолчанию: `top:120px` или `left:48px`.</span><span class="sxs-lookup"><span data-stu-id="e64e9-114">If an absolute positioned element omits the top or left coordinate, the missing coordinate is set to its default value: `top:120px` or `left:48px`.</span></span> <span data-ttu-id="e64e9-115">Эти координаты, используемые по умолчанию, указывают положение непосредственно под областью заголовка.</span><span class="sxs-lookup"><span data-stu-id="e64e9-115">These default coordinates specify a position just below the title area.</span></span> <span data-ttu-id="e64e9-116">Помните, что если не указывать координаты элементов, последние будут накладываться друг на друга.</span><span class="sxs-lookup"><span data-stu-id="e64e9-116">Be aware that omitting coordinates can result in elements that are stacked on top of each other.</span></span>

- <span data-ttu-id="e64e9-117">Элементы с абсолютным положением не должны быть вложенными и не должны содержать элементы с заданными положениями.</span><span class="sxs-lookup"><span data-stu-id="e64e9-117">Absolute positioned elements cannot be nested or contain positioned elements.</span></span> <span data-ttu-id="e64e9-118">API игнорирует все параметры положения, указанные во вложенных элементах внутри элемента div с абсолютным положением, отображает вложенный контент внутри родительского элемента div с абсолютным положением и возвращает предупреждение через свойство **api.diagnostics** в ответе.</span><span class="sxs-lookup"><span data-stu-id="e64e9-118">The API ignores any position settings specified on nested elements inside an absolute positioned div, renders the nested content inside the absolute positioned parent div, and returns a warning in the **api.diagnostics** property in the response.</span></span>


### <a name="example"></a><span data-ttu-id="e64e9-119">Пример</span><span class="sxs-lookup"><span data-stu-id="e64e9-119">Example</span></span>

<span data-ttu-id="e64e9-120">В примере ниже показан прямой дочерний элемент `p`, элемент div с абсолютным положением и элемент div с неабсолютным положением.</span><span class="sxs-lookup"><span data-stu-id="e64e9-120">The following example contains a direct `p` child, an absolute positioned div, and a non-absolute positioned div.</span></span>

#### <a name="input-html"></a><span data-ttu-id="e64e9-121">Входной HTML-код</span><span class="sxs-lookup"><span data-stu-id="e64e9-121">Input HTML</span></span>  

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

<span data-ttu-id="e64e9-122">API отрисовывает элемент div с неабсолютным положением в элементе div, используемом по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e64e9-122">The API renders the non-absolute positioned div in the default div.</span></span> <span data-ttu-id="e64e9-123">Обратите внимание, что система игнорирует вложенные теги `<div>`, так как в них не определено никакой семантической информации (например, `data-id`).</span><span class="sxs-lookup"><span data-stu-id="e64e9-123">Note that the nested `<div>` tags are discarded because they do not define any semantic information (such as `data-id`).</span></span>

#### <a name="output-html"></a><span data-ttu-id="e64e9-124">Выходной HTML-код</span><span class="sxs-lookup"><span data-stu-id="e64e9-124">Output HTML</span></span> 

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

### <a name="example"></a><span data-ttu-id="e64e9-125">Пример</span><span class="sxs-lookup"><span data-stu-id="e64e9-125">Example</span></span>

<span data-ttu-id="e64e9-126">В примере ниже показано, как создать страницу, которая содержит один элемент div с абсолютным положением и одно изображение с абсолютным положением.</span><span class="sxs-lookup"><span data-stu-id="e64e9-126">The following example creates a page that contains one absolute positioned div and one absolute positioned image.</span></span>


#### <a name="input-html"></a><span data-ttu-id="e64e9-127">Входной HTML-код</span><span class="sxs-lookup"><span data-stu-id="e64e9-127">Input HTML</span></span>  

```html 
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body data-absolute-enabled="true">
        <div style="position:absolute;width:280px;top:120px;left:68px">
            <p>Some text</p>
            <img style="width:120px" src="https://officeimg.vo.msecnd.net/files/018/949/ZA103278226.png" />
            <div>
                <p>More text inside a regular, nested div</p>
            </div>
        </div>
        <img style="position:absolute;width:360px;top:350px;left:300px" src="https://officeimg.vo.msecnd.net/files/018/949/ZA103278226.png" />
    </body>
</html>
```
 
<span data-ttu-id="e64e9-128">API OneNote оценивает входной HTML-код и сохраняет весь семантический контент и информацию о структуре, которые поддерживает OneNote.</span><span class="sxs-lookup"><span data-stu-id="e64e9-128">The OneNote API evaluates the input HTML and preserves all semantic content and any structural information that is supported by OneNote.</span></span> <span data-ttu-id="e64e9-129">Полученная в результате страница отображается, как показано на рисунке ниже (но без видимых границ для элемента div и изображения).</span><span class="sxs-lookup"><span data-stu-id="e64e9-129">The resulting page renders as shown in the following image (but without the visible borders for the div and image).</span></span> 

![Полученная в результате страница с элементом div и изображением с абсолютными положениями](images/abs-pos.png)

<span data-ttu-id="e64e9-131">Обратите внимание на изменение незначимого вложенного элемента div по сравнению со входным HTML-кодом.</span><span class="sxs-lookup"><span data-stu-id="e64e9-131">Notice the changes to the non-contributing, nested div from the input HTML.</span></span> <span data-ttu-id="e64e9-132">API сохраняет контент, содержащийся в элементе div, но игнорирует теги `<div>`, так как в элементе div не определена семантическая информация (например, `data-id`).</span><span class="sxs-lookup"><span data-stu-id="e64e9-132">The API preserves the div's content but discards the `<div>` tags because the div doesn't define semantic information (such as `data-id`).</span></span>

<span data-ttu-id="e64e9-133">Дополнительные сведения о том, как API OneNote обрабатывает входной и выходной HTML-код, см. в статье [Входной и выходной HTML-код на страницах OneNote](onenote-input-output-html.md).</span><span class="sxs-lookup"><span data-stu-id="e64e9-133">For more information about how the OneNote API handles input and output HTML, see [Input and output HTML for OneNote pages](onenote-input-output-html.md).</span></span>

<a name="style-attributes"></a>

## <a name="supported-css-style-attributes"></a><span data-ttu-id="e64e9-134">Поддерживаемые атрибуты стиля CSS</span><span class="sxs-lookup"><span data-stu-id="e64e9-134">Supported CSS style attributes</span></span>

<span data-ttu-id="e64e9-135">Для всех элементов с абсолютными положениями можно указать положения левого верхнего угла.</span><span class="sxs-lookup"><span data-stu-id="e64e9-135">All absolute positioned elements can specify top and left positions.</span></span> <span data-ttu-id="e64e9-136">Для элемента div и изображения можно указать ширину. Кроме того, для изображений можно указать высоту.</span><span class="sxs-lookup"><span data-stu-id="e64e9-136">Divs and images can specify width, and images can also specify height.</span></span> <span data-ttu-id="e64e9-137">Пример:</span><span class="sxs-lookup"><span data-stu-id="e64e9-137">For example:</span></span>

```html
<img style="position:absolute;top:140px;left:95px;width:480px;height:665px" src="..." />
```

| <span data-ttu-id="e64e9-138">Атрибут</span><span class="sxs-lookup"><span data-stu-id="e64e9-138">Attribute</span></span> | <span data-ttu-id="e64e9-139">Поддерживаемый элемент</span><span class="sxs-lookup"><span data-stu-id="e64e9-139">Supported element</span></span> | <span data-ttu-id="e64e9-140">Описание</span><span class="sxs-lookup"><span data-stu-id="e64e9-140">Description</span></span> |  
|:------|:------|:------|  
| <span data-ttu-id="e64e9-141">top</span><span class="sxs-lookup"><span data-stu-id="e64e9-141">top</span></span> | <span data-ttu-id="e64e9-142">div, img, object</span><span class="sxs-lookup"><span data-stu-id="e64e9-142">div, img, object</span></span> | <span data-ttu-id="e64e9-143">Координата верхней границы элемента по оси Y; только в пикселях.</span><span class="sxs-lookup"><span data-stu-id="e64e9-143">The y-axis coordinate of the element's top border, in pixels only.</span></span> <span data-ttu-id="e64e9-144">По умолчанию используется значение 120 пикселей.</span><span class="sxs-lookup"><span data-stu-id="e64e9-144">Default is 120 pixels.</span></span><br/><br/><span data-ttu-id="e64e9-145">Пример: `top:140px`</span><span class="sxs-lookup"><span data-stu-id="e64e9-145">Example: `top:140px`</span></span> |  
| <span data-ttu-id="e64e9-146">left</span><span class="sxs-lookup"><span data-stu-id="e64e9-146">left</span></span> |  <span data-ttu-id="e64e9-147">div, img, object</span><span class="sxs-lookup"><span data-stu-id="e64e9-147">div, img, object</span></span>  | <span data-ttu-id="e64e9-148">Координата левой границы элемента по оси X; только в пикселях.</span><span class="sxs-lookup"><span data-stu-id="e64e9-148">The x-axis coordinate of the element's left border, in pixels only.</span></span> <span data-ttu-id="e64e9-149">По умолчанию используется значение 48 пикселей.</span><span class="sxs-lookup"><span data-stu-id="e64e9-149">Default is 48 pixels.</span></span><br/><br/><span data-ttu-id="e64e9-150">Пример: `left:95px`</span><span class="sxs-lookup"><span data-stu-id="e64e9-150">Example: `left:95px`</span></span> |  
| <span data-ttu-id="e64e9-151">width</span><span class="sxs-lookup"><span data-stu-id="e64e9-151">width</span></span> |  <span data-ttu-id="e64e9-152">div, img</span><span class="sxs-lookup"><span data-stu-id="e64e9-152">div, img</span></span>  | <span data-ttu-id="e64e9-153">Ширина элемента; только в пикселях.</span><span class="sxs-lookup"><span data-stu-id="e64e9-153">The width of the element, in pixels only.</span></span><br/><br/><span data-ttu-id="e64e9-154">Пример: `width:480px`</span><span class="sxs-lookup"><span data-stu-id="e64e9-154">Example: `width:480px`</span></span> |  
| <span data-ttu-id="e64e9-155">height</span><span class="sxs-lookup"><span data-stu-id="e64e9-155">height</span></span> | <span data-ttu-id="e64e9-156">img</span><span class="sxs-lookup"><span data-stu-id="e64e9-156">img</span></span> | <span data-ttu-id="e64e9-157">Высота элемента; только в пикселях.</span><span class="sxs-lookup"><span data-stu-id="e64e9-157">The height of the element, in pixels only.</span></span> <span data-ttu-id="e64e9-158">Для элементов div высота рассчитывается в среде выполнения, и система игнорирует любое заданное значение высоты.</span><span class="sxs-lookup"><span data-stu-id="e64e9-158">For divs, height is calculated at runtime and any specified height value is ignored.</span></span><br/><br/><span data-ttu-id="e64e9-159">Пример: `height:665px`</span><span class="sxs-lookup"><span data-stu-id="e64e9-159">Example: `height:665px`</span></span> |  
 
<span data-ttu-id="e64e9-160">Система игнорирует другие атрибуты положения, например `z-index`.</span><span class="sxs-lookup"><span data-stu-id="e64e9-160">Other position attributes, such as `z-index`, are ignored.</span></span> <span data-ttu-id="e64e9-161">Для изображений с абсолютными положениями можно использовать атрибут `data-render-src` или `src`.</span><span class="sxs-lookup"><span data-stu-id="e64e9-161">Absolute positioned images can use either the `data-render-src` or `src` attribute.</span></span>


<a name="request-response-info"></a>

## <a name="response-information"></a><span data-ttu-id="e64e9-162">Информация в ответе</span><span class="sxs-lookup"><span data-stu-id="e64e9-162">Response information</span></span>

<span data-ttu-id="e64e9-163">API OneNote возвращает указанные ниже сведения в ответе.</span><span class="sxs-lookup"><span data-stu-id="e64e9-163">The OneNote API returns the following information in the response.</span></span>

| <span data-ttu-id="e64e9-164">Данные в отклике</span><span class="sxs-lookup"><span data-stu-id="e64e9-164">Response data</span></span> | <span data-ttu-id="e64e9-165">Описание</span><span class="sxs-lookup"><span data-stu-id="e64e9-165">Description</span></span> |  
|:------|:------|  
| <span data-ttu-id="e64e9-166">Код успешного завершения действия</span><span class="sxs-lookup"><span data-stu-id="e64e9-166">Success code</span></span> | <span data-ttu-id="e64e9-167">Код состояния HTTP 201 при успешном выполнении запроса POST и код состояния HTTP 204 при успешном выполнении запроса PATCH.</span><span class="sxs-lookup"><span data-stu-id="e64e9-167">A 201 HTTP status code for a successful POST request, and a 204 HTTP status code for a successful PATCH request.</span></span> |  
| <span data-ttu-id="e64e9-168">Ошибки</span><span class="sxs-lookup"><span data-stu-id="e64e9-168">Errors</span></span> | <span data-ttu-id="e64e9-169">Дополнительные сведения об ошибках OneNote, которые может возвращать Microsoft Graph, см. в статье [Коды ошибок для API OneNote в Microsoft Graph](onenote-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="e64e9-169">Read [Error codes for OneNote APIs in Microsoft Graph](onenote-error-codes.md) to learn about OneNote errors that Microsoft Graph can return.</span></span> |  
  


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="e64e9-170">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e64e9-170">Permissions</span></span>

<span data-ttu-id="e64e9-171">Чтобы можно было создавать или изменять страницы OneNote, вам придется запросить соответствующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="e64e9-171">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="e64e9-172">Выберите минимальный уровень разрешений, необходимый для работы вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="e64e9-172">Choose the lowest level of permissions that your app needs to do its work.</span></span>

#### <a name="permissions-for-post-pages"></a><span data-ttu-id="e64e9-173">Разрешения для запросов POST со страницами</span><span class="sxs-lookup"><span data-stu-id="e64e9-173">Permissions for POST pages</span></span> 

- <span data-ttu-id="e64e9-174">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="e64e9-174">Notes.Create</span></span>
- <span data-ttu-id="e64e9-175">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e64e9-175">Notes.ReadWrite</span></span>
- <span data-ttu-id="e64e9-176">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e64e9-176">Notes.ReadWrite.All</span></span>  


#### <a name="permissions-for-patch-pages"></a><span data-ttu-id="e64e9-177">Разрешения в случае запросов PATCH для страниц</span><span class="sxs-lookup"><span data-stu-id="e64e9-177">Permissions for PATCH pages</span></span> 

- <span data-ttu-id="e64e9-178">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e64e9-178">Notes.ReadWrite</span></span>
- <span data-ttu-id="e64e9-179">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e64e9-179">Notes.ReadWrite.All</span></span>

<span data-ttu-id="e64e9-180">Дополнительные сведения об областях разрешений и принципе их работы см. в разделе [Области разрешений OneNote](permissions-reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="e64e9-180">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions-reference.md#notes-permissions).</span></span>


<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="e64e9-181">См. также</span><span class="sxs-lookup"><span data-stu-id="e64e9-181">See also</span></span>

- [<span data-ttu-id="e64e9-182">Создание страниц OneNote</span><span class="sxs-lookup"><span data-stu-id="e64e9-182">Create OneNote pages</span></span>](onenote-create-page.md)
- [<span data-ttu-id="e64e9-183">Обновление содержимого страницы OneNote</span><span class="sxs-lookup"><span data-stu-id="e64e9-183">Update OneNote page content</span></span>](onenote-update-page.md)
- [<span data-ttu-id="e64e9-184">Интеграция с OneNote</span><span class="sxs-lookup"><span data-stu-id="e64e9-184">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="e64e9-185">Блог разработчиков OneNote</span><span class="sxs-lookup"><span data-stu-id="e64e9-185">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="e64e9-186">Вопросы разработки OneNote для Microsoft Q&A</span><span class="sxs-lookup"><span data-stu-id="e64e9-186">OneNote development questions on Microsoft Q&A</span></span>](https://docs.microsoft.com/answers/topics/microsoft-graph-notes.html)
- [<span data-ttu-id="e64e9-187">Репозитории GitHub OneNote</span><span class="sxs-lookup"><span data-stu-id="e64e9-187">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)  

