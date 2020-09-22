---
title: 'driveItem: Preview'
description: Это действие позволяет получать кратковременно недопустимые URL-адреса для встраиваемых элементов, чтобы отобразить временный предварительный просмотр.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
author: JeremyKelley
ms.openlocfilehash: f56f62fdd0244a5bc3a014cae4ad4bc9151181c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981886"
---
# <a name="driveitem-preview"></a><span data-ttu-id="657d8-103">driveItem: Preview</span><span class="sxs-lookup"><span data-stu-id="657d8-103">driveItem: preview</span></span>

<span data-ttu-id="657d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="657d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="657d8-105">Это действие позволяет получать кратковременно недопустимые URL-адреса для встраиваемых элементов, чтобы отобразить временный предварительный просмотр.</span><span class="sxs-lookup"><span data-stu-id="657d8-105">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="657d8-106">Если вы хотите получить ссылки с большим сроком действия, используйте вместо этого API [CreateLink][] .</span><span class="sxs-lookup"><span data-stu-id="657d8-106">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="657d8-107">**Примечание:** В настоящее время действие **Предварительный просмотр** доступно только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="657d8-107">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="657d8-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="657d8-109">Permissions</span></span>

<span data-ttu-id="657d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="657d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="657d8-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="657d8-112">Permission type</span></span>                        | <span data-ttu-id="657d8-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="657d8-113">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="657d8-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="657d8-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="657d8-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="657d8-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="657d8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="657d8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="657d8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="657d8-117">Not supported.</span></span>
| <span data-ttu-id="657d8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="657d8-118">Application</span></span>                            | <span data-ttu-id="657d8-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="657d8-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="657d8-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="657d8-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="657d8-121">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="657d8-121">Request body</span></span>

