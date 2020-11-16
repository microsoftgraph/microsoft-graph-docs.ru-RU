---
title: Список устройств
description: Получение списка объектов устройств, зарегистрированных в организации.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 14ef2993f6dd7766846bb006d047cd4e2f90c615
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2020
ms.locfileid: "49082239"
---
# <a name="list-devices"></a><span data-ttu-id="765b9-103">Список устройств</span><span class="sxs-lookup"><span data-stu-id="765b9-103">List devices</span></span>

<span data-ttu-id="765b9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="765b9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="765b9-105">Получение списка объектов устройств, зарегистрированных в организации.</span><span class="sxs-lookup"><span data-stu-id="765b9-105">Retrieve a list of device objects registered in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="765b9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="765b9-106">Permissions</span></span>
<span data-ttu-id="765b9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="765b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="765b9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="765b9-109">Permission type</span></span>      | <span data-ttu-id="765b9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="765b9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="765b9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="765b9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="765b9-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="765b9-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="765b9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="765b9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="765b9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="765b9-114">Not supported.</span></span>    |
|<span data-ttu-id="765b9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="765b9-115">Application</span></span> | <span data-ttu-id="765b9-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="765b9-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="765b9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="765b9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="765b9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="765b9-118">Optional query parameters</span></span>

<span data-ttu-id="765b9-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="765b9-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="765b9-120">Вы можете использовать `$search` в свойствах **displayName** и **description**.</span><span class="sxs-lookup"><span data-stu-id="765b9-120">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="765b9-121">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="765b9-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="765b9-122">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="765b9-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="765b9-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="765b9-123">Request headers</span></span>

| <span data-ttu-id="765b9-124">Имя</span><span class="sxs-lookup"><span data-stu-id="765b9-124">Name</span></span>       |  <span data-ttu-id="765b9-125">Описание</span><span class="sxs-lookup"><span data-stu-id="765b9-125">Description</span></span>|
|:-----------|:------------|
| <span data-ttu-id="765b9-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="765b9-126">Authorization</span></span>  | <span data-ttu-id="765b9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="765b9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="765b9-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="765b9-129">ConsistencyLevel</span></span> | <span data-ttu-id="765b9-130">необязательный.</span><span class="sxs-lookup"><span data-stu-id="765b9-130">eventual.</span></span> <span data-ttu-id="765b9-131">Этот заголовок и `$count` требуются при использовании `$search`или применении `$filter` с параметром запроса `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="765b9-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="765b9-132">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="765b9-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="765b9-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="765b9-133">Request body</span></span>
<span data-ttu-id="765b9-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="765b9-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="765b9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="765b9-135">Response</span></span>

<span data-ttu-id="765b9-136">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="765b9-136">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="765b9-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="765b9-137">Examples</span></span>

### <a name="example-1-get-a-list-of-devices"></a><span data-ttu-id="765b9-138">Пример 1: получение списка устройств</span><span class="sxs-lookup"><span data-stu-id="765b9-138">Example 1: Get a list of devices</span></span>

#### <a name="request"></a><span data-ttu-id="765b9-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="765b9-139">Request</span></span>

<span data-ttu-id="765b9-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="765b9-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="765b9-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="765b9-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices
```
# <a name="c"></a>[<span data-ttu-id="765b9-142">C#</span><span class="sxs-lookup"><span data-stu-id="765b9-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="765b9-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="765b9-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="765b9-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="765b9-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="765b9-145">Java</span><span class="sxs-lookup"><span data-stu-id="765b9-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="765b9-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="765b9-146">Response</span></span>

<span data-ttu-id="765b9-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="765b9-147">The following is an example of the response.</span></span>

> <span data-ttu-id="765b9-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="765b9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-devices"></a><span data-ttu-id="765b9-150">Пример 2: получение только количества устройств</span><span class="sxs-lookup"><span data-stu-id="765b9-150">Example 2: Get only a count of devices</span></span>

#### <a name="request"></a><span data-ttu-id="765b9-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="765b9-151">Request</span></span>

<span data-ttu-id="765b9-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="765b9-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="765b9-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="765b9-153">Response</span></span>

<span data-ttu-id="765b9-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="765b9-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-3-use-filter-and-top-to-get-one-device-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="765b9-155">Пример 3: используйте $filter и $top, чтобы получить одно устройство с отображаемым именем, начинающимся с "a", включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="765b9-155">Example 3: Use $filter and $top to get one device with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="765b9-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="765b9-156">Request</span></span>

<span data-ttu-id="765b9-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="765b9-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="765b9-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="765b9-158">Response</span></span>

<span data-ttu-id="765b9-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="765b9-159">The following is an example of the response.</span></span>

><span data-ttu-id="765b9-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="765b9-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#devices",
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

### <a name="example-4-use-search-to-get-devices-with-display-names-that-contain-the-letters-android-including-a-count-of-returned-objects"></a><span data-ttu-id="765b9-162">Пример 4: использование $search для получения устройств с отображаемыми именами, которые содержат буквы "Android", включая число возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="765b9-162">Example 4: Use $search to get devices with display names that contain the letters 'Android' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="765b9-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="765b9-163">Request</span></span>

<span data-ttu-id="765b9-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="765b9-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_android_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices?$search="displayName:Android"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="765b9-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="765b9-165">Response</span></span>

<span data-ttu-id="765b9-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="765b9-166">The following is an example of the response.</span></span>

><span data-ttu-id="765b9-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="765b9-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#devices",
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
}-->
