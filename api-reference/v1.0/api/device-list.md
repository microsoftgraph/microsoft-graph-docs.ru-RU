---
title: Список устройств
description: Получение списка объектов устройств, зарегистрированных в организации.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 8f17537315e97efb99837a9333cf5821818007ec
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039729"
---
# <a name="list-devices"></a><span data-ttu-id="deb19-103">Список устройств</span><span class="sxs-lookup"><span data-stu-id="deb19-103">List devices</span></span>

<span data-ttu-id="deb19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deb19-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="deb19-105">Получение списка объектов устройств, зарегистрированных в организации.</span><span class="sxs-lookup"><span data-stu-id="deb19-105">Retrieve a list of device objects registered in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="deb19-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="deb19-106">Permissions</span></span>
<span data-ttu-id="deb19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="deb19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="deb19-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="deb19-109">Permission type</span></span>      | <span data-ttu-id="deb19-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="deb19-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="deb19-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="deb19-111">Delegated (work or school account)</span></span> | <span data-ttu-id="deb19-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="deb19-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="deb19-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="deb19-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="deb19-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="deb19-114">Not supported.</span></span>    |
|<span data-ttu-id="deb19-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="deb19-115">Application</span></span> | <span data-ttu-id="deb19-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deb19-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="deb19-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="deb19-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="deb19-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="deb19-118">Optional query parameters</span></span>

<span data-ttu-id="deb19-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа, в том числе `$search`, `$count` і `$filter`.</span><span class="sxs-lookup"><span data-stu-id="deb19-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="deb19-120">Вы можете использовать `$search` в свойствах **displayName** и **description**.</span><span class="sxs-lookup"><span data-stu-id="deb19-120">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="deb19-121">Когда элементы добавляются или обновляются для этого ресурса, они специально индексируются для использования с помощью параметров `$count` и `$search`.</span><span class="sxs-lookup"><span data-stu-id="deb19-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="deb19-122">Между добавлением или обновлением элемента и его появлением в индексе может возникать небольшая задержка.</span><span class="sxs-lookup"><span data-stu-id="deb19-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="deb19-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="deb19-123">Request headers</span></span>

| <span data-ttu-id="deb19-124">Имя</span><span class="sxs-lookup"><span data-stu-id="deb19-124">Name</span></span>       |  <span data-ttu-id="deb19-125">Описание</span><span class="sxs-lookup"><span data-stu-id="deb19-125">Description</span></span>|
|:-----------|:------------|
| <span data-ttu-id="deb19-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="deb19-126">Authorization</span></span>  | <span data-ttu-id="deb19-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="deb19-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="deb19-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="deb19-129">ConsistencyLevel</span></span> | <span data-ttu-id="deb19-130">необязательный.</span><span class="sxs-lookup"><span data-stu-id="deb19-130">eventual.</span></span> <span data-ttu-id="deb19-131">Этот заголовок и `$count` требуются при использовании `$search`или применении `$filter` с параметром запроса `$orderby`.</span><span class="sxs-lookup"><span data-stu-id="deb19-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="deb19-132">В нем используется индекс, который может не соответствовать последним изменениям объекта.</span><span class="sxs-lookup"><span data-stu-id="deb19-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="deb19-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="deb19-133">Request body</span></span>
<span data-ttu-id="deb19-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="deb19-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="deb19-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="deb19-135">Response</span></span>

<span data-ttu-id="deb19-136">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="deb19-136">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="deb19-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="deb19-137">Examples</span></span>

### <a name="example-1-get-a-list-of-devices"></a><span data-ttu-id="deb19-138">Пример 1. Получить список устройств</span><span class="sxs-lookup"><span data-stu-id="deb19-138">Example 1: Get a list of devices</span></span>

#### <a name="request"></a><span data-ttu-id="deb19-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="deb19-139">Request</span></span>

<span data-ttu-id="deb19-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="deb19-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="deb19-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="deb19-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices
```
# <a name="c"></a>[<span data-ttu-id="deb19-142">C#</span><span class="sxs-lookup"><span data-stu-id="deb19-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="deb19-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="deb19-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="deb19-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="deb19-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="deb19-145">Java</span><span class="sxs-lookup"><span data-stu-id="deb19-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="deb19-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="deb19-146">Response</span></span>

<span data-ttu-id="deb19-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="deb19-147">The following is an example of the response.</span></span>

> <span data-ttu-id="deb19-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="deb19-148">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-devices"></a><span data-ttu-id="deb19-149">Пример 2. Получить только количество устройств</span><span class="sxs-lookup"><span data-stu-id="deb19-149">Example 2: Get only a count of devices</span></span>

#### <a name="request"></a><span data-ttu-id="deb19-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="deb19-150">Request</span></span>

<span data-ttu-id="deb19-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="deb19-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="deb19-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="deb19-152">Response</span></span>

<span data-ttu-id="deb19-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="deb19-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-3-use-filter-and-top-to-get-one-device-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="deb19-154">Пример 3. Использование $filter и $top для получения одного устройства с именем отображения, которое начинается с "a", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="deb19-154">Example 3: Use $filter and $top to get one device with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="deb19-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="deb19-155">Request</span></span>

<span data-ttu-id="deb19-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="deb19-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="deb19-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="deb19-157">Response</span></span>

<span data-ttu-id="deb19-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="deb19-158">The following is an example of the response.</span></span>

><span data-ttu-id="deb19-159">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="deb19-159">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-use-search-to-get-devices-with-display-names-that-contain-the-letters-android-including-a-count-of-returned-objects"></a><span data-ttu-id="deb19-160">Пример 4. Использование $search для получения устройств с именами отображения, которые содержат буквы "Android", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="deb19-160">Example 4: Use $search to get devices with display names that contain the letters 'Android' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="deb19-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="deb19-161">Request</span></span>

<span data-ttu-id="deb19-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="deb19-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_android_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices?$search="displayName:Android"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="deb19-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="deb19-163">Response</span></span>

<span data-ttu-id="deb19-164">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="deb19-164">The following is an example of the response.</span></span>

><span data-ttu-id="deb19-165">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="deb19-165">**Note:** The response object shown here might be shortened for readability.</span></span>

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