<span data-ttu-id="657d8-122">В теле запроса определяются свойства внедряемого URL-адреса, запрашиваемого приложением.</span><span class="sxs-lookup"><span data-stu-id="657d8-122">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="657d8-123">Запрос должен быть объектом JSON с указанными ниже свойствами.</span><span class="sxs-lookup"><span data-stu-id="657d8-123">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="657d8-124">Имя</span><span class="sxs-lookup"><span data-stu-id="657d8-124">Name</span></span>      |  <span data-ttu-id="657d8-125">Тип</span><span class="sxs-lookup"><span data-stu-id="657d8-125">Type</span></span>         | <span data-ttu-id="657d8-126">Описание</span><span class="sxs-lookup"><span data-stu-id="657d8-126">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="657d8-127">Просмотр</span><span class="sxs-lookup"><span data-stu-id="657d8-127">viewer</span></span>      | <span data-ttu-id="657d8-128">string</span><span class="sxs-lookup"><span data-stu-id="657d8-128">string</span></span>        | <span data-ttu-id="657d8-129">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="657d8-129">Optional.</span></span> <span data-ttu-id="657d8-130">Предварительная версия приложения для использования.</span><span class="sxs-lookup"><span data-stu-id="657d8-130">Preview app to use.</span></span> <span data-ttu-id="657d8-131">`onedrive` или `office`.</span><span class="sxs-lookup"><span data-stu-id="657d8-131">`onedrive` or `office`.</span></span> <span data-ttu-id="657d8-132">Если значение равно null, подходящее средство просмотра будет выбрано автоматически.</span><span class="sxs-lookup"><span data-stu-id="657d8-132">If null, a suitable viewer will be chosen automatically.</span></span>
| <span data-ttu-id="657d8-133">не для Chrome</span><span class="sxs-lookup"><span data-stu-id="657d8-133">chromeless</span></span>  | <span data-ttu-id="657d8-134">boolean</span><span class="sxs-lookup"><span data-stu-id="657d8-134">boolean</span></span>       | <span data-ttu-id="657d8-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="657d8-135">Optional.</span></span> <span data-ttu-id="657d8-136">Если `true` выбрано значение (по умолчанию), то Внедренное представление не будет содержать элементы управления.</span><span class="sxs-lookup"><span data-stu-id="657d8-136">If `true` (default), the embedded view will not include any controls.</span></span>
| <span data-ttu-id="657d8-137">алловедит</span><span class="sxs-lookup"><span data-stu-id="657d8-137">allowEdit</span></span>   | <span data-ttu-id="657d8-138">boolean</span><span class="sxs-lookup"><span data-stu-id="657d8-138">boolean</span></span>       | <span data-ttu-id="657d8-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="657d8-139">Optional.</span></span> <span data-ttu-id="657d8-140">Если `true` файл можно редактировать из встроенного пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="657d8-140">If `true`, the file can be edited from the embedded UI.</span></span>
| <span data-ttu-id="657d8-141">page</span><span class="sxs-lookup"><span data-stu-id="657d8-141">page</span></span>        | <span data-ttu-id="657d8-142">строка или число</span><span class="sxs-lookup"><span data-stu-id="657d8-142">string/number</span></span> | <span data-ttu-id="657d8-143">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="657d8-143">Optional.</span></span> <span data-ttu-id="657d8-144">Номер страницы для начала документа, если это необходимо.</span><span class="sxs-lookup"><span data-stu-id="657d8-144">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="657d8-145">Указывается как строка для будущих случаев использования для типов файлов, таких как ZIP.</span><span class="sxs-lookup"><span data-stu-id="657d8-145">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="657d8-146">zoom</span><span class="sxs-lookup"><span data-stu-id="657d8-146">zoom</span></span>        | <span data-ttu-id="657d8-147">number</span><span class="sxs-lookup"><span data-stu-id="657d8-147">number</span></span>        | <span data-ttu-id="657d8-148">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="657d8-148">Optional.</span></span> <span data-ttu-id="657d8-149">Масштаб (при необходимости) для запуска.</span><span class="sxs-lookup"><span data-stu-id="657d8-149">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="657d8-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="657d8-150">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="657d8-151">Ответом будет объект JSON, содержащий следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="657d8-151">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="657d8-152">Имя</span><span class="sxs-lookup"><span data-stu-id="657d8-152">Name</span></span>           | <span data-ttu-id="657d8-153">Тип</span><span class="sxs-lookup"><span data-stu-id="657d8-153">Type</span></span>   | <span data-ttu-id="657d8-154">Описание</span><span class="sxs-lookup"><span data-stu-id="657d8-154">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="657d8-155">Команда</span><span class="sxs-lookup"><span data-stu-id="657d8-155">getUrl</span></span>         | <span data-ttu-id="657d8-156">string</span><span class="sxs-lookup"><span data-stu-id="657d8-156">string</span></span> | <span data-ttu-id="657d8-157">URL-адрес, подходящие для внедрения с помощью HTTP GET (Iframes и т. д.)</span><span class="sxs-lookup"><span data-stu-id="657d8-157">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="657d8-158">постурл</span><span class="sxs-lookup"><span data-stu-id="657d8-158">postUrl</span></span>        | <span data-ttu-id="657d8-159">string</span><span class="sxs-lookup"><span data-stu-id="657d8-159">string</span></span> | <span data-ttu-id="657d8-160">URL-адрес, подходящий для внедрения с помощью HTTP POST (форма POST, JS и т. д.)</span><span class="sxs-lookup"><span data-stu-id="657d8-160">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="657d8-161">Параметры</span><span class="sxs-lookup"><span data-stu-id="657d8-161">postParameters</span></span> | <span data-ttu-id="657d8-162">string</span><span class="sxs-lookup"><span data-stu-id="657d8-162">string</span></span> | <span data-ttu-id="657d8-163">Параметры POST для включения при использовании Постурл</span><span class="sxs-lookup"><span data-stu-id="657d8-163">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="657d8-164">В зависимости от текущего состояния поддержки внедрения для заданных параметров может возвращаться либо getUrl, Постурл, либо и то, и другое.</span><span class="sxs-lookup"><span data-stu-id="657d8-164">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="657d8-165">i-параметры — это строка, отформатированная как `application/x-www-form-urlencoded` , и при выполнении POST для постурл Content-Type необходимо задать соответствующие параметры.</span><span class="sxs-lookup"><span data-stu-id="657d8-165">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="657d8-166">Например:</span><span class="sxs-lookup"><span data-stu-id="657d8-166">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a><span data-ttu-id="657d8-167">Наблюдатели</span><span class="sxs-lookup"><span data-stu-id="657d8-167">Viewers</span></span>

><span data-ttu-id="657d8-168">**Примечание:** Этот параметр является устаревшим и не будет доступен в конечной точке версии 1.0.</span><span class="sxs-lookup"><span data-stu-id="657d8-168">**Note:** This parameter is deprecated and will not be made available on the v1.0 endpoint.</span></span>

