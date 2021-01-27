---
title: Список устройств usageRights
description: Получить список объектов usageRights для устройства.
author: jeeshnair
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 73a67ecd46085c7c4369e68db5f72655cbaf395a
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013627"
---
# <a name="list-device-usagerights"></a><span data-ttu-id="06d33-103">Список устройств usageRights</span><span class="sxs-lookup"><span data-stu-id="06d33-103">List device usageRights</span></span>
<span data-ttu-id="06d33-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06d33-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06d33-105">Получить список объектов [usageRight](../resources/usageright.md) для заданного устройства.</span><span class="sxs-lookup"><span data-stu-id="06d33-105">Retrieve a list of [usageRight](../resources/usageright.md) objects for a given device.</span></span>

## <a name="permissions"></a><span data-ttu-id="06d33-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06d33-106">Permissions</span></span>
<span data-ttu-id="06d33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06d33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06d33-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06d33-109">Permission type</span></span>|<span data-ttu-id="06d33-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06d33-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06d33-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06d33-111">Delegated (work or school account)</span></span>|<span data-ttu-id="06d33-112">Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06d33-112">Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="06d33-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06d33-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06d33-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06d33-114">Not supported.</span></span>|
|<span data-ttu-id="06d33-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06d33-115">Application</span></span>|<span data-ttu-id="06d33-116">Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06d33-116">Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06d33-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06d33-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /devices/{objectId}/usageRights
```

## <a name="optional-query-parameters"></a><span data-ttu-id="06d33-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="06d33-118">Optional query parameters</span></span>
<span data-ttu-id="06d33-119">Этот API поддерживает параметр $filter [OData.](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="06d33-119">This API supports the $filter [OData query parameter](/graph/query-parameters).</span></span> <span data-ttu-id="06d33-120">Поддерживаются следующие шаблоны $filter:</span><span class="sxs-lookup"><span data-stu-id="06d33-120">The following patterns of $filter are supported:</span></span>

- <span data-ttu-id="06d33-121">$filter = state eq 'value'</span><span class="sxs-lookup"><span data-stu-id="06d33-121">$filter = state eq 'value'</span></span>
- <span data-ttu-id="06d33-122">$filter = serviceIdentifier eq 'value'</span><span class="sxs-lookup"><span data-stu-id="06d33-122">$filter = serviceIdentifier eq 'value'</span></span>
- <span data-ttu-id="06d33-123">$filter = state eq 'value' and serviceIdentifier eq 'value'</span><span class="sxs-lookup"><span data-stu-id="06d33-123">$filter = state eq 'value' and serviceIdentifier eq 'value'</span></span>
- <span data-ttu-id="06d33-124">$filter = state in ('value1', 'value2')</span><span class="sxs-lookup"><span data-stu-id="06d33-124">$filter = state in ('value1', 'value2')</span></span>
- <span data-ttu-id="06d33-125">$filter = serviceIdentifier в ('value1', 'value2')</span><span class="sxs-lookup"><span data-stu-id="06d33-125">$filter = serviceIdentifier in ('value1', 'value2')</span></span>
- <span data-ttu-id="06d33-126">$filter = state in ('value1', 'value2') and serviceIdentifier in ('value1', 'value2')</span><span class="sxs-lookup"><span data-stu-id="06d33-126">$filter = state in ('value1', 'value2') and serviceIdentifier in ('value1', 'value2')</span></span>

## <a name="request-headers"></a><span data-ttu-id="06d33-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06d33-127">Request headers</span></span>
|<span data-ttu-id="06d33-128">Имя</span><span class="sxs-lookup"><span data-stu-id="06d33-128">Name</span></span>|<span data-ttu-id="06d33-129">Описание</span><span class="sxs-lookup"><span data-stu-id="06d33-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="06d33-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06d33-130">Authorization</span></span>|<span data-ttu-id="06d33-p103">Bearer {token}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06d33-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="06d33-133">odata.maxpagesize</span><span class="sxs-lookup"><span data-stu-id="06d33-133">odata.maxpagesize</span></span>|<span data-ttu-id="06d33-134">Установите максимальный размер страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="06d33-134">Set the max result page size pereference.</span></span> <span data-ttu-id="06d33-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="06d33-135">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="06d33-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="06d33-136">Request body</span></span>
<span data-ttu-id="06d33-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06d33-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06d33-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="06d33-138">Response</span></span>
<span data-ttu-id="06d33-139">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [usageRight](../resources/usageright.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="06d33-139">If successful, this method returns a `200 OK` response code and a collection of [usageRight](../resources/usageright.md) objects in the response body.</span></span>

<span data-ttu-id="06d33-140">Кроме того, если в отклике больше страниц, возвращается @odata.nextLink.</span><span class="sxs-lookup"><span data-stu-id="06d33-140">Additionally, if there are more pages in the response an @odata.nextLink is returned.</span></span>

## <a name="examples"></a><span data-ttu-id="06d33-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="06d33-141">Examples</span></span>

### <a name="example-1-get-all-usage-rights-for-a-device"></a><span data-ttu-id="06d33-142">Пример 1. Получите все права на использование устройства</span><span class="sxs-lookup"><span data-stu-id="06d33-142">Example 1: Get all usage rights for a device</span></span>
 
#### <a name="request"></a><span data-ttu-id="06d33-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="06d33-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="06d33-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="06d33-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usageright"
}
-->
``` http
GET https://graph.microsoft.com/beta/devices/{objectId}/usageRights
```
# <a name="c"></a>[<span data-ttu-id="06d33-145">C#</span><span class="sxs-lookup"><span data-stu-id="06d33-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usageright-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06d33-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06d33-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usageright-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06d33-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06d33-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usageright-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06d33-148">Java</span><span class="sxs-lookup"><span data-stu-id="06d33-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usageright-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="06d33-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="06d33-149">Response</span></span>
><span data-ttu-id="06d33-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="06d33-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.usageRight)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#devices('fead5c35-ebc5-47c4-a909-c43b4faf2160')/usageRights",
  "@odata.nextLink": "https://graph.microsoft.com/beta/devices/fead5c35-ebc5-47c4-a909-c43b4faf2160/usageRights?$skiptoken=W4diD29cGKX1bX",
  "value": [
    {
      "id": "99f828b9-09f2-445d-a758-b6727316dbe1",
      "catalogId": "CFQ7TTC0KCRG:0001",
      "serviceIdentifier": "mscrm.f6d23ec7-255c-4bd8-8c99-dc041d5cb8b3.517f7ddd-df45-4f1c-83ec-a081a047f546",
      "state": "active"
    }
  ]
}
```

