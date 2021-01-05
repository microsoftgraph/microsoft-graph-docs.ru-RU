---
title: Список устройств
description: 'Получение списка устройств, зарегистрированных в каталоге. '
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: eeb80864abfd8e198093d839930bc37065c5fd4d
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752782"
---
# <a name="list-devices"></a><span data-ttu-id="64275-103">Список устройств</span><span class="sxs-lookup"><span data-stu-id="64275-103">List devices</span></span>

<span data-ttu-id="64275-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64275-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64275-105">Получение списка устройств, зарегистрированных в каталоге.</span><span class="sxs-lookup"><span data-stu-id="64275-105">Retrieve a list of devices registered in the directory.</span></span> 

## <a name="permissions"></a><span data-ttu-id="64275-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64275-106">Permissions</span></span>

<span data-ttu-id="64275-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64275-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="64275-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64275-109">Permission type</span></span> | <span data-ttu-id="64275-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64275-110">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="64275-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64275-111">Delegated (work or school account)</span></span> | <span data-ttu-id="64275-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="64275-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="64275-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64275-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64275-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64275-114">Not supported.</span></span> |
| <span data-ttu-id="64275-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="64275-115">Application</span></span> | <span data-ttu-id="64275-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64275-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64275-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64275-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64275-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="64275-118">Optional query parameters</span></span>

<span data-ttu-id="64275-119">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="64275-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="64275-120">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="64275-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="64275-121">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="64275-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="64275-122">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="64275-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64275-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64275-123">Request headers</span></span>

| <span data-ttu-id="64275-124">Имя</span><span class="sxs-lookup"><span data-stu-id="64275-124">Name</span></span> | <span data-ttu-id="64275-125">Описание</span><span class="sxs-lookup"><span data-stu-id="64275-125">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="64275-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64275-126">Authorization</span></span>  | <span data-ttu-id="64275-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64275-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="64275-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="64275-129">ConsistencyLevel</span></span> | <span data-ttu-id="64275-130">необязательный.</span><span class="sxs-lookup"><span data-stu-id="64275-130">eventual.</span></span> <span data-ttu-id="64275-131">Этот заголовок и `$count` требуются при использовании `$search`или применении `$filter` с параметром запроса `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="64275-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="64275-132">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="64275-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64275-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64275-133">Request body</span></span>

<span data-ttu-id="64275-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64275-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64275-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="64275-135">Response</span></span>

<span data-ttu-id="64275-136">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="64275-136">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64275-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="64275-137">Examples</span></span>

### <a name="example-1-get-a-list-of-devices"></a><span data-ttu-id="64275-138">Пример 1. Получить список устройств</span><span class="sxs-lookup"><span data-stu-id="64275-138">Example 1: Get a list of devices</span></span>

#### <a name="request"></a><span data-ttu-id="64275-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="64275-139">Request</span></span>

<span data-ttu-id="64275-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64275-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="64275-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="64275-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices
```
# <a name="c"></a>[<span data-ttu-id="64275-142">C#</span><span class="sxs-lookup"><span data-stu-id="64275-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64275-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64275-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64275-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64275-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64275-145">Java</span><span class="sxs-lookup"><span data-stu-id="64275-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="64275-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="64275-146">Response</span></span>

<span data-ttu-id="64275-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="64275-147">Here is an example of the response.</span></span>
> <span data-ttu-id="64275-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64275-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-devices"></a><span data-ttu-id="64275-150">Пример 2. Получите только количество устройств</span><span class="sxs-lookup"><span data-stu-id="64275-150">Example 2: Get only a count of devices</span></span>

#### <a name="request"></a><span data-ttu-id="64275-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="64275-151">Request</span></span>

<span data-ttu-id="64275-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64275-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="64275-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="64275-153">Response</span></span>

<span data-ttu-id="64275-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="64275-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="64275-155">294</span><span class="sxs-lookup"><span data-stu-id="64275-155">294</span></span>

### <a name="example-3-use-filter-and-top-to-get-one-device-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="64275-156">Пример 3. Используйте $filter и $top, чтобы получить одно устройство с отображаемой именем, которое начинается с "a", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="64275-156">Example 3: Use $filter and $top to get one device with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="64275-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="64275-157">Request</span></span>

<span data-ttu-id="64275-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64275-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="64275-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="64275-159">Response</span></span>

<span data-ttu-id="64275-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="64275-160">The following is an example of the response.</span></span>
><span data-ttu-id="64275-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64275-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "operatingSystemVersion":"10.0",
      "hostNames":[]
    },
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000001",
      "deviceVersion":1,
      "displayName":"a_device_1",
      "Manufacturer":"Microsoft",
      "Model":"Surface",
      "operatingSystemVersion":"windows10EnterpriseN",
      "hostNames":["device_1.contoso.onmicrosoft.com", "device_1"]
    }
  ]
}
```

### <a name="example-4-use-search-to-get-devices-with-display-names-that-contain-the-letters-android-including-a-count-of-returned-objects"></a><span data-ttu-id="64275-163">Пример 4. Использование $search для получения устройств с отображаемой и отображаемой именами, которые содержат буквы "Android", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="64275-163">Example 4: Use $search to get devices with display names that contain the letters 'Android' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="64275-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="64275-164">Request</span></span>

<span data-ttu-id="64275-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64275-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$search="displayName:Android"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="64275-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="64275-166">Response</span></span>

<span data-ttu-id="64275-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="64275-167">The following is an example of the response.</span></span>
><span data-ttu-id="64275-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64275-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "operatingSystemVersion":"10.0",
      "hostNames":[]
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


