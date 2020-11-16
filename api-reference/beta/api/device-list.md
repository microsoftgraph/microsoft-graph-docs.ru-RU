---
title: Список устройств
description: 'Получение списка устройств, зарегистрированных в каталоге. '
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2d0fe2403e04751a734da726d6f4c2cb6890813a
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2020
ms.locfileid: "49082019"
---
# <a name="list-devices"></a><span data-ttu-id="b6b0a-103">Список устройств</span><span class="sxs-lookup"><span data-stu-id="b6b0a-103">List devices</span></span>

<span data-ttu-id="b6b0a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6b0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6b0a-105">Получение списка устройств, зарегистрированных в каталоге.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-105">Retrieve a list of devices registered in the directory.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b6b0a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b6b0a-106">Permissions</span></span>

<span data-ttu-id="b6b0a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6b0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="b6b0a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6b0a-109">Permission type</span></span> | <span data-ttu-id="b6b0a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6b0a-110">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="b6b0a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6b0a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b6b0a-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b6b0a-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="b6b0a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6b0a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6b0a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-114">Not supported.</span></span> |
| <span data-ttu-id="b6b0a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6b0a-115">Application</span></span> | <span data-ttu-id="b6b0a-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6b0a-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6b0a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6b0a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6b0a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b6b0a-118">Optional query parameters</span></span>

<span data-ttu-id="b6b0a-119">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="b6b0a-120">`$search` можно использовать в свойстве **displayName**.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="b6b0a-121">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="b6b0a-122">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6b0a-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6b0a-123">Request headers</span></span>

| <span data-ttu-id="b6b0a-124">Имя</span><span class="sxs-lookup"><span data-stu-id="b6b0a-124">Name</span></span> | <span data-ttu-id="b6b0a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b6b0a-125">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="b6b0a-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6b0a-126">Authorization</span></span>  | <span data-ttu-id="b6b0a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b6b0a-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="b6b0a-129">ConsistencyLevel</span></span> | <span data-ttu-id="b6b0a-130">необязательный.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-130">eventual.</span></span> <span data-ttu-id="b6b0a-131">Этот заголовок и `$count` требуются при использовании `$search`или применении `$filter` с параметром запроса `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="b6b0a-132">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6b0a-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6b0a-133">Request body</span></span>

<span data-ttu-id="b6b0a-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6b0a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6b0a-135">Response</span></span>

<span data-ttu-id="b6b0a-136">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-136">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b6b0a-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="b6b0a-137">Examples</span></span>

### <a name="example-1-get-a-list-of-devices"></a><span data-ttu-id="b6b0a-138">Пример 1: получение списка устройств</span><span class="sxs-lookup"><span data-stu-id="b6b0a-138">Example 1: Get a list of devices</span></span>

#### <a name="request"></a><span data-ttu-id="b6b0a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6b0a-139">Request</span></span>

<span data-ttu-id="b6b0a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b6b0a-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6b0a-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices
```
# <a name="c"></a>[<span data-ttu-id="b6b0a-142">C#</span><span class="sxs-lookup"><span data-stu-id="b6b0a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6b0a-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6b0a-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6b0a-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6b0a-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6b0a-145">Java</span><span class="sxs-lookup"><span data-stu-id="b6b0a-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="b6b0a-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6b0a-146">Response</span></span>

<span data-ttu-id="b6b0a-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-147">Here is an example of the response.</span></span>
> <span data-ttu-id="b6b0a-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-devices"></a><span data-ttu-id="b6b0a-150">Пример 2: получение только количества устройств</span><span class="sxs-lookup"><span data-stu-id="b6b0a-150">Example 2: Get only a count of devices</span></span>

#### <a name="request"></a><span data-ttu-id="b6b0a-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6b0a-151">Request</span></span>

<span data-ttu-id="b6b0a-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b6b0a-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6b0a-153">Response</span></span>

<span data-ttu-id="b6b0a-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="b6b0a-155">294</span><span class="sxs-lookup"><span data-stu-id="b6b0a-155">294</span></span>

### <a name="example-3-use-filter-and-top-to-get-one-device-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="b6b0a-156">Пример 3: используйте $filter и $top, чтобы получить одно устройство с отображаемым именем, начинающимся с "a", включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-156">Example 3: Use $filter and $top to get one device with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="b6b0a-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6b0a-157">Request</span></span>

<span data-ttu-id="b6b0a-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b6b0a-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6b0a-159">Response</span></span>

<span data-ttu-id="b6b0a-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-160">The following is an example of the response.</span></span>
><span data-ttu-id="b6b0a-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-search-to-get-devices-with-display-names-that-contain-the-letters-android-including-a-count-of-returned-objects"></a><span data-ttu-id="b6b0a-163">Пример 4: использование $search для получения устройств с отображаемыми именами, которые содержат буквы "Android", включая число возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="b6b0a-163">Example 4: Use $search to get devices with display names that contain the letters 'Android' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="b6b0a-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6b0a-164">Request</span></span>

<span data-ttu-id="b6b0a-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$search="displayName:Android"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="b6b0a-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6b0a-166">Response</span></span>

<span data-ttu-id="b6b0a-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-167">The following is an example of the response.</span></span>
><span data-ttu-id="b6b0a-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b6b0a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


