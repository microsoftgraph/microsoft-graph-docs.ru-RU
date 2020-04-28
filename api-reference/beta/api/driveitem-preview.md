---
title: 'driveItem: Preview'
description: Это действие позволяет получать кратковременно недопустимые URL-адреса для встраиваемых элементов, чтобы отобразить временный предварительный просмотр.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
author: ''
ms.openlocfilehash: 8edd4aa2280978cca21443dbd3c6d175d0a64bd5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432441"
---
# <a name="driveitem-preview"></a><span data-ttu-id="d19d0-103">driveItem: Preview</span><span class="sxs-lookup"><span data-stu-id="d19d0-103">driveItem: preview</span></span>

<span data-ttu-id="d19d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d19d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d19d0-105">Это действие позволяет получать кратковременно недопустимые URL-адреса для встраиваемых элементов, чтобы отобразить временный предварительный просмотр.</span><span class="sxs-lookup"><span data-stu-id="d19d0-105">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="d19d0-106">Если вы хотите получить ссылки с большим сроком действия, используйте вместо этого API [CreateLink][] .</span><span class="sxs-lookup"><span data-stu-id="d19d0-106">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="d19d0-107">**Примечание:** В настоящее время действие **Предварительный просмотр** доступно только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="d19d0-107">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="d19d0-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d19d0-109">Permissions</span></span>

<span data-ttu-id="d19d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d19d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d19d0-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d19d0-112">Permission type</span></span>                        | <span data-ttu-id="d19d0-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d19d0-113">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="d19d0-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d19d0-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="d19d0-115">Files. Read, Files. ReadWrite, Files. ReadWrite. ALL, sites. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="d19d0-115">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="d19d0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d19d0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d19d0-117">Files. Read, Files. ReadWrite, Files. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d19d0-117">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="d19d0-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d19d0-118">Application</span></span>                            | <span data-ttu-id="d19d0-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d19d0-119">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="d19d0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d19d0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="d19d0-121">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d19d0-121">Request body</span></span>