<span data-ttu-id="657d8-169">Для параметра **средства просмотра** разрешены следующие значения.</span><span class="sxs-lookup"><span data-stu-id="657d8-169">The following values are allowed for the **viewer** parameter.</span></span>

| <span data-ttu-id="657d8-170">Значение типа</span><span class="sxs-lookup"><span data-stu-id="657d8-170">Type value</span></span> | <span data-ttu-id="657d8-171">Описание</span><span class="sxs-lookup"><span data-stu-id="657d8-171">Description</span></span>
|:-----------|:----------------------------------------------------------------
| <span data-ttu-id="657d8-172">определен</span><span class="sxs-lookup"><span data-stu-id="657d8-172">(null)</span></span>     | <span data-ttu-id="657d8-173">Выбирает соответствующее приложение для отображения файла.</span><span class="sxs-lookup"><span data-stu-id="657d8-173">Chooses an appropriate app for rendering the file.</span></span> <span data-ttu-id="657d8-174">В большинстве случаев будет использоваться `onedrive` Предварительный просмотр, но он может варьироваться в зависимости от типа файла.</span><span class="sxs-lookup"><span data-stu-id="657d8-174">In most cases this will use the `onedrive` previewer, but may vary by file type.</span></span>
| `onedrive` | <span data-ttu-id="657d8-175">Использование приложения предварительного просмотра OneDrive для отображения файла.</span><span class="sxs-lookup"><span data-stu-id="657d8-175">Use the OneDrive previewer app to render the file.</span></span>
| `office`   | <span data-ttu-id="657d8-176">Используйте веб-версию Office для отображения файла.</span><span class="sxs-lookup"><span data-stu-id="657d8-176">Use the web version of Office to render the file.</span></span> <span data-ttu-id="657d8-177">Допускается только для документов Office.</span><span class="sxs-lookup"><span data-stu-id="657d8-177">Only valid for Office documents.</span></span>

### <a name="chrome-vs-chromeless"></a><span data-ttu-id="657d8-178">Хром VS Chrome</span><span class="sxs-lookup"><span data-stu-id="657d8-178">Chrome vs chromeless</span></span>
><span data-ttu-id="657d8-179">**Примечание:** Этот параметр является устаревшим и не будет доступен в конечной точке версии 1.0.</span><span class="sxs-lookup"><span data-stu-id="657d8-179">**Note:** This parameter is deprecated and will not be made available on the v1.0 endpoint.</span></span>

<span data-ttu-id="657d8-180">Если `chromeless` этот параметр имеет значение true, предварительный просмотр будет иметь исходное представление файла.</span><span class="sxs-lookup"><span data-stu-id="657d8-180">If `chromeless` is true, the preview will be a bare rendering of the file.</span></span>
<span data-ttu-id="657d8-181">В противном случае для взаимодействия с документом или представлением могут отображаться дополнительные панели инструментов и кнопки.</span><span class="sxs-lookup"><span data-stu-id="657d8-181">Otherwise, there may be additional toolbars/buttons displayed for interacting with the document/view.</span></span>

### <a name="viewedit"></a><span data-ttu-id="657d8-182">Просмотр и редактирование</span><span class="sxs-lookup"><span data-stu-id="657d8-182">View/edit</span></span>
><span data-ttu-id="657d8-183">**Примечание:** Этот параметр является устаревшим и не будет доступен в конечной точке версии 1.0.</span><span class="sxs-lookup"><span data-stu-id="657d8-183">**Note:** This parameter is deprecated and will not be made available on the v1.0 endpoint.</span></span>

<span data-ttu-id="657d8-184">Если `allowEdit` имеет значение true, документ можно изменить с помощью встроенной предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="657d8-184">If `allowEdit` is true, the document can be modified by user interaction with the embedded preview.</span></span>
<span data-ttu-id="657d8-185">Эта возможность может быть недоступна для предварительных версий приложений и типов файлов.</span><span class="sxs-lookup"><span data-stu-id="657d8-185">This capability may not be available for all preview apps or file types.</span></span>

### <a name="pagezoom"></a><span data-ttu-id="657d8-186">Страница/масштаб</span><span class="sxs-lookup"><span data-stu-id="657d8-186">Page/zoom</span></span>

<span data-ttu-id="657d8-187">`page`Параметры и `zoom` могут быть недоступны для всех предварительных версий приложений, но будут применены, если это приложение поддерживает приложение предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="657d8-187">The `page` and `zoom` options might not be available for all preview apps, but will be applied if the preview app supports it.</span></span>