### <a name="example-2-get-usage-rights-for-a-device-with-specific-service-identifiers-and-states"></a><span data-ttu-id="06d33-151">Пример 2. Получите права на использование для устройства с определенными идентификаторами и состояниями службы</span><span class="sxs-lookup"><span data-stu-id="06d33-151">Example 2: Get usage rights for a device with specific service identifiers and states</span></span>

#### <a name="request"></a><span data-ttu-id="06d33-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="06d33-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="06d33-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="06d33-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usageright"
}
-->
``` http
GET https://graph.microsoft.com/beta/devices/{objectId}/usageRights?$filter=state in ('active', 'suspended') and serviceIdentifier in ('ABCD')
```
# <a name="c"></a>[<span data-ttu-id="06d33-154">C#</span><span class="sxs-lookup"><span data-stu-id="06d33-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usageright-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06d33-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06d33-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usageright-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06d33-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06d33-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usageright-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06d33-157">Java</span><span class="sxs-lookup"><span data-stu-id="06d33-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usageright-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="06d33-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="06d33-158">Response</span></span>
><span data-ttu-id="06d33-159">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="06d33-159">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.usageRight)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#devices('fead5c35-ebc5-47c4-a909-c43b4faf2160')/usageRights",
  "value": [
    {
      "id": "9905e6b1-9040-4926-b028-fdb748c359d6",
      "catalogId": "CFQ7TTC0KCRG:0001",
      "serviceIdentifier": "ABCD",
      "state": "active"
    }
  ]
}
```