<span data-ttu-id="d19d0-122">В теле запроса определяются свойства внедряемого URL-адреса, запрашиваемого приложением.</span><span class="sxs-lookup"><span data-stu-id="d19d0-122">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="d19d0-123">Запрос должен быть объектом JSON с указанными ниже свойствами.</span><span class="sxs-lookup"><span data-stu-id="d19d0-123">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="d19d0-124">Имя</span><span class="sxs-lookup"><span data-stu-id="d19d0-124">Name</span></span>      |  <span data-ttu-id="d19d0-125">Тип</span><span class="sxs-lookup"><span data-stu-id="d19d0-125">Type</span></span>         | <span data-ttu-id="d19d0-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d19d0-126">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="d19d0-127">Просмотр</span><span class="sxs-lookup"><span data-stu-id="d19d0-127">viewer</span></span>      | <span data-ttu-id="d19d0-128">string</span><span class="sxs-lookup"><span data-stu-id="d19d0-128">string</span></span>        | <span data-ttu-id="d19d0-129">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d19d0-129">Optional.</span></span> <span data-ttu-id="d19d0-130">Предварительная версия приложения для использования.</span><span class="sxs-lookup"><span data-stu-id="d19d0-130">Preview app to use.</span></span> <span data-ttu-id="d19d0-131">`onedrive` или `office`.</span><span class="sxs-lookup"><span data-stu-id="d19d0-131">`onedrive` or `office`.</span></span> <span data-ttu-id="d19d0-132">Если значение равно null, подходящее средство просмотра будет выбрано автоматически.</span><span class="sxs-lookup"><span data-stu-id="d19d0-132">If null, a suitable viewer will be chosen automatically.</span></span>
| <span data-ttu-id="d19d0-133">не для Chrome</span><span class="sxs-lookup"><span data-stu-id="d19d0-133">chromeless</span></span>  | <span data-ttu-id="d19d0-134">boolean</span><span class="sxs-lookup"><span data-stu-id="d19d0-134">boolean</span></span>       | <span data-ttu-id="d19d0-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d19d0-135">Optional.</span></span> <span data-ttu-id="d19d0-136">Если `true` выбрано значение (по умолчанию), то Внедренное представление не будет содержать элементы управления.</span><span class="sxs-lookup"><span data-stu-id="d19d0-136">If `true` (default), the embedded view will not include any controls.</span></span>
| <span data-ttu-id="d19d0-137">алловедит</span><span class="sxs-lookup"><span data-stu-id="d19d0-137">allowEdit</span></span>   | <span data-ttu-id="d19d0-138">boolean</span><span class="sxs-lookup"><span data-stu-id="d19d0-138">boolean</span></span>       | <span data-ttu-id="d19d0-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="d19d0-139">Optional.</span></span> <span data-ttu-id="d19d0-140">Если `true`файл можно редактировать из встроенного пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="d19d0-140">If `true`, the file can be edited from the embedded UI.</span></span>
| <span data-ttu-id="d19d0-141">page</span><span class="sxs-lookup"><span data-stu-id="d19d0-141">page</span></span>        | <span data-ttu-id="d19d0-142">строка или число</span><span class="sxs-lookup"><span data-stu-id="d19d0-142">string/number</span></span> | <span data-ttu-id="d19d0-143">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="d19d0-143">Optional.</span></span> <span data-ttu-id="d19d0-144">Номер страницы для начала документа, если это необходимо.</span><span class="sxs-lookup"><span data-stu-id="d19d0-144">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="d19d0-145">Указывается как строка для будущих случаев использования для типов файлов, таких как ZIP.</span><span class="sxs-lookup"><span data-stu-id="d19d0-145">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="d19d0-146">zoom</span><span class="sxs-lookup"><span data-stu-id="d19d0-146">zoom</span></span>        | <span data-ttu-id="d19d0-147">number</span><span class="sxs-lookup"><span data-stu-id="d19d0-147">number</span></span>        | <span data-ttu-id="d19d0-148">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="d19d0-148">Optional.</span></span> <span data-ttu-id="d19d0-149">Масштаб (при необходимости) для запуска.</span><span class="sxs-lookup"><span data-stu-id="d19d0-149">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="d19d0-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="d19d0-150">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="d19d0-151">Ответом будет объект JSON, содержащий следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="d19d0-151">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="d19d0-152">Имя</span><span class="sxs-lookup"><span data-stu-id="d19d0-152">Name</span></span>           | <span data-ttu-id="d19d0-153">Тип</span><span class="sxs-lookup"><span data-stu-id="d19d0-153">Type</span></span>   | <span data-ttu-id="d19d0-154">Описание</span><span class="sxs-lookup"><span data-stu-id="d19d0-154">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="d19d0-155">Команда</span><span class="sxs-lookup"><span data-stu-id="d19d0-155">getUrl</span></span>         | <span data-ttu-id="d19d0-156">string</span><span class="sxs-lookup"><span data-stu-id="d19d0-156">string</span></span> | <span data-ttu-id="d19d0-157">URL-адрес, подходящие для внедрения с помощью HTTP GET (Iframes и т. д.)</span><span class="sxs-lookup"><span data-stu-id="d19d0-157">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="d19d0-158">постурл</span><span class="sxs-lookup"><span data-stu-id="d19d0-158">postUrl</span></span>        | <span data-ttu-id="d19d0-159">string</span><span class="sxs-lookup"><span data-stu-id="d19d0-159">string</span></span> | <span data-ttu-id="d19d0-160">URL-адрес, подходящий для внедрения с помощью HTTP POST (форма POST, JS и т. д.)</span><span class="sxs-lookup"><span data-stu-id="d19d0-160">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="d19d0-161">Параметры</span><span class="sxs-lookup"><span data-stu-id="d19d0-161">postParameters</span></span> | <span data-ttu-id="d19d0-162">string</span><span class="sxs-lookup"><span data-stu-id="d19d0-162">string</span></span> | <span data-ttu-id="d19d0-163">Параметры POST для включения при использовании Постурл</span><span class="sxs-lookup"><span data-stu-id="d19d0-163">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="d19d0-164">В зависимости от текущего состояния поддержки внедрения для заданных параметров может возвращаться либо getUrl, Постурл, либо и то, и другое.</span><span class="sxs-lookup"><span data-stu-id="d19d0-164">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="d19d0-165">i-параметры — это строка, `application/x-www-form-urlencoded`отформатированная как, и при выполнении POST для постурл Content-Type необходимо задать соответствующие параметры.</span><span class="sxs-lookup"><span data-stu-id="d19d0-165">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="d19d0-166">Например:</span><span class="sxs-lookup"><span data-stu-id="d19d0-166">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a><span data-ttu-id="d19d0-167">Наблюдатели</span><span class="sxs-lookup"><span data-stu-id="d19d0-167">Viewers</span></span>

