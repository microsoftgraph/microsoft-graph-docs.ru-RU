---
title: 'driveItem: предварительный просмотр'
description: Это действие позволяет получать кратковременного встраиваемые URL-адреса для элемента для визуализации временные предварительного просмотра.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ae5140bf6164aedd051f04c2c43c361f16517e7a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986077"
---
# <a name="driveitem-preview"></a><span data-ttu-id="ed464-103">driveItem: предварительный просмотр</span><span class="sxs-lookup"><span data-stu-id="ed464-103">driveItem: preview</span></span>

<span data-ttu-id="ed464-104">Это действие позволяет получать кратковременного встраиваемые URL-адреса для элемента для визуализации временные предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="ed464-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="ed464-105">Если вы хотите получить длинные встраиваемые ссылки, используйте [команду createLink][] API.</span><span class="sxs-lookup"><span data-stu-id="ed464-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="ed464-106">**Примечание:** Действие **предварительного просмотра** в данный момент доступна только на сервере SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="ed464-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[команду createLink]: driveitem-createlink.md
[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="ed464-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed464-108">Permissions</span></span>

<span data-ttu-id="ed464-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed464-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed464-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed464-111">Permission type</span></span>                        | <span data-ttu-id="ed464-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed464-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="ed464-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed464-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed464-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed464-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="ed464-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed464-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed464-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed464-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="ed464-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed464-117">Application</span></span>                            | <span data-ttu-id="ed464-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed464-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="ed464-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed464-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="ed464-120">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ed464-120">Request body</span></span>

<span data-ttu-id="ed464-121">Текст запроса определяет свойства встраиваемые URL-адреса, запрашивающего приложения.</span><span class="sxs-lookup"><span data-stu-id="ed464-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="ed464-122">Запрос должен быть объектом JSON с указанными ниже свойствами.</span><span class="sxs-lookup"><span data-stu-id="ed464-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="ed464-123">Имя</span><span class="sxs-lookup"><span data-stu-id="ed464-123">Name</span></span>      |  <span data-ttu-id="ed464-124">Тип</span><span class="sxs-lookup"><span data-stu-id="ed464-124">Type</span></span>         | <span data-ttu-id="ed464-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ed464-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="ed464-126">page</span><span class="sxs-lookup"><span data-stu-id="ed464-126">page</span></span>        | <span data-ttu-id="ed464-127">Строка или номер</span><span class="sxs-lookup"><span data-stu-id="ed464-127">string/number</span></span> | <span data-ttu-id="ed464-128">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="ed464-128">Optional.</span></span> <span data-ttu-id="ed464-129">Номер документа для запуска, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="ed464-129">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="ed464-130">Указан как строка для использования в будущем случаев вокруг типов файлов, например ZIP.</span><span class="sxs-lookup"><span data-stu-id="ed464-130">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="ed464-131">zoom</span><span class="sxs-lookup"><span data-stu-id="ed464-131">zoom</span></span>        | <span data-ttu-id="ed464-132">число</span><span class="sxs-lookup"><span data-stu-id="ed464-132">number</span></span>        | <span data-ttu-id="ed464-133">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="ed464-133">Optional.</span></span> <span data-ttu-id="ed464-134">Выбор масштаба для запуска, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="ed464-134">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="ed464-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="ed464-135">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="ed464-136">Ответ будет объект JSON, который содержит следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="ed464-136">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="ed464-137">Имя</span><span class="sxs-lookup"><span data-stu-id="ed464-137">Name</span></span>           | <span data-ttu-id="ed464-138">Тип</span><span class="sxs-lookup"><span data-stu-id="ed464-138">Type</span></span>   | <span data-ttu-id="ed464-139">Описание</span><span class="sxs-lookup"><span data-stu-id="ed464-139">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="ed464-140">getUrl</span><span class="sxs-lookup"><span data-stu-id="ed464-140">getUrl</span></span>         | <span data-ttu-id="ed464-141">строка</span><span class="sxs-lookup"><span data-stu-id="ed464-141">string</span></span> | <span data-ttu-id="ed464-142">URL-адрес для внедрения с помощью HTTP GET (Интернет-кадров, и т.д.)</span><span class="sxs-lookup"><span data-stu-id="ed464-142">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="ed464-143">postUrl</span><span class="sxs-lookup"><span data-stu-id="ed464-143">postUrl</span></span>        | <span data-ttu-id="ed464-144">строка</span><span class="sxs-lookup"><span data-stu-id="ed464-144">string</span></span> | <span data-ttu-id="ed464-145">URL-адрес для внедрения с помощью HTTP POST (отправки формы, JS, и т.д.)</span><span class="sxs-lookup"><span data-stu-id="ed464-145">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="ed464-146">postParameters</span><span class="sxs-lookup"><span data-stu-id="ed464-146">postParameters</span></span> | <span data-ttu-id="ed464-147">строка</span><span class="sxs-lookup"><span data-stu-id="ed464-147">string</span></span> | <span data-ttu-id="ed464-148">Параметры отправки для включения при использовании postUrl</span><span class="sxs-lookup"><span data-stu-id="ed464-148">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="ed464-149">В зависимости от текущего состояния внедрить поддержку указанные параметры могут возвращаться getUrl, postUrl или оба.</span><span class="sxs-lookup"><span data-stu-id="ed464-149">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="ed464-150">postParameters — это строка в формате `application/x-www-form-urlencoded`, и, если для выполнения ОТПРАВКУ postUrl типа контента необходимо задать соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="ed464-150">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="ed464-151">Примеры:</span><span class="sxs-lookup"><span data-stu-id="ed464-151">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="ed464-152">Масштаб страницы /</span><span class="sxs-lookup"><span data-stu-id="ed464-152">Page/zoom</span></span>

<span data-ttu-id="ed464-153">«Страница» и «отобразить» параметры могут быть недоступны для всех приложений предварительного просмотра, но будет применяться, если версия приложения поддерживает его.</span><span class="sxs-lookup"><span data-stu-id="ed464-153">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
