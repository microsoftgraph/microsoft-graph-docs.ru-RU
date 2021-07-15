---
title: Список устройств
description: 'Получение списка устройств, зарегистрированных в каталоге. '
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a045c9459a465eed05d35ecb63f4045ba71602de
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430065"
---
# <a name="list-devices"></a><span data-ttu-id="8c1ce-103">Список устройств</span><span class="sxs-lookup"><span data-stu-id="8c1ce-103">List devices</span></span>

<span data-ttu-id="8c1ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c1ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c1ce-105">Получение списка устройств, зарегистрированных в каталоге.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-105">Retrieve a list of devices registered in the directory.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8c1ce-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c1ce-106">Permissions</span></span>

<span data-ttu-id="8c1ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c1ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="8c1ce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c1ce-109">Permission type</span></span> | <span data-ttu-id="8c1ce-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c1ce-110">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="8c1ce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c1ce-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8c1ce-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8c1ce-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="8c1ce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c1ce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c1ce-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-114">Not supported.</span></span> |
| <span data-ttu-id="8c1ce-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8c1ce-115">Application</span></span> | <span data-ttu-id="8c1ce-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c1ce-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c1ce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c1ce-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c1ce-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8c1ce-118">Optional query parameters</span></span>

<span data-ttu-id="8c1ce-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select` и `$top` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-119">This method supports the `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="8c1ce-120">Некоторые запросы поддерживаются только при использовании заголовка **ConsistencyLevel** с присвоенным значением `eventual` и `$count`.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-120">Some queries are supported only when you use the **ConsistencyLevel** header set to `eventual` and `$count`.</span></span> <span data-ttu-id="8c1ce-121">Дополнительные сведения см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="8c1ce-121">For more information, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c1ce-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c1ce-122">Request headers</span></span>

| <span data-ttu-id="8c1ce-123">Имя</span><span class="sxs-lookup"><span data-stu-id="8c1ce-123">Name</span></span> | <span data-ttu-id="8c1ce-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8c1ce-124">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="8c1ce-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c1ce-125">Authorization</span></span>  | <span data-ttu-id="8c1ce-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8c1ce-128">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="8c1ce-128">ConsistencyLevel</span></span> | <span data-ttu-id="8c1ce-129">необязательный.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-129">eventual.</span></span> <span data-ttu-id="8c1ce-130">Этот заголовок и `$count` требуются при использовании `$search` или определенном использовании `$filter`.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-130">This header and `$count` are required when using `$search`, or in specific usage of `$filter`.</span></span> <span data-ttu-id="8c1ce-131">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="8c1ce-131">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c1ce-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c1ce-132">Request body</span></span>

<span data-ttu-id="8c1ce-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c1ce-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c1ce-134">Response</span></span>

<span data-ttu-id="8c1ce-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [device](../resources/device.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-135">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c1ce-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="8c1ce-136">Examples</span></span>

### <a name="example-1-get-a-list-of-devices"></a><span data-ttu-id="8c1ce-137">Пример 1. Получить список устройств</span><span class="sxs-lookup"><span data-stu-id="8c1ce-137">Example 1: Get a list of devices</span></span>

#### <a name="request"></a><span data-ttu-id="8c1ce-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c1ce-138">Request</span></span>

<span data-ttu-id="8c1ce-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8c1ce-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c1ce-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices
```
# <a name="c"></a>[<span data-ttu-id="8c1ce-141">C#</span><span class="sxs-lookup"><span data-stu-id="8c1ce-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c1ce-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c1ce-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c1ce-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c1ce-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c1ce-144">Java</span><span class="sxs-lookup"><span data-stu-id="8c1ce-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8c1ce-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c1ce-145">Response</span></span>

<span data-ttu-id="8c1ce-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-146">Here is an example of the response.</span></span>
> <span data-ttu-id="8c1ce-147">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-147">Note: The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-devices"></a><span data-ttu-id="8c1ce-148">Пример 2. Получить только количество устройств</span><span class="sxs-lookup"><span data-stu-id="8c1ce-148">Example 2: Get only a count of devices</span></span>

#### <a name="request"></a><span data-ttu-id="8c1ce-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c1ce-149">Request</span></span>

<span data-ttu-id="8c1ce-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-150">The following is an example of the request.</span></span> <span data-ttu-id="8c1ce-151">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual`, так как в запросе присутствует `$count`.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-151">This request requires the **ConsistencyLevel** header set to `eventual` because `$count` is in the request.</span></span> <span data-ttu-id="8c1ce-152">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="8c1ce-152">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="8c1ce-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c1ce-153">Response</span></span>

<span data-ttu-id="8c1ce-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-154">The following is an example of the response.</span></span>

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

<span data-ttu-id="8c1ce-155">294</span><span class="sxs-lookup"><span data-stu-id="8c1ce-155">294</span></span>

### <a name="example-3-use-filter-and-top-to-get-one-device-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="8c1ce-156">Пример 3. Использование $filter и $top для получения одного устройства с именем отображения, которое начинается с "a", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="8c1ce-156">Example 3: Use $filter and $top to get one device with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="8c1ce-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c1ce-157">Request</span></span>

<span data-ttu-id="8c1ce-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-158">The following is an example of the request.</span></span> <span data-ttu-id="8c1ce-159">Для этого запроса требуется заголовок **ConsistencyLevel** с присвоенным значением `eventual` и строка запроса `$count=true`, так как запрос содержит параметры запроса `$orderBy` и `$filter`.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-159">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters.</span></span> <span data-ttu-id="8c1ce-160">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="8c1ce-160">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="8c1ce-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c1ce-161">Response</span></span>

<span data-ttu-id="8c1ce-162">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-162">The following is an example of the response.</span></span>
><span data-ttu-id="8c1ce-163">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-163">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-use-search-to-get-devices-with-display-names-that-contain-the-letters-android-including-a-count-of-returned-objects"></a><span data-ttu-id="8c1ce-164">Пример 4. Использование $search для получения устройств с именами отображения, которые содержат буквы "Android", включая количество возвращенных объектов</span><span class="sxs-lookup"><span data-stu-id="8c1ce-164">Example 4: Use $search to get devices with display names that contain the letters 'Android' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="8c1ce-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c1ce-165">Request</span></span>

<span data-ttu-id="8c1ce-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-166">The following is an example of the request.</span></span> <span data-ttu-id="8c1ce-167">Этот запрос требует заглавного **загона ConsistencyLevel,** так как строка запроса `eventual` находится в `$search` `$count=true` запросе.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-167">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` and the `$count=true` query string is in the request.</span></span> <span data-ttu-id="8c1ce-168">Дополнительные сведения об использовании **ConsistencyLevel** и `$count` см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="8c1ce-168">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>


<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$search="displayName:Android"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="8c1ce-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c1ce-169">Response</span></span>

<span data-ttu-id="8c1ce-170">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-170">The following is an example of the response.</span></span>
><span data-ttu-id="8c1ce-171">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8c1ce-171">**Note:** The response object shown here might be shortened for readability.</span></span>

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


