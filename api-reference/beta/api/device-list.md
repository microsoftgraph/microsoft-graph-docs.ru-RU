---
title: Список устройств
description: 'Получение списка устройств, зарегистрированных в каталоге. '
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9f5ccff9b3c0bbfae164fbcb8abb7ea41a542ad0
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903862"
---
# <a name="list-devices"></a><span data-ttu-id="32072-103">Список устройств</span><span class="sxs-lookup"><span data-stu-id="32072-103">List devices</span></span>

<span data-ttu-id="32072-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32072-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32072-105">Получение списка устройств, зарегистрированных в каталоге.</span><span class="sxs-lookup"><span data-stu-id="32072-105">Retrieve a list of devices registered in the directory.</span></span> 

## <a name="permissions"></a><span data-ttu-id="32072-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32072-106">Permissions</span></span>

<span data-ttu-id="32072-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32072-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="32072-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32072-109">Permission type</span></span> | <span data-ttu-id="32072-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32072-110">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="32072-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32072-111">Delegated (work or school account)</span></span> | <span data-ttu-id="32072-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="32072-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="32072-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32072-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32072-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32072-114">Not supported.</span></span> |
| <span data-ttu-id="32072-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32072-115">Application</span></span> | <span data-ttu-id="32072-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32072-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="32072-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32072-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices
```

## <a name="optional-query-parameters"></a><span data-ttu-id="32072-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="32072-118">Optional query parameters</span></span>

<span data-ttu-id="32072-119">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="32072-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="32072-120">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="32072-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="32072-121">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="32072-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="32072-122">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="32072-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="32072-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32072-123">Request headers</span></span>

| <span data-ttu-id="32072-124">Имя</span><span class="sxs-lookup"><span data-stu-id="32072-124">Name</span></span> | <span data-ttu-id="32072-125">Описание</span><span class="sxs-lookup"><span data-stu-id="32072-125">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="32072-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32072-126">Authorization</span></span>  | <span data-ttu-id="32072-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32072-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="32072-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="32072-129">ConsistencyLevel</span></span> | <span data-ttu-id="32072-130">необязательный.</span><span class="sxs-lookup"><span data-stu-id="32072-130">eventual.</span></span> <span data-ttu-id="32072-131">Этот заголовок и `$count` требуются при использовании `$search`или применении `$filter` с параметром запроса `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="32072-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="32072-132">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="32072-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32072-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32072-133">Request body</span></span>

<span data-ttu-id="32072-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="32072-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32072-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="32072-135">Response</span></span>

<span data-ttu-id="32072-136">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="32072-136">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="32072-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="32072-137">Examples</span></span>

### <a name="example-1-get-a-list-of-devices"></a><span data-ttu-id="32072-138">Пример 1: получение списка устройств</span><span class="sxs-lookup"><span data-stu-id="32072-138">Example 1: Get a list of devices</span></span>

#### <a name="request"></a><span data-ttu-id="32072-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="32072-139">Request</span></span>

<span data-ttu-id="32072-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32072-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="32072-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="32072-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices
```
# <a name="c"></a>[<span data-ttu-id="32072-142">C#</span><span class="sxs-lookup"><span data-stu-id="32072-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32072-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32072-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32072-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32072-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="32072-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="32072-145">Response</span></span>

<span data-ttu-id="32072-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="32072-146">Here is an example of the response.</span></span>
> <span data-ttu-id="32072-p105">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32072-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000000",
      "deviceVersion":1,
      "displayName":"contoso_Android",
      "Manufacturer":"Google",
      "Model":"Pixel 3a",
      "operatingSystemVersion":"10.0"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-devices"></a><span data-ttu-id="32072-149">Пример 2: получение только количества устройств</span><span class="sxs-lookup"><span data-stu-id="32072-149">Example 2: Get only a count of devices</span></span>

#### <a name="request"></a><span data-ttu-id="32072-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="32072-150">Request</span></span>

<span data-ttu-id="32072-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32072-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="32072-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="32072-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="32072-153">C#</span><span class="sxs-lookup"><span data-stu-id="32072-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32072-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32072-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32072-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32072-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="32072-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="32072-156">Response</span></span>

<span data-ttu-id="32072-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="32072-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="32072-158">294</span><span class="sxs-lookup"><span data-stu-id="32072-158">294</span></span>

### <a name="example-3-use-filter-and-top-to-get-one-device-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="32072-159">Пример 3: используйте $filter и $top, чтобы получить одно устройство с отображаемым именем, начинающимся с "a", включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="32072-159">Example 3: Use $filter and $top to get one device with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="32072-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="32072-160">Request</span></span>

<span data-ttu-id="32072-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32072-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="32072-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="32072-162">Response</span></span>

<span data-ttu-id="32072-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="32072-163">The following is an example of the response.</span></span>
><span data-ttu-id="32072-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32072-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#devices",
  "@odata.count":1,
  "value":[
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000000",
      "deviceVersion":1,
      "displayName":"a_device_1",
      "Manufacturer":"Google",
      "Model":"Pixel 3a",
      "operatingSystemVersion":"10.0"
    }
  ]
}
```

### <a name="example-4-use-search-to-get-devices-with-display-names-that-contain-the-letters-android-including-a-count-of-returned-objects"></a><span data-ttu-id="32072-166">Пример 4: использование $search для получения устройств с отображаемыми именами, которые содержат буквы "Android", включая число возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="32072-166">Example 4: Use $search to get devices with display names that contain the letters 'Android' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="32072-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="32072-167">Request</span></span>

<span data-ttu-id="32072-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32072-168">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="32072-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="32072-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$search="displayName:Android"&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="32072-170">C#</span><span class="sxs-lookup"><span data-stu-id="32072-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32072-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32072-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32072-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32072-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="32072-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="32072-173">Response</span></span>

<span data-ttu-id="32072-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="32072-174">The following is an example of the response.</span></span>
><span data-ttu-id="32072-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32072-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#devices",
  "@odata.count":1396,
  "value":[
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000000",
      "deviceVersion":1,
      "displayName":"contoso_Android",
      "Manufacturer":"Google",
      "Model":"Pixel 3a",
      "operatingSystemVersion":"10.0"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


