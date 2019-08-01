---
title: 'driveItem: Preview'
description: Это действие позволяет получать кратковременно недопустимые URL-адреса для встраиваемых элементов, чтобы отобразить временный предварительный просмотр.
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: 1de53b8183f4277c0241a08822ef539613b83a45
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015343"
---
# <a name="driveitem-preview"></a><span data-ttu-id="e587a-103">driveItem: Preview</span><span class="sxs-lookup"><span data-stu-id="e587a-103">driveItem: preview</span></span>

<span data-ttu-id="e587a-104">Это действие позволяет получать кратковременно недопустимые URL-адреса для встраиваемых элементов, чтобы отобразить временный предварительный просмотр.</span><span class="sxs-lookup"><span data-stu-id="e587a-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="e587a-105">Если вы хотите получить ссылки с большим сроком действия, используйте вместо этого API [CreateLink][] .</span><span class="sxs-lookup"><span data-stu-id="e587a-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="e587a-106">**Примечание:** В настоящее время действие **Предварительный просмотр** доступно только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e587a-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="e587a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e587a-108">Permissions</span></span>

<span data-ttu-id="e587a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e587a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e587a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e587a-111">Permission type</span></span>                        | <span data-ttu-id="e587a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e587a-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="e587a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e587a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e587a-114">Files. Read, Files. ReadWrite, Files. ReadWrite. ALL, sites. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="e587a-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="e587a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e587a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e587a-116">Files. Read, Files. ReadWrite, Files. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e587a-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="e587a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e587a-117">Application</span></span>                            | <span data-ttu-id="e587a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e587a-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="e587a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e587a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="e587a-120">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e587a-120">Request body</span></span>

<span data-ttu-id="e587a-121">В теле запроса определяются свойства внедряемого URL-адреса, запрашиваемого приложением.</span><span class="sxs-lookup"><span data-stu-id="e587a-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="e587a-122">Запрос должен быть объектом JSON с указанными ниже свойствами.</span><span class="sxs-lookup"><span data-stu-id="e587a-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="e587a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e587a-123">Name</span></span>      |  <span data-ttu-id="e587a-124">Тип</span><span class="sxs-lookup"><span data-stu-id="e587a-124">Type</span></span>         | <span data-ttu-id="e587a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e587a-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="e587a-126">page</span><span class="sxs-lookup"><span data-stu-id="e587a-126">page</span></span>        | <span data-ttu-id="e587a-127">строка или число</span><span class="sxs-lookup"><span data-stu-id="e587a-127">string/number</span></span> | <span data-ttu-id="e587a-128">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="e587a-128">Optional.</span></span> <span data-ttu-id="e587a-129">Номер страницы для начала документа, если это необходимо.</span><span class="sxs-lookup"><span data-stu-id="e587a-129">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="e587a-130">Указывается как строка для будущих случаев использования для типов файлов, таких как ZIP.</span><span class="sxs-lookup"><span data-stu-id="e587a-130">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="e587a-131">zoom</span><span class="sxs-lookup"><span data-stu-id="e587a-131">zoom</span></span>        | <span data-ttu-id="e587a-132">number</span><span class="sxs-lookup"><span data-stu-id="e587a-132">number</span></span>        | <span data-ttu-id="e587a-133">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e587a-133">Optional.</span></span> <span data-ttu-id="e587a-134">Масштаб (при необходимости) для запуска.</span><span class="sxs-lookup"><span data-stu-id="e587a-134">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="e587a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e587a-135">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="e587a-136">Ответом будет объект JSON, содержащий следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="e587a-136">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="e587a-137">Имя</span><span class="sxs-lookup"><span data-stu-id="e587a-137">Name</span></span>           | <span data-ttu-id="e587a-138">Тип</span><span class="sxs-lookup"><span data-stu-id="e587a-138">Type</span></span>   | <span data-ttu-id="e587a-139">Описание</span><span class="sxs-lookup"><span data-stu-id="e587a-139">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="e587a-140">Команда</span><span class="sxs-lookup"><span data-stu-id="e587a-140">getUrl</span></span>         | <span data-ttu-id="e587a-141">string</span><span class="sxs-lookup"><span data-stu-id="e587a-141">string</span></span> | <span data-ttu-id="e587a-142">URL-адрес, подходящие для внедрения с помощью HTTP GET (Iframes и т. д.)</span><span class="sxs-lookup"><span data-stu-id="e587a-142">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="e587a-143">Постурл</span><span class="sxs-lookup"><span data-stu-id="e587a-143">postUrl</span></span>        | <span data-ttu-id="e587a-144">string</span><span class="sxs-lookup"><span data-stu-id="e587a-144">string</span></span> | <span data-ttu-id="e587a-145">URL-адрес, подходящий для внедрения с помощью HTTP POST (форма POST, JS и т. д.)</span><span class="sxs-lookup"><span data-stu-id="e587a-145">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="e587a-146">Параметры</span><span class="sxs-lookup"><span data-stu-id="e587a-146">postParameters</span></span> | <span data-ttu-id="e587a-147">string</span><span class="sxs-lookup"><span data-stu-id="e587a-147">string</span></span> | <span data-ttu-id="e587a-148">Параметры POST для включения при использовании Постурл</span><span class="sxs-lookup"><span data-stu-id="e587a-148">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="e587a-149">В зависимости от текущего состояния поддержки внедрения для заданных параметров может возвращаться либо getUrl, Постурл, либо и то, и другое.</span><span class="sxs-lookup"><span data-stu-id="e587a-149">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="e587a-150">i-параметры — это строка, `application/x-www-form-urlencoded`отформатированная как, и при выполнении POST для постурл Content-Type необходимо задать соответствующие параметры.</span><span class="sxs-lookup"><span data-stu-id="e587a-150">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="e587a-151">Пример:</span><span class="sxs-lookup"><span data-stu-id="e587a-151">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="e587a-152">Страница/масштаб</span><span class="sxs-lookup"><span data-stu-id="e587a-152">Page/zoom</span></span>

<span data-ttu-id="e587a-153">Параметры "Page" и "Zoom" могут быть недоступны для всех предварительных приложений, но будут применены, если это приложение поддерживает приложение Preview.</span><span class="sxs-lookup"><span data-stu-id="e587a-153">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
