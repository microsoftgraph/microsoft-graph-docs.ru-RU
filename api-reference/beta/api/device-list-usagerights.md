---
title: Список использования устройствRights
description: Извлечение списка объектов useRights для устройства.
author: jeeshnair
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 1edaa5f049a80744999c4259f8755f0be3d9aaf4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437128"
---
# <a name="list-device-usagerights"></a><span data-ttu-id="872fe-103">Список использования устройствRights</span><span class="sxs-lookup"><span data-stu-id="872fe-103">List device usageRights</span></span>
<span data-ttu-id="872fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="872fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="872fe-105">Извлечение списка [объектов useRight](../resources/usageright.md) для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="872fe-105">Retrieve a list of [usageRight](../resources/usageright.md) objects for a given device.</span></span>

## <a name="permissions"></a><span data-ttu-id="872fe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="872fe-106">Permissions</span></span>
<span data-ttu-id="872fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="872fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="872fe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="872fe-109">Permission type</span></span>|<span data-ttu-id="872fe-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="872fe-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="872fe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="872fe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="872fe-112">Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="872fe-112">Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="872fe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="872fe-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="872fe-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="872fe-114">Not supported.</span></span>|
|<span data-ttu-id="872fe-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="872fe-115">Application</span></span>|<span data-ttu-id="872fe-116">Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="872fe-116">Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="872fe-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="872fe-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /devices/{objectId}/usageRights
```

## <a name="optional-query-parameters"></a><span data-ttu-id="872fe-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="872fe-118">Optional query parameters</span></span>
<span data-ttu-id="872fe-119">Этот API поддерживает параметр $filter [OData.](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="872fe-119">This API supports the $filter [OData query parameter](/graph/query-parameters).</span></span> <span data-ttu-id="872fe-120">Поддерживаются следующие шаблоны $filter:</span><span class="sxs-lookup"><span data-stu-id="872fe-120">The following patterns of $filter are supported:</span></span>

- <span data-ttu-id="872fe-121">$filter = значение состояния eq</span><span class="sxs-lookup"><span data-stu-id="872fe-121">$filter = state eq 'value'</span></span>
- <span data-ttu-id="872fe-122">$filter = serviceIdentifier eq 'value'</span><span class="sxs-lookup"><span data-stu-id="872fe-122">$filter = serviceIdentifier eq 'value'</span></span>
- <span data-ttu-id="872fe-123">$filter = состояние eq 'value' и serviceIdentifier eq 'value'</span><span class="sxs-lookup"><span data-stu-id="872fe-123">$filter = state eq 'value' and serviceIdentifier eq 'value'</span></span>
- <span data-ttu-id="872fe-124">$filter = состояние в ('value1', 'value2')</span><span class="sxs-lookup"><span data-stu-id="872fe-124">$filter = state in ('value1', 'value2')</span></span>
- <span data-ttu-id="872fe-125">$filter = serviceIdentifier в ('value1', 'value2')</span><span class="sxs-lookup"><span data-stu-id="872fe-125">$filter = serviceIdentifier in ('value1', 'value2')</span></span>
- <span data-ttu-id="872fe-126">$filter = состояние в ('value1', 'value2') и serviceIdentifier в ('value1', 'value2')</span><span class="sxs-lookup"><span data-stu-id="872fe-126">$filter = state in ('value1', 'value2') and serviceIdentifier in ('value1', 'value2')</span></span>

## <a name="request-headers"></a><span data-ttu-id="872fe-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="872fe-127">Request headers</span></span>
|<span data-ttu-id="872fe-128">Имя</span><span class="sxs-lookup"><span data-stu-id="872fe-128">Name</span></span>|<span data-ttu-id="872fe-129">Описание</span><span class="sxs-lookup"><span data-stu-id="872fe-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="872fe-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="872fe-130">Authorization</span></span>|<span data-ttu-id="872fe-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="872fe-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="872fe-133">odata.maxpagesize</span><span class="sxs-lookup"><span data-stu-id="872fe-133">odata.maxpagesize</span></span>|<span data-ttu-id="872fe-134">Установите переоценку размера страницы максимального результата.</span><span class="sxs-lookup"><span data-stu-id="872fe-134">Set the max result page size pereference.</span></span> <span data-ttu-id="872fe-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="872fe-135">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="872fe-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="872fe-136">Request body</span></span>
<span data-ttu-id="872fe-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="872fe-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="872fe-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="872fe-138">Response</span></span>
<span data-ttu-id="872fe-139">В случае успешного использования этот метод возвращает код отклика и коллекцию `200 OK` [объектов useRight](../resources/usageright.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="872fe-139">If successful, this method returns a `200 OK` response code and a collection of [usageRight](../resources/usageright.md) objects in the response body.</span></span>

<span data-ttu-id="872fe-140">Кроме того, если в ответе больше страниц, возвращается @odata.nextLink.</span><span class="sxs-lookup"><span data-stu-id="872fe-140">Additionally, if there are more pages in the response an @odata.nextLink is returned.</span></span>

## <a name="examples"></a><span data-ttu-id="872fe-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="872fe-141">Examples</span></span>

### <a name="example-1-get-all-usage-rights-for-a-device"></a><span data-ttu-id="872fe-142">Пример 1. Получить все права использования для устройства</span><span class="sxs-lookup"><span data-stu-id="872fe-142">Example 1: Get all usage rights for a device</span></span>
 
#### <a name="request"></a><span data-ttu-id="872fe-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="872fe-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="872fe-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="872fe-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usageright"
}
-->
``` http
GET https://graph.microsoft.com/beta/devices/{objectId}/usageRights
```
# <a name="c"></a>[<span data-ttu-id="872fe-145">C#</span><span class="sxs-lookup"><span data-stu-id="872fe-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usageright-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="872fe-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="872fe-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usageright-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="872fe-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="872fe-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usageright-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="872fe-148">Java</span><span class="sxs-lookup"><span data-stu-id="872fe-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usageright-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="872fe-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="872fe-149">Response</span></span>
><span data-ttu-id="872fe-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="872fe-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-usage-rights-for-a-device-with-specific-service-identifiers-and-states"></a><span data-ttu-id="872fe-151">Пример 2. Получить права использования для устройства с определенными идентификаторами и состояниями службы</span><span class="sxs-lookup"><span data-stu-id="872fe-151">Example 2: Get usage rights for a device with specific service identifiers and states</span></span>

#### <a name="request"></a><span data-ttu-id="872fe-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="872fe-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="872fe-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="872fe-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usageright"
}
-->
``` http
GET https://graph.microsoft.com/beta/devices/{objectId}/usageRights?$filter=state in ('active', 'suspended') and serviceIdentifier in ('ABCD')
```
# <a name="c"></a>[<span data-ttu-id="872fe-154">C#</span><span class="sxs-lookup"><span data-stu-id="872fe-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usageright-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="872fe-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="872fe-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usageright-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="872fe-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="872fe-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usageright-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="872fe-157">Java</span><span class="sxs-lookup"><span data-stu-id="872fe-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usageright-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="872fe-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="872fe-158">Response</span></span>
><span data-ttu-id="872fe-159">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="872fe-159">**Note:** The response object shown here might be shortened for readability.</span></span>
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
