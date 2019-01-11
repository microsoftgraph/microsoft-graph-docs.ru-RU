---
title: 'driveItem: предварительный просмотр'
description: Это действие позволяет получать кратковременного встраиваемые URL-адреса для элемента для визуализации временные предварительного просмотра.
localization_priority: Normal
ms.openlocfilehash: c04a73d514dfb5a92030c4c2016579d469063f9d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850773"
---
# <a name="driveitem-preview"></a><span data-ttu-id="350cd-103">driveItem: предварительный просмотр</span><span class="sxs-lookup"><span data-stu-id="350cd-103">driveItem: preview</span></span>

<span data-ttu-id="350cd-104">Это действие позволяет получать кратковременного встраиваемые URL-адреса для элемента для визуализации временные предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="350cd-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="350cd-105">Если вы хотите получить длинные встраиваемые ссылки, используйте [команду createLink][] API.</span><span class="sxs-lookup"><span data-stu-id="350cd-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="350cd-106">**Примечание:** Действие **предварительного просмотра** в данный момент доступна только на сервере SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="350cd-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[команду createLink]: driveitem-createlink.md
[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="350cd-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="350cd-108">Permissions</span></span>

<span data-ttu-id="350cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="350cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="350cd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="350cd-111">Permission type</span></span>                        | <span data-ttu-id="350cd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="350cd-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="350cd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="350cd-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="350cd-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="350cd-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="350cd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="350cd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="350cd-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="350cd-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="350cd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="350cd-117">Application</span></span>                            | <span data-ttu-id="350cd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="350cd-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="350cd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="350cd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="350cd-120">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="350cd-120">Request body</span></span>

<span data-ttu-id="350cd-121">Текст запроса определяет свойства встраиваемые URL-адреса, запрашивающего приложения.</span><span class="sxs-lookup"><span data-stu-id="350cd-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="350cd-122">Запрос должен быть объектом JSON с указанными ниже свойствами.</span><span class="sxs-lookup"><span data-stu-id="350cd-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="350cd-123">Имя</span><span class="sxs-lookup"><span data-stu-id="350cd-123">Name</span></span>      |  <span data-ttu-id="350cd-124">Тип</span><span class="sxs-lookup"><span data-stu-id="350cd-124">Type</span></span>         | <span data-ttu-id="350cd-125">Описание</span><span class="sxs-lookup"><span data-stu-id="350cd-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="350cd-126">page</span><span class="sxs-lookup"><span data-stu-id="350cd-126">page</span></span>        | <span data-ttu-id="350cd-127">Строка или номер</span><span class="sxs-lookup"><span data-stu-id="350cd-127">string/number</span></span> | <span data-ttu-id="350cd-128">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="350cd-128">Optional.</span></span> <span data-ttu-id="350cd-129">Номер документа для запуска, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="350cd-129">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="350cd-130">Указан как строка для использования в будущем случаев вокруг типов файлов, например ZIP.</span><span class="sxs-lookup"><span data-stu-id="350cd-130">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="350cd-131">zoom</span><span class="sxs-lookup"><span data-stu-id="350cd-131">zoom</span></span>        | <span data-ttu-id="350cd-132">число</span><span class="sxs-lookup"><span data-stu-id="350cd-132">number</span></span>        | <span data-ttu-id="350cd-133">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="350cd-133">Optional.</span></span> <span data-ttu-id="350cd-134">Выбор масштаба для запуска, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="350cd-134">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="350cd-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="350cd-135">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="350cd-136">Ответ будет объект JSON, который содержит следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="350cd-136">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="350cd-137">Имя</span><span class="sxs-lookup"><span data-stu-id="350cd-137">Name</span></span>           | <span data-ttu-id="350cd-138">Тип</span><span class="sxs-lookup"><span data-stu-id="350cd-138">Type</span></span>   | <span data-ttu-id="350cd-139">Описание</span><span class="sxs-lookup"><span data-stu-id="350cd-139">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="350cd-140">getUrl</span><span class="sxs-lookup"><span data-stu-id="350cd-140">getUrl</span></span>         | <span data-ttu-id="350cd-141">string</span><span class="sxs-lookup"><span data-stu-id="350cd-141">string</span></span> | <span data-ttu-id="350cd-142">URL-адрес для внедрения с помощью HTTP GET (Интернет-кадров, и т.д.)</span><span class="sxs-lookup"><span data-stu-id="350cd-142">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="350cd-143">postUrl</span><span class="sxs-lookup"><span data-stu-id="350cd-143">postUrl</span></span>        | <span data-ttu-id="350cd-144">string</span><span class="sxs-lookup"><span data-stu-id="350cd-144">string</span></span> | <span data-ttu-id="350cd-145">URL-адрес для внедрения с помощью HTTP POST (отправки формы, JS, и т.д.)</span><span class="sxs-lookup"><span data-stu-id="350cd-145">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="350cd-146">postParameters</span><span class="sxs-lookup"><span data-stu-id="350cd-146">postParameters</span></span> | <span data-ttu-id="350cd-147">string</span><span class="sxs-lookup"><span data-stu-id="350cd-147">string</span></span> | <span data-ttu-id="350cd-148">Параметры отправки для включения при использовании postUrl</span><span class="sxs-lookup"><span data-stu-id="350cd-148">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="350cd-149">В зависимости от текущего состояния внедрить поддержку указанные параметры могут возвращаться getUrl, postUrl или оба.</span><span class="sxs-lookup"><span data-stu-id="350cd-149">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="350cd-150">postParameters — это строка в формате `application/x-www-form-urlencoded`, и, если для выполнения ОТПРАВКУ postUrl типа контента необходимо задать соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="350cd-150">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="350cd-151">Пример:</span><span class="sxs-lookup"><span data-stu-id="350cd-151">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="350cd-152">Масштаб страницы /</span><span class="sxs-lookup"><span data-stu-id="350cd-152">Page/zoom</span></span>

<span data-ttu-id="350cd-153">«Страница» и «отобразить» параметры могут быть недоступны для всех приложений предварительного просмотра, но будет применяться, если версия приложения поддерживает его.</span><span class="sxs-lookup"><span data-stu-id="350cd-153">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
