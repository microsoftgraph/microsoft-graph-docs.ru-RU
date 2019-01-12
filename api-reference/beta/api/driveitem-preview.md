---
title: 'driveItem: предварительный просмотр'
description: Это действие позволяет получать кратковременного встраиваемые URL-адреса для элемента для визуализации временные предварительного просмотра.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: be96a0cd451bb3f1c75c32f235d7669ce0bd7509
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980877"
---
# <a name="driveitem-preview"></a><span data-ttu-id="5c7da-103">driveItem: предварительный просмотр</span><span class="sxs-lookup"><span data-stu-id="5c7da-103">driveItem: preview</span></span>

> <span data-ttu-id="5c7da-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5c7da-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c7da-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c7da-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5c7da-106">Это действие позволяет получать кратковременного встраиваемые URL-адреса для элемента для визуализации временные предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="5c7da-106">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="5c7da-107">Если вы хотите получить длинные встраиваемые ссылки, используйте [команду createLink][] API.</span><span class="sxs-lookup"><span data-stu-id="5c7da-107">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="5c7da-108">**Примечание:** Действие **предварительного просмотра** в данный момент доступна только на сервере SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="5c7da-108">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[команду createLink]: driveitem-createlink.md
[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="5c7da-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c7da-110">Permissions</span></span>

<span data-ttu-id="5c7da-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c7da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5c7da-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c7da-113">Permission type</span></span>                        | <span data-ttu-id="5c7da-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c7da-114">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="5c7da-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c7da-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="5c7da-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c7da-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="5c7da-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c7da-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c7da-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c7da-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="5c7da-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c7da-119">Application</span></span>                            | <span data-ttu-id="5c7da-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c7da-120">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="5c7da-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c7da-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="5c7da-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c7da-122">Request body</span></span>

<span data-ttu-id="5c7da-123">Текст запроса определяет свойства встраиваемые URL-адреса, запрашивающего приложения.</span><span class="sxs-lookup"><span data-stu-id="5c7da-123">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="5c7da-124">Запрос должен быть объектом JSON с указанными ниже свойствами.</span><span class="sxs-lookup"><span data-stu-id="5c7da-124">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="5c7da-125">Имя</span><span class="sxs-lookup"><span data-stu-id="5c7da-125">Name</span></span>      |  <span data-ttu-id="5c7da-126">Тип</span><span class="sxs-lookup"><span data-stu-id="5c7da-126">Type</span></span>         | <span data-ttu-id="5c7da-127">Описание</span><span class="sxs-lookup"><span data-stu-id="5c7da-127">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="5c7da-128">Средство просмотра</span><span class="sxs-lookup"><span data-stu-id="5c7da-128">viewer</span></span>      | <span data-ttu-id="5c7da-129">строка</span><span class="sxs-lookup"><span data-stu-id="5c7da-129">string</span></span>        | <span data-ttu-id="5c7da-130">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="5c7da-130">Optional.</span></span> <span data-ttu-id="5c7da-131">Предварительная версия приложения для использования.</span><span class="sxs-lookup"><span data-stu-id="5c7da-131">Preview app to use.</span></span> <span data-ttu-id="5c7da-132">`onedrive` или `office`.</span><span class="sxs-lookup"><span data-stu-id="5c7da-132">`onedrive` or `office`.</span></span> <span data-ttu-id="5c7da-133">Если значение null, подходящее средство просмотра выбирается автоматически.</span><span class="sxs-lookup"><span data-stu-id="5c7da-133">If null, a suitable viewer will be chosen automatically.</span></span>
| <span data-ttu-id="5c7da-134">chromeless</span><span class="sxs-lookup"><span data-stu-id="5c7da-134">chromeless</span></span>  | <span data-ttu-id="5c7da-135">boolean</span><span class="sxs-lookup"><span data-stu-id="5c7da-135">boolean</span></span>       | <span data-ttu-id="5c7da-136">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="5c7da-136">Optional.</span></span> <span data-ttu-id="5c7da-137">Если `true` (по умолчанию), внедренное представление не будет содержать все элементы управления.</span><span class="sxs-lookup"><span data-stu-id="5c7da-137">If `true` (default), the embedded view will not include any controls.</span></span>
| <span data-ttu-id="5c7da-138">Свойство allowEdit</span><span class="sxs-lookup"><span data-stu-id="5c7da-138">allowEdit</span></span>   | <span data-ttu-id="5c7da-139">boolean</span><span class="sxs-lookup"><span data-stu-id="5c7da-139">boolean</span></span>       | <span data-ttu-id="5c7da-140">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="5c7da-140">Optional.</span></span> <span data-ttu-id="5c7da-141">Если `true`, файл можно редактировать в пользовательском Интерфейсе внедренных.</span><span class="sxs-lookup"><span data-stu-id="5c7da-141">If `true`, the file can be edited from the embedded UI.</span></span>
| <span data-ttu-id="5c7da-142">page</span><span class="sxs-lookup"><span data-stu-id="5c7da-142">page</span></span>        | <span data-ttu-id="5c7da-143">Строка или номер</span><span class="sxs-lookup"><span data-stu-id="5c7da-143">string/number</span></span> | <span data-ttu-id="5c7da-144">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="5c7da-144">Optional.</span></span> <span data-ttu-id="5c7da-145">Номер документа для запуска, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="5c7da-145">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="5c7da-146">Указан как строка для использования в будущем случаев вокруг типов файлов, например ZIP.</span><span class="sxs-lookup"><span data-stu-id="5c7da-146">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="5c7da-147">zoom</span><span class="sxs-lookup"><span data-stu-id="5c7da-147">zoom</span></span>        | <span data-ttu-id="5c7da-148">число</span><span class="sxs-lookup"><span data-stu-id="5c7da-148">number</span></span>        | <span data-ttu-id="5c7da-149">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="5c7da-149">Optional.</span></span> <span data-ttu-id="5c7da-150">Выбор масштаба для запуска, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="5c7da-150">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="5c7da-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c7da-151">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="5c7da-152">Ответ будет объект JSON, который содержит следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="5c7da-152">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="5c7da-153">Имя</span><span class="sxs-lookup"><span data-stu-id="5c7da-153">Name</span></span>           | <span data-ttu-id="5c7da-154">Тип</span><span class="sxs-lookup"><span data-stu-id="5c7da-154">Type</span></span>   | <span data-ttu-id="5c7da-155">Описание</span><span class="sxs-lookup"><span data-stu-id="5c7da-155">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="5c7da-156">getUrl</span><span class="sxs-lookup"><span data-stu-id="5c7da-156">getUrl</span></span>         | <span data-ttu-id="5c7da-157">строка</span><span class="sxs-lookup"><span data-stu-id="5c7da-157">string</span></span> | <span data-ttu-id="5c7da-158">URL-адрес для внедрения с помощью HTTP GET (Интернет-кадров, и т.д.)</span><span class="sxs-lookup"><span data-stu-id="5c7da-158">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="5c7da-159">postUrl</span><span class="sxs-lookup"><span data-stu-id="5c7da-159">postUrl</span></span>        | <span data-ttu-id="5c7da-160">строка</span><span class="sxs-lookup"><span data-stu-id="5c7da-160">string</span></span> | <span data-ttu-id="5c7da-161">URL-адрес для внедрения с помощью HTTP POST (отправки формы, JS, и т.д.)</span><span class="sxs-lookup"><span data-stu-id="5c7da-161">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="5c7da-162">postParameters</span><span class="sxs-lookup"><span data-stu-id="5c7da-162">postParameters</span></span> | <span data-ttu-id="5c7da-163">строка</span><span class="sxs-lookup"><span data-stu-id="5c7da-163">string</span></span> | <span data-ttu-id="5c7da-164">Параметры отправки для включения при использовании postUrl</span><span class="sxs-lookup"><span data-stu-id="5c7da-164">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="5c7da-165">В зависимости от текущего состояния внедрить поддержку указанные параметры могут возвращаться getUrl, postUrl или оба.</span><span class="sxs-lookup"><span data-stu-id="5c7da-165">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="5c7da-166">postParameters — это строка в формате `application/x-www-form-urlencoded`, и, если для выполнения ОТПРАВКУ postUrl типа контента необходимо задать соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="5c7da-166">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="5c7da-167">Примеры:</span><span class="sxs-lookup"><span data-stu-id="5c7da-167">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a><span data-ttu-id="5c7da-168">Средства просмотра</span><span class="sxs-lookup"><span data-stu-id="5c7da-168">Viewers</span></span>

<span data-ttu-id="5c7da-169">Для **просмотра** параметров могут следующие значения.</span><span class="sxs-lookup"><span data-stu-id="5c7da-169">The following values are allowed for the **viewer** parameter.</span></span>

| <span data-ttu-id="5c7da-170">Значение типа</span><span class="sxs-lookup"><span data-stu-id="5c7da-170">Type value</span></span> | <span data-ttu-id="5c7da-171">Описание</span><span class="sxs-lookup"><span data-stu-id="5c7da-171">Description</span></span>
|:-----------|:----------------------------------------------------------------
| <span data-ttu-id="5c7da-172">(null)</span><span class="sxs-lookup"><span data-stu-id="5c7da-172">(null)</span></span>     | <span data-ttu-id="5c7da-173">Выбирает соответствующие приложения для отображения файла.</span><span class="sxs-lookup"><span data-stu-id="5c7da-173">Chooses an appropriate app for rendering the file.</span></span> <span data-ttu-id="5c7da-174">В большинстве случаев это будет использовать `onedrive` средство просмотра, но могут в зависимости от типа файла.</span><span class="sxs-lookup"><span data-stu-id="5c7da-174">In most cases this will use the `onedrive` previewer, but may vary by file type.</span></span>
| `onedrive` | <span data-ttu-id="5c7da-175">Использование приложения просмотра OneDrive для отображения файла.</span><span class="sxs-lookup"><span data-stu-id="5c7da-175">Use the OneDrive previewer app to render the file.</span></span>
| `office`   | <span data-ttu-id="5c7da-176">Используйте WAC (Office online) для отображения файла.</span><span class="sxs-lookup"><span data-stu-id="5c7da-176">Use the WAC (Office online) to render the file.</span></span> <span data-ttu-id="5c7da-177">Поддерживается только при работе с документами Office.</span><span class="sxs-lookup"><span data-stu-id="5c7da-177">Only valid for Office documents.</span></span>

### <a name="chrome-vs-chromeless"></a><span data-ttu-id="5c7da-178">Chromeless хрома vs</span><span class="sxs-lookup"><span data-stu-id="5c7da-178">Chrome vs chromeless</span></span>

<span data-ttu-id="5c7da-179">Если `chromeless` имеет значение true, предварительный просмотр будет исходного состояния отображения файла.</span><span class="sxs-lookup"><span data-stu-id="5c7da-179">If `chromeless` is true, the preview will be a bare rendering of the file.</span></span>
<span data-ttu-id="5c7da-180">В противном случае может быть дополнительные панели инструментов и кнопок, отображаемых для взаимодействия с документов и представлений.</span><span class="sxs-lookup"><span data-stu-id="5c7da-180">Otherwise, there may be additional toolbars/buttons displayed for interacting with the document/view.</span></span>

### <a name="viewedit"></a><span data-ttu-id="5c7da-181">Просмотр и изменение</span><span class="sxs-lookup"><span data-stu-id="5c7da-181">View/edit</span></span>

<span data-ttu-id="5c7da-182">Если `allowEdit` имеет значение true, документ можно изменить взаимодействия с пользователем с внедренным предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="5c7da-182">If `allowEdit` is true, the document can be modified by user interaction with the embedded preview.</span></span>
<span data-ttu-id="5c7da-183">Эта возможность не могут быть доступны для всех приложений предварительного просмотра или типов файлов.</span><span class="sxs-lookup"><span data-stu-id="5c7da-183">This capability may not be available for all preview apps or file types.</span></span>

### <a name="pagezoom"></a><span data-ttu-id="5c7da-184">Масштаб страницы /</span><span class="sxs-lookup"><span data-stu-id="5c7da-184">Page/zoom</span></span>

<span data-ttu-id="5c7da-185">`page` И `zoom` параметры могут быть недоступны для всех приложений предварительного просмотра, но будет применяться, если версия приложения поддерживает его.</span><span class="sxs-lookup"><span data-stu-id="5c7da-185">The `page` and `zoom` options might not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
