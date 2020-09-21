---
title: 'driveItem: Preview'
description: Это действие позволяет получать кратковременно недопустимые URL-адреса для встраиваемых элементов, чтобы отобразить временный предварительный просмотр.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: apiPageType
ms.openlocfilehash: 5fea16ce14e2df4b87ddc2b3f9246dfe758ec5b1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073266"
---
# <a name="driveitem-preview"></a><span data-ttu-id="f0397-103">driveItem: Preview</span><span class="sxs-lookup"><span data-stu-id="f0397-103">driveItem: preview</span></span>

<span data-ttu-id="f0397-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0397-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f0397-105">Это действие позволяет получить короткий URL-адрес, который можно внедрить для элемента, чтобы отобразить временный предварительный просмотр.</span><span class="sxs-lookup"><span data-stu-id="f0397-105">This action allows you to obtain a short-lived embeddable URL for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="f0397-106">Если вы хотите получить ссылки с большим сроком действия, используйте вместо этого API [CreateLink][] .</span><span class="sxs-lookup"><span data-stu-id="f0397-106">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="f0397-107">**Примечание:** В настоящее время действие **Предварительный просмотр** доступно только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f0397-107">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="f0397-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f0397-109">Permissions</span></span>

<span data-ttu-id="f0397-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0397-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f0397-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0397-112">Permission type</span></span>                        | <span data-ttu-id="f0397-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0397-113">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="f0397-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0397-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="f0397-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0397-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="f0397-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0397-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0397-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0397-117">Not supported.</span></span>
| <span data-ttu-id="f0397-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0397-118">Application</span></span>                            | <span data-ttu-id="f0397-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0397-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="f0397-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0397-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="f0397-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0397-121">Request body</span></span>

<span data-ttu-id="f0397-122">В теле запроса определяются свойства внедряемого URL-адреса, запрашиваемого приложением.</span><span class="sxs-lookup"><span data-stu-id="f0397-122">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="f0397-123">Запрос должен быть объектом JSON с указанными ниже свойствами.</span><span class="sxs-lookup"><span data-stu-id="f0397-123">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="f0397-124">Имя</span><span class="sxs-lookup"><span data-stu-id="f0397-124">Name</span></span>      |  <span data-ttu-id="f0397-125">Тип</span><span class="sxs-lookup"><span data-stu-id="f0397-125">Type</span></span>         | <span data-ttu-id="f0397-126">Описание</span><span class="sxs-lookup"><span data-stu-id="f0397-126">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="f0397-127">page</span><span class="sxs-lookup"><span data-stu-id="f0397-127">page</span></span>        | <span data-ttu-id="f0397-128">строка или число</span><span class="sxs-lookup"><span data-stu-id="f0397-128">string/number</span></span> | <span data-ttu-id="f0397-129">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="f0397-129">Optional.</span></span> <span data-ttu-id="f0397-130">Номер страницы для начала документа, если это необходимо.</span><span class="sxs-lookup"><span data-stu-id="f0397-130">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="f0397-131">Указывается как строка для будущих случаев использования для типов файлов, таких как ZIP.</span><span class="sxs-lookup"><span data-stu-id="f0397-131">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="f0397-132">zoom</span><span class="sxs-lookup"><span data-stu-id="f0397-132">zoom</span></span>        | <span data-ttu-id="f0397-133">number</span><span class="sxs-lookup"><span data-stu-id="f0397-133">number</span></span>        | <span data-ttu-id="f0397-134">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f0397-134">Optional.</span></span> <span data-ttu-id="f0397-135">Масштаб (при необходимости) для запуска.</span><span class="sxs-lookup"><span data-stu-id="f0397-135">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="f0397-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0397-136">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="f0397-137">Ответом будет объект JSON, содержащий следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="f0397-137">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="f0397-138">Имя</span><span class="sxs-lookup"><span data-stu-id="f0397-138">Name</span></span>           | <span data-ttu-id="f0397-139">Тип</span><span class="sxs-lookup"><span data-stu-id="f0397-139">Type</span></span>   | <span data-ttu-id="f0397-140">Описание</span><span class="sxs-lookup"><span data-stu-id="f0397-140">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="f0397-141">Команда</span><span class="sxs-lookup"><span data-stu-id="f0397-141">getUrl</span></span>         | <span data-ttu-id="f0397-142">string</span><span class="sxs-lookup"><span data-stu-id="f0397-142">string</span></span> | <span data-ttu-id="f0397-143">URL-адрес, подходящие для внедрения с помощью HTTP GET (Iframes и т. д.)</span><span class="sxs-lookup"><span data-stu-id="f0397-143">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="f0397-144">постурл</span><span class="sxs-lookup"><span data-stu-id="f0397-144">postUrl</span></span>        | <span data-ttu-id="f0397-145">string</span><span class="sxs-lookup"><span data-stu-id="f0397-145">string</span></span> | <span data-ttu-id="f0397-146">URL-адрес, подходящий для внедрения с помощью HTTP POST (форма POST, JS и т. д.)</span><span class="sxs-lookup"><span data-stu-id="f0397-146">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="f0397-147">Параметры</span><span class="sxs-lookup"><span data-stu-id="f0397-147">postParameters</span></span> | <span data-ttu-id="f0397-148">string</span><span class="sxs-lookup"><span data-stu-id="f0397-148">string</span></span> | <span data-ttu-id="f0397-149">Параметры POST для включения при использовании Постурл</span><span class="sxs-lookup"><span data-stu-id="f0397-149">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="f0397-150">В зависимости от текущего состояния поддержки внедрения для заданных параметров может возвращаться либо getUrl, Постурл, либо и то, и другое.</span><span class="sxs-lookup"><span data-stu-id="f0397-150">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="f0397-151">i-параметры — это строка, отформатированная как `application/x-www-form-urlencoded` , и при выполнении POST для постурл Content-Type необходимо задать соответствующие параметры.</span><span class="sxs-lookup"><span data-stu-id="f0397-151">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="f0397-152">Пример.</span><span class="sxs-lookup"><span data-stu-id="f0397-152">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="f0397-153">Страница/масштаб</span><span class="sxs-lookup"><span data-stu-id="f0397-153">Page/zoom</span></span>

<span data-ttu-id="f0397-154">Параметры "Page" и "Zoom" могут быть недоступны для всех предварительных приложений, но будут применены, если это приложение поддерживает приложение Preview.</span><span class="sxs-lookup"><span data-stu-id="f0397-154">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>

