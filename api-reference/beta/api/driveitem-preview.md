---
title: 'driveItem: предварительный просмотр'
description: Это действие позволяет получать кратковременного встраиваемые URL-адреса для элемента для визуализации временные предварительного просмотра.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a49a05e1e01616bc9bbbb713fd05805d9af3070
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508540"
---
# <a name="driveitem-preview"></a><span data-ttu-id="97398-103">driveItem: предварительный просмотр</span><span class="sxs-lookup"><span data-stu-id="97398-103">driveItem: preview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97398-104">Это действие позволяет получать кратковременного встраиваемые URL-адреса для элемента для визуализации временные предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="97398-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="97398-105">Если вы хотите получить длинные встраиваемые ссылки, используйте [команду createLink][] API.</span><span class="sxs-lookup"><span data-stu-id="97398-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="97398-106">**Примечание:** Действие **предварительного просмотра** в данный момент доступна только на сервере SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="97398-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[команду createLink]: driveitem-createlink.md
[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="97398-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97398-108">Permissions</span></span>

<span data-ttu-id="97398-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97398-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97398-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97398-111">Permission type</span></span>                        | <span data-ttu-id="97398-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97398-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="97398-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97398-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="97398-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97398-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="97398-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97398-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97398-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97398-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="97398-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97398-117">Application</span></span>                            | <span data-ttu-id="97398-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97398-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="97398-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97398-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="97398-120">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97398-120">Request body</span></span>

<span data-ttu-id="97398-121">Текст запроса определяет свойства встраиваемые URL-адреса, запрашивающего приложения.</span><span class="sxs-lookup"><span data-stu-id="97398-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="97398-122">Запрос должен быть объектом JSON с указанными ниже свойствами.</span><span class="sxs-lookup"><span data-stu-id="97398-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="97398-123">Имя</span><span class="sxs-lookup"><span data-stu-id="97398-123">Name</span></span>      |  <span data-ttu-id="97398-124">Тип</span><span class="sxs-lookup"><span data-stu-id="97398-124">Type</span></span>         | <span data-ttu-id="97398-125">Описание</span><span class="sxs-lookup"><span data-stu-id="97398-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="97398-126">Средство просмотра</span><span class="sxs-lookup"><span data-stu-id="97398-126">viewer</span></span>      | <span data-ttu-id="97398-127">string</span><span class="sxs-lookup"><span data-stu-id="97398-127">string</span></span>        | <span data-ttu-id="97398-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="97398-128">Optional.</span></span> <span data-ttu-id="97398-129">Предварительная версия приложения для использования.</span><span class="sxs-lookup"><span data-stu-id="97398-129">Preview app to use.</span></span> <span data-ttu-id="97398-130">`onedrive` или `office`.</span><span class="sxs-lookup"><span data-stu-id="97398-130">`onedrive` or `office`.</span></span> <span data-ttu-id="97398-131">Если значение null, подходящее средство просмотра выбирается автоматически.</span><span class="sxs-lookup"><span data-stu-id="97398-131">If null, a suitable viewer will be chosen automatically.</span></span>
| <span data-ttu-id="97398-132">chromeless</span><span class="sxs-lookup"><span data-stu-id="97398-132">chromeless</span></span>  | <span data-ttu-id="97398-133">boolean</span><span class="sxs-lookup"><span data-stu-id="97398-133">boolean</span></span>       | <span data-ttu-id="97398-134">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="97398-134">Optional.</span></span> <span data-ttu-id="97398-135">Если `true` (по умолчанию), внедренное представление не будет содержать все элементы управления.</span><span class="sxs-lookup"><span data-stu-id="97398-135">If `true` (default), the embedded view will not include any controls.</span></span>
| <span data-ttu-id="97398-136">AllowEdit</span><span class="sxs-lookup"><span data-stu-id="97398-136">allowEdit</span></span>   | <span data-ttu-id="97398-137">boolean</span><span class="sxs-lookup"><span data-stu-id="97398-137">boolean</span></span>       | <span data-ttu-id="97398-138">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="97398-138">Optional.</span></span> <span data-ttu-id="97398-139">Если `true`, файл можно редактировать в пользовательском Интерфейсе внедренных.</span><span class="sxs-lookup"><span data-stu-id="97398-139">If `true`, the file can be edited from the embedded UI.</span></span>
| <span data-ttu-id="97398-140">page</span><span class="sxs-lookup"><span data-stu-id="97398-140">page</span></span>        | <span data-ttu-id="97398-141">Строка или номер</span><span class="sxs-lookup"><span data-stu-id="97398-141">string/number</span></span> | <span data-ttu-id="97398-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="97398-142">Optional.</span></span> <span data-ttu-id="97398-143">Номер документа для запуска, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="97398-143">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="97398-144">Указан как строка для использования в будущем случаев вокруг типов файлов, например ZIP.</span><span class="sxs-lookup"><span data-stu-id="97398-144">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="97398-145">zoom</span><span class="sxs-lookup"><span data-stu-id="97398-145">zoom</span></span>        | <span data-ttu-id="97398-146">число</span><span class="sxs-lookup"><span data-stu-id="97398-146">number</span></span>        | <span data-ttu-id="97398-147">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="97398-147">Optional.</span></span> <span data-ttu-id="97398-148">Выбор масштаба для запуска, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="97398-148">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="97398-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="97398-149">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="97398-150">Ответ будет объект JSON, который содержит следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="97398-150">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="97398-151">Имя</span><span class="sxs-lookup"><span data-stu-id="97398-151">Name</span></span>           | <span data-ttu-id="97398-152">Тип</span><span class="sxs-lookup"><span data-stu-id="97398-152">Type</span></span>   | <span data-ttu-id="97398-153">Описание</span><span class="sxs-lookup"><span data-stu-id="97398-153">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="97398-154">getUrl</span><span class="sxs-lookup"><span data-stu-id="97398-154">getUrl</span></span>         | <span data-ttu-id="97398-155">string</span><span class="sxs-lookup"><span data-stu-id="97398-155">string</span></span> | <span data-ttu-id="97398-156">URL-адрес для внедрения с помощью HTTP GET (Интернет-кадров, и т.д.)</span><span class="sxs-lookup"><span data-stu-id="97398-156">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="97398-157">postUrl</span><span class="sxs-lookup"><span data-stu-id="97398-157">postUrl</span></span>        | <span data-ttu-id="97398-158">string</span><span class="sxs-lookup"><span data-stu-id="97398-158">string</span></span> | <span data-ttu-id="97398-159">URL-адрес для внедрения с помощью HTTP POST (отправки формы, JS, и т.д.)</span><span class="sxs-lookup"><span data-stu-id="97398-159">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="97398-160">postParameters</span><span class="sxs-lookup"><span data-stu-id="97398-160">postParameters</span></span> | <span data-ttu-id="97398-161">string</span><span class="sxs-lookup"><span data-stu-id="97398-161">string</span></span> | <span data-ttu-id="97398-162">Параметры отправки для включения при использовании postUrl</span><span class="sxs-lookup"><span data-stu-id="97398-162">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="97398-163">В зависимости от текущего состояния внедрить поддержку указанные параметры могут возвращаться getUrl, postUrl или оба.</span><span class="sxs-lookup"><span data-stu-id="97398-163">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="97398-164">postParameters — это строка в формате `application/x-www-form-urlencoded`, и, если для выполнения ОТПРАВКУ postUrl типа контента необходимо задать соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="97398-164">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="97398-165">Пример:</span><span class="sxs-lookup"><span data-stu-id="97398-165">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a><span data-ttu-id="97398-166">Средства просмотра</span><span class="sxs-lookup"><span data-stu-id="97398-166">Viewers</span></span>

<span data-ttu-id="97398-167">Для **просмотра** параметров могут следующие значения.</span><span class="sxs-lookup"><span data-stu-id="97398-167">The following values are allowed for the **viewer** parameter.</span></span>

| <span data-ttu-id="97398-168">Значение типа</span><span class="sxs-lookup"><span data-stu-id="97398-168">Type value</span></span> | <span data-ttu-id="97398-169">Описание</span><span class="sxs-lookup"><span data-stu-id="97398-169">Description</span></span>
|:-----------|:----------------------------------------------------------------
| <span data-ttu-id="97398-170">Null</span><span class="sxs-lookup"><span data-stu-id="97398-170">(null)</span></span>     | <span data-ttu-id="97398-171">Выбирает соответствующие приложения для отображения файла.</span><span class="sxs-lookup"><span data-stu-id="97398-171">Chooses an appropriate app for rendering the file.</span></span> <span data-ttu-id="97398-172">В большинстве случаев это будет использовать `onedrive` средство просмотра, но могут в зависимости от типа файла.</span><span class="sxs-lookup"><span data-stu-id="97398-172">In most cases this will use the `onedrive` previewer, but may vary by file type.</span></span>
| `onedrive` | <span data-ttu-id="97398-173">Использование приложения просмотра OneDrive для отображения файла.</span><span class="sxs-lookup"><span data-stu-id="97398-173">Use the OneDrive previewer app to render the file.</span></span>
| `office`   | <span data-ttu-id="97398-174">Используйте WAC (Office online) для отображения файла.</span><span class="sxs-lookup"><span data-stu-id="97398-174">Use the WAC (Office online) to render the file.</span></span> <span data-ttu-id="97398-175">Поддерживается только при работе с документами Office.</span><span class="sxs-lookup"><span data-stu-id="97398-175">Only valid for Office documents.</span></span>

### <a name="chrome-vs-chromeless"></a><span data-ttu-id="97398-176">Chromeless хрома vs</span><span class="sxs-lookup"><span data-stu-id="97398-176">Chrome vs chromeless</span></span>

<span data-ttu-id="97398-177">Если `chromeless` имеет значение true, предварительный просмотр будет исходного состояния отображения файла.</span><span class="sxs-lookup"><span data-stu-id="97398-177">If `chromeless` is true, the preview will be a bare rendering of the file.</span></span>
<span data-ttu-id="97398-178">В противном случае может быть дополнительные панели инструментов и кнопок, отображаемых для взаимодействия с документов и представлений.</span><span class="sxs-lookup"><span data-stu-id="97398-178">Otherwise, there may be additional toolbars/buttons displayed for interacting with the document/view.</span></span>

### <a name="viewedit"></a><span data-ttu-id="97398-179">Просмотр и изменение</span><span class="sxs-lookup"><span data-stu-id="97398-179">View/edit</span></span>

<span data-ttu-id="97398-180">Если `allowEdit` имеет значение true, документ можно изменить взаимодействия с пользователем с внедренным предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="97398-180">If `allowEdit` is true, the document can be modified by user interaction with the embedded preview.</span></span>
<span data-ttu-id="97398-181">Эта возможность не могут быть доступны для всех приложений предварительного просмотра или типов файлов.</span><span class="sxs-lookup"><span data-stu-id="97398-181">This capability may not be available for all preview apps or file types.</span></span>

### <a name="pagezoom"></a><span data-ttu-id="97398-182">Масштаб страницы /</span><span class="sxs-lookup"><span data-stu-id="97398-182">Page/zoom</span></span>

<span data-ttu-id="97398-183">`page` И `zoom` параметры могут быть недоступны для всех приложений предварительного просмотра, но будет применяться, если версия приложения поддерживает его.</span><span class="sxs-lookup"><span data-stu-id="97398-183">The `page` and `zoom` options might not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-preview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
