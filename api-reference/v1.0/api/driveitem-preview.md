---
title: 'driveItem: Preview'
description: Это действие позволяет получать кратковременно недопустимые URL-адреса для встраиваемых элементов, чтобы отобразить временный предварительный просмотр.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ae5140bf6164aedd051f04c2c43c361f16517e7a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572705"
---
# <a name="driveitem-preview"></a><span data-ttu-id="541db-103">driveItem: Preview</span><span class="sxs-lookup"><span data-stu-id="541db-103">driveItem: preview</span></span>

<span data-ttu-id="541db-104">Это действие позволяет получать кратковременно недопустимые URL-адреса для встраиваемых элементов, чтобы отобразить временный предварительный просмотр.</span><span class="sxs-lookup"><span data-stu-id="541db-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="541db-105">Если вы хотите получить ссылки с большим сроком действия, используйте вместо этого API [CreateLink][] .</span><span class="sxs-lookup"><span data-stu-id="541db-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="541db-106">**Примечание:** В настоящее время действие **Предварительный просмотр** доступно только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="541db-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="541db-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="541db-108">Permissions</span></span>

<span data-ttu-id="541db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="541db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="541db-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="541db-111">Permission type</span></span>                        | <span data-ttu-id="541db-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="541db-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="541db-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="541db-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="541db-114">Files. Read, Files. ReadWrite, Files. ReadWrite. ALL, sites. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="541db-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="541db-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="541db-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="541db-116">Files. Read, Files. ReadWrite, Files. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="541db-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="541db-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="541db-117">Application</span></span>                            | <span data-ttu-id="541db-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="541db-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="541db-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="541db-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="541db-120">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="541db-120">Request body</span></span>

<span data-ttu-id="541db-121">В теле запроса определяются свойства внедряемого URL-адреса, запрашиваемого приложением.</span><span class="sxs-lookup"><span data-stu-id="541db-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="541db-122">Запрос должен быть объектом JSON с указанными ниже свойствами.</span><span class="sxs-lookup"><span data-stu-id="541db-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="541db-123">Имя</span><span class="sxs-lookup"><span data-stu-id="541db-123">Name</span></span>      |  <span data-ttu-id="541db-124">Тип</span><span class="sxs-lookup"><span data-stu-id="541db-124">Type</span></span>         | <span data-ttu-id="541db-125">Описание</span><span class="sxs-lookup"><span data-stu-id="541db-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="541db-126">page</span><span class="sxs-lookup"><span data-stu-id="541db-126">page</span></span>        | <span data-ttu-id="541db-127">строка или число</span><span class="sxs-lookup"><span data-stu-id="541db-127">string/number</span></span> | <span data-ttu-id="541db-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="541db-128">Optional.</span></span> <span data-ttu-id="541db-129">Номер страницы для начала документа, если это необходимо.</span><span class="sxs-lookup"><span data-stu-id="541db-129">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="541db-130">Указывается как строка для будущих случаев использования для типов файлов, таких как ZIP.</span><span class="sxs-lookup"><span data-stu-id="541db-130">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="541db-131">zoom</span><span class="sxs-lookup"><span data-stu-id="541db-131">zoom</span></span>        | <span data-ttu-id="541db-132">number</span><span class="sxs-lookup"><span data-stu-id="541db-132">number</span></span>        | <span data-ttu-id="541db-133">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="541db-133">Optional.</span></span> <span data-ttu-id="541db-134">Масштаб (при необходимости) для запуска.</span><span class="sxs-lookup"><span data-stu-id="541db-134">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="541db-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="541db-135">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="541db-136">Ответом будет объект JSON, содержащий следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="541db-136">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="541db-137">Имя</span><span class="sxs-lookup"><span data-stu-id="541db-137">Name</span></span>           | <span data-ttu-id="541db-138">Тип</span><span class="sxs-lookup"><span data-stu-id="541db-138">Type</span></span>   | <span data-ttu-id="541db-139">Описание</span><span class="sxs-lookup"><span data-stu-id="541db-139">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="541db-140">Команда</span><span class="sxs-lookup"><span data-stu-id="541db-140">getUrl</span></span>         | <span data-ttu-id="541db-141">string</span><span class="sxs-lookup"><span data-stu-id="541db-141">string</span></span> | <span data-ttu-id="541db-142">URL-адрес, подходящие для внедрения с помощью HTTP GET (Iframes и т. д.)</span><span class="sxs-lookup"><span data-stu-id="541db-142">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="541db-143">Постурл</span><span class="sxs-lookup"><span data-stu-id="541db-143">postUrl</span></span>        | <span data-ttu-id="541db-144">string</span><span class="sxs-lookup"><span data-stu-id="541db-144">string</span></span> | <span data-ttu-id="541db-145">URL-адрес, подходящий для внедрения с помощью HTTP POST (форма POST, JS и т. д.)</span><span class="sxs-lookup"><span data-stu-id="541db-145">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="541db-146">Параметры</span><span class="sxs-lookup"><span data-stu-id="541db-146">postParameters</span></span> | <span data-ttu-id="541db-147">string</span><span class="sxs-lookup"><span data-stu-id="541db-147">string</span></span> | <span data-ttu-id="541db-148">Параметры POST для включения при использовании Постурл</span><span class="sxs-lookup"><span data-stu-id="541db-148">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="541db-149">В зависимости от текущего состояния поддержки внедрения для заданных параметров может возвращаться либо getUrl, Постурл, либо и то, и другое.</span><span class="sxs-lookup"><span data-stu-id="541db-149">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="541db-150">i-параметры — это строка, `application/x-www-form-urlencoded`отформатированная как, и при выполнении POST для постурл Content-Type необходимо задать соответствующие параметры.</span><span class="sxs-lookup"><span data-stu-id="541db-150">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="541db-151">Примеры:</span><span class="sxs-lookup"><span data-stu-id="541db-151">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="541db-152">Страница/масштаб</span><span class="sxs-lookup"><span data-stu-id="541db-152">Page/zoom</span></span>

<span data-ttu-id="541db-153">Параметры "Page" и "Zoom" могут быть недоступны для всех предварительных приложений, но будут применены, если это приложение поддерживает приложение Preview.</span><span class="sxs-lookup"><span data-stu-id="541db-153">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
