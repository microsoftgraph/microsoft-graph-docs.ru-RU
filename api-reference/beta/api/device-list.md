---
title: Список устройств
description: 'Получение списка устройств, зарегистрированных в каталоге. '
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f032d3ce61f1f85ca3c7b4955d98b5159db5a5e1
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44287999"
---
# <a name="list-devices"></a><span data-ttu-id="f6767-103">Список устройств</span><span class="sxs-lookup"><span data-stu-id="f6767-103">List devices</span></span>

<span data-ttu-id="f6767-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6767-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6767-105">Получение списка устройств, зарегистрированных в каталоге.</span><span class="sxs-lookup"><span data-stu-id="f6767-105">Retrieve a list of devices registered in the directory.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f6767-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6767-106">Permissions</span></span>

<span data-ttu-id="f6767-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6767-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="f6767-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6767-109">Permission type</span></span> | <span data-ttu-id="f6767-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6767-110">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="f6767-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6767-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f6767-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f6767-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="f6767-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6767-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6767-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6767-114">Not supported.</span></span> |
| <span data-ttu-id="f6767-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6767-115">Application</span></span> | <span data-ttu-id="f6767-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6767-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6767-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6767-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6767-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f6767-118">Optional query parameters</span></span>

<span data-ttu-id="f6767-119">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа, включая `$search` , `$count` и `$filter` .</span><span class="sxs-lookup"><span data-stu-id="f6767-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="f6767-120">Можно использовать `$search` свойство **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="f6767-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="f6767-121">При добавлении или обновлении элементов для этого ресурса они могут индексироваться для использования с `$count` `$search` параметрами запроса.</span><span class="sxs-lookup"><span data-stu-id="f6767-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="f6767-122">Между добавлением или обновлением элемента может быть небольшая задержка, а когда он доступен в индексе.</span><span class="sxs-lookup"><span data-stu-id="f6767-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6767-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6767-123">Request headers</span></span>

| <span data-ttu-id="f6767-124">Имя</span><span class="sxs-lookup"><span data-stu-id="f6767-124">Name</span></span> | <span data-ttu-id="f6767-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f6767-125">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="f6767-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6767-126">Authorization</span></span>  | <span data-ttu-id="f6767-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6767-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f6767-129">консистенцилевел</span><span class="sxs-lookup"><span data-stu-id="f6767-129">ConsistencyLevel</span></span> | <span data-ttu-id="f6767-130">закончить.</span><span class="sxs-lookup"><span data-stu-id="f6767-130">eventual.</span></span> <span data-ttu-id="f6767-131">Этот заголовок и `$count` обязательные при использовании `$search` `$filter` с `$orderby` параметром Query.</span><span class="sxs-lookup"><span data-stu-id="f6767-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="f6767-132">Он использует индекс, который может быть не последним в актуальном изменении объекта.</span><span class="sxs-lookup"><span data-stu-id="f6767-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6767-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f6767-133">Request body</span></span>

<span data-ttu-id="f6767-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6767-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6767-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6767-135">Response</span></span>

<span data-ttu-id="f6767-136">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6767-136">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f6767-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="f6767-137">Examples</span></span>

### <a name="example-1-get-a-list-of-devices"></a><span data-ttu-id="f6767-138">Пример 1: получение списка устройств</span><span class="sxs-lookup"><span data-stu-id="f6767-138">Example 1: Get a list of devices</span></span>

#### <a name="request"></a><span data-ttu-id="f6767-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6767-139">Request</span></span>

<span data-ttu-id="f6767-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6767-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f6767-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6767-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices
```
# <a name="c"></a>[<span data-ttu-id="f6767-142">C#</span><span class="sxs-lookup"><span data-stu-id="f6767-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6767-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6767-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6767-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6767-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f6767-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6767-145">Response</span></span>

<span data-ttu-id="f6767-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f6767-146">Here is an example of the response.</span></span>
> <span data-ttu-id="f6767-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6767-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-devices"></a><span data-ttu-id="f6767-149">Пример 2: получение только количества устройств</span><span class="sxs-lookup"><span data-stu-id="f6767-149">Example 2: Get only a count of devices</span></span>

#### <a name="request"></a><span data-ttu-id="f6767-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6767-150">Request</span></span>

<span data-ttu-id="f6767-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6767-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="f6767-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6767-152">Response</span></span>

<span data-ttu-id="f6767-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f6767-153">The following is an example of the response.</span></span>

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

<span data-ttu-id="f6767-154">294</span><span class="sxs-lookup"><span data-stu-id="f6767-154">294</span></span>

### <a name="example-3-use-filter-and-top-to-get-one-device-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="f6767-155">Пример 3: используйте $filter и $top, чтобы получить одно устройство с отображаемым именем, начинающимся с "a", включая количество возвращаемых объектов.</span><span class="sxs-lookup"><span data-stu-id="f6767-155">Example 3: Use $filter and $top to get one device with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="f6767-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6767-156">Request</span></span>

<span data-ttu-id="f6767-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6767-157">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="f6767-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6767-158">Response</span></span>

<span data-ttu-id="f6767-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f6767-159">The following is an example of the response.</span></span>
><span data-ttu-id="f6767-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6767-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-search-to-get-devices-with-display-names-that-contain-the-letters-android-including-a-count-of-returned-objects"></a><span data-ttu-id="f6767-162">Пример 4: использование $search для получения устройств с отображаемыми именами, которые содержат буквы "Android", включая число возвращаемых объектов</span><span class="sxs-lookup"><span data-stu-id="f6767-162">Example 4: Use $search to get devices with display names that contain the letters 'Android' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="f6767-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6767-163">Request</span></span>

<span data-ttu-id="f6767-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6767-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$search="displayName:Android"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="f6767-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6767-165">Response</span></span>

<span data-ttu-id="f6767-166">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f6767-166">The following is an example of the response.</span></span>
><span data-ttu-id="f6767-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6767-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