<span data-ttu-id="d19d0-168">Для параметра **средства просмотра** разрешены следующие значения.</span><span class="sxs-lookup"><span data-stu-id="d19d0-168">The following values are allowed for the **viewer** parameter.</span></span>

| <span data-ttu-id="d19d0-169">Значение типа</span><span class="sxs-lookup"><span data-stu-id="d19d0-169">Type value</span></span> | <span data-ttu-id="d19d0-170">Описание</span><span class="sxs-lookup"><span data-stu-id="d19d0-170">Description</span></span>
|:-----------|:----------------------------------------------------------------
| <span data-ttu-id="d19d0-171">определен</span><span class="sxs-lookup"><span data-stu-id="d19d0-171">(null)</span></span>     | <span data-ttu-id="d19d0-172">Выбирает соответствующее приложение для отображения файла.</span><span class="sxs-lookup"><span data-stu-id="d19d0-172">Chooses an appropriate app for rendering the file.</span></span> <span data-ttu-id="d19d0-173">В большинстве случаев будет использоваться `onedrive` предварительный просмотр, но он может варьироваться в зависимости от типа файла.</span><span class="sxs-lookup"><span data-stu-id="d19d0-173">In most cases this will use the `onedrive` previewer, but may vary by file type.</span></span>
| `onedrive` | <span data-ttu-id="d19d0-174">Использование приложения предварительного просмотра OneDrive для отображения файла.</span><span class="sxs-lookup"><span data-stu-id="d19d0-174">Use the OneDrive previewer app to render the file.</span></span>
| `office`   | <span data-ttu-id="d19d0-175">Используйте веб-версию Office для отображения файла.</span><span class="sxs-lookup"><span data-stu-id="d19d0-175">Use the web version of Office to render the file.</span></span> <span data-ttu-id="d19d0-176">Допускается только для документов Office.</span><span class="sxs-lookup"><span data-stu-id="d19d0-176">Only valid for Office documents.</span></span>

### <a name="chrome-vs-chromeless"></a><span data-ttu-id="d19d0-177">Хром VS Chrome</span><span class="sxs-lookup"><span data-stu-id="d19d0-177">Chrome vs chromeless</span></span>

<span data-ttu-id="d19d0-178">Если `chromeless` этот параметр имеет значение true, предварительный просмотр будет иметь исходное представление файла.</span><span class="sxs-lookup"><span data-stu-id="d19d0-178">If `chromeless` is true, the preview will be a bare rendering of the file.</span></span>
<span data-ttu-id="d19d0-179">В противном случае для взаимодействия с документом или представлением могут отображаться дополнительные панели инструментов и кнопки.</span><span class="sxs-lookup"><span data-stu-id="d19d0-179">Otherwise, there may be additional toolbars/buttons displayed for interacting with the document/view.</span></span>

### <a name="viewedit"></a><span data-ttu-id="d19d0-180">Просмотр и редактирование</span><span class="sxs-lookup"><span data-stu-id="d19d0-180">View/edit</span></span>

<span data-ttu-id="d19d0-181">Если `allowEdit` имеет значение true, документ можно изменить с помощью встроенной предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="d19d0-181">If `allowEdit` is true, the document can be modified by user interaction with the embedded preview.</span></span>
<span data-ttu-id="d19d0-182">Эта возможность может быть недоступна для предварительных версий приложений и типов файлов.</span><span class="sxs-lookup"><span data-stu-id="d19d0-182">This capability may not be available for all preview apps or file types.</span></span>

### <a name="pagezoom"></a><span data-ttu-id="d19d0-183">Страница/масштаб</span><span class="sxs-lookup"><span data-stu-id="d19d0-183">Page/zoom</span></span>

<span data-ttu-id="d19d0-184">Параметры `page` и `zoom` могут быть недоступны для всех предварительных версий приложений, но будут применены, если это приложение поддерживает приложение предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="d19d0-184">The `page` and `zoom` options might not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
