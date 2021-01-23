---
title: Список user usageRights
description: Получить список объектов usageRights для пользователя.
author: jeeshnair
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8896dc2ceff5109061eac01d56af8ceabb032dbd
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944365"
---
# <a name="list-user-usagerights"></a><span data-ttu-id="c2897-103">Список user usageRights</span><span class="sxs-lookup"><span data-stu-id="c2897-103">List user usageRights</span></span>
<span data-ttu-id="c2897-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2897-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2897-105">Получить список объектов [usageRight](../resources/usageright.md) для заданного пользователя.</span><span class="sxs-lookup"><span data-stu-id="c2897-105">Retrieve a list of [usageRight](../resources/usageright.md) objects for a given user.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2897-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2897-106">Permissions</span></span>
<span data-ttu-id="c2897-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2897-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2897-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2897-109">Permission type</span></span>|<span data-ttu-id="c2897-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2897-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2897-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2897-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c2897-112">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2897-112">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="c2897-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2897-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2897-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2897-114">Not supported.</span></span>|
|<span data-ttu-id="c2897-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2897-115">Application</span></span>|<span data-ttu-id="c2897-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2897-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2897-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2897-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{userId}/usageRights
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c2897-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c2897-118">Optional query parameters</span></span>
<span data-ttu-id="c2897-119">Этот API поддерживает параметр $filter [OData.](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="c2897-119">This API supports the $filter [OData query parameter](/graph/query-parameters).</span></span> <span data-ttu-id="c2897-120">Поддерживаются следующие шаблоны $filter:</span><span class="sxs-lookup"><span data-stu-id="c2897-120">The following patterns of $filter are supported:</span></span>

- <span data-ttu-id="c2897-121">$filter = state eq 'value'</span><span class="sxs-lookup"><span data-stu-id="c2897-121">$filter = state eq 'value'</span></span>
- <span data-ttu-id="c2897-122">$filter = serviceIdentifier eq 'value'</span><span class="sxs-lookup"><span data-stu-id="c2897-122">$filter = serviceIdentifier eq 'value'</span></span>
- <span data-ttu-id="c2897-123">$filter = state eq 'value' and serviceIdentifier eq 'value'</span><span class="sxs-lookup"><span data-stu-id="c2897-123">$filter = state eq 'value' and serviceIdentifier eq 'value'</span></span>
- <span data-ttu-id="c2897-124">$filter = state in ('value1', 'value2')</span><span class="sxs-lookup"><span data-stu-id="c2897-124">$filter = state in ('value1', 'value2')</span></span>
- <span data-ttu-id="c2897-125">$filter = serviceIdentifier в ('value1', 'value2')</span><span class="sxs-lookup"><span data-stu-id="c2897-125">$filter = serviceIdentifier in ('value1', 'value2')</span></span>
- <span data-ttu-id="c2897-126">$filter = state in ('value1', 'value2') and serviceIdentifier in ('value1', 'value2')</span><span class="sxs-lookup"><span data-stu-id="c2897-126">$filter = state in ('value1', 'value2') and serviceIdentifier in ('value1', 'value2')</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2897-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2897-127">Request headers</span></span>
|<span data-ttu-id="c2897-128">Имя</span><span class="sxs-lookup"><span data-stu-id="c2897-128">Name</span></span>|<span data-ttu-id="c2897-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c2897-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c2897-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2897-130">Authorization</span></span>|<span data-ttu-id="c2897-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2897-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c2897-133">odata.maxpagesize</span><span class="sxs-lookup"><span data-stu-id="c2897-133">odata.maxpagesize</span></span>|<span data-ttu-id="c2897-134">Установите максимальный размер страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="c2897-134">Set the max result page size pereference.</span></span> <span data-ttu-id="c2897-135">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c2897-135">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2897-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2897-136">Request body</span></span>
<span data-ttu-id="c2897-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2897-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2897-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2897-138">Response</span></span>
<span data-ttu-id="c2897-139">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [usageRight](../resources/usageright.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2897-139">If successful, this method returns a `200 OK` response code and a collection of [usageRight](../resources/usageright.md) objects in the response body.</span></span>

<span data-ttu-id="c2897-140">Кроме того, если в отклике больше страниц, возвращается @odata.nextLink.</span><span class="sxs-lookup"><span data-stu-id="c2897-140">Additionally, if there are more pages in the response an @odata.nextLink is returned.</span></span>

## <a name="examples"></a><span data-ttu-id="c2897-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="c2897-141">Examples</span></span>

### <a name="example-1-get-all-usage-rights-for-a-user"></a><span data-ttu-id="c2897-142">Пример 1. Получите все права на использование для пользователя</span><span class="sxs-lookup"><span data-stu-id="c2897-142">Example 1: Get all usage rights for a user</span></span>

#### <a name="request"></a><span data-ttu-id="c2897-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2897-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_usageright"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{userId}/usageRights
```

#### <a name="response"></a><span data-ttu-id="c2897-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2897-144">Response</span></span>
><span data-ttu-id="c2897-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c2897-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64952b80-51fd-4378-9ba5-589a840afb80')/usageRights",
  "@odata.nextLink": "https://graph.microsoft.com/beta/users/64952b80-51fd-4378-9ba5-589a840afb80/usageRights?$skiptoken=W4diD29cGKX1bX",
  "value": [
    {
      "id": "c2e034cb-3cbc-41be-a496-bfcd031e4cfc",
      "catalogId": "CFQ7TTC0KCRG:0001",
      "serviceIdentifier": "mscrm.f6d23ec7-255c-4bd8-8c99-dc041d5cb8b3.517f7ddd-df45-4f1c-83ec-a081a047f546",
      "state": "active"
    }
  ]
}
```

### <a name="example-2-get-usage-rights-for-a-user-with-specific-service-identifiers-and-states"></a><span data-ttu-id="c2897-146">Пример 2. Получите права на использование для пользователя с определенными идентификаторами и состояниями службы</span><span class="sxs-lookup"><span data-stu-id="c2897-146">Example 2: Get usage rights for a user with specific service identifiers and states</span></span>

#### <a name="request"></a><span data-ttu-id="c2897-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2897-147">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_usageright"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{userId}/usageRights?$filter=state in ('active', 'suspended') and serviceIdentifier in ('ABCD')
```

#### <a name="response"></a><span data-ttu-id="c2897-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2897-148">Response</span></span>
><span data-ttu-id="c2897-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c2897-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64952b80-51fd-4378-9ba5-589a840afb80')/usageRights",
  "value": [
    {
      "id": "505261eb-b4ee-421c-8206-05529ae2c150",
      "catalogId": "CFQ7TTC0KCRG:0001",
      "serviceIdentifier": "ABCD",
      "state": "active"
    }
  ]
}
```