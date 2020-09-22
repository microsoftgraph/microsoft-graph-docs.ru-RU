---
title: Перечисление транзитивных групп устройств
description: Получение групп, участником которых является устройство.
author: spunukol
ms.prod: microsoft-identity-platform
localization_priority: Normal
doc_type: apiPageType
ms.openlocfilehash: 859cd2fa83a62f04d65f2553e2fd33f3c483e760
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078026"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="625a7-103">Перечисление транзитивных групп устройств</span><span class="sxs-lookup"><span data-stu-id="625a7-103">List device transitive groups</span></span>

<span data-ttu-id="625a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="625a7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="625a7-105">Получение групп, участником которых является устройство.</span><span class="sxs-lookup"><span data-stu-id="625a7-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="625a7-106">Этот запрос API является транзитивным, а также возвращает все группы, в которых устройство является вложенным членом.</span><span class="sxs-lookup"><span data-stu-id="625a7-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="625a7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="625a7-107">Permissions</span></span>

<span data-ttu-id="625a7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="625a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="625a7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="625a7-110">Permission type</span></span>      | <span data-ttu-id="625a7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="625a7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="625a7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="625a7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="625a7-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="625a7-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="625a7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="625a7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="625a7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="625a7-115">Not supported.</span></span>    |
|<span data-ttu-id="625a7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="625a7-116">Application</span></span> | <span data-ttu-id="625a7-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="625a7-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="625a7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="625a7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="625a7-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="625a7-119">Optional query parameters</span></span>

<span data-ttu-id="625a7-120">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="625a7-120">This method supports the [OData Query Parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="625a7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="625a7-121">Request headers</span></span>

| <span data-ttu-id="625a7-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="625a7-122">Header</span></span>       | <span data-ttu-id="625a7-123">Значение</span><span class="sxs-lookup"><span data-stu-id="625a7-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="625a7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="625a7-124">Authorization</span></span>  | <span data-ttu-id="625a7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="625a7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="625a7-127">Accept</span><span class="sxs-lookup"><span data-stu-id="625a7-127">Accept</span></span>  | <span data-ttu-id="625a7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="625a7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="625a7-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="625a7-129">Request body</span></span>

<span data-ttu-id="625a7-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="625a7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="625a7-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="625a7-131">Response</span></span>

<span data-ttu-id="625a7-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="625a7-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="625a7-133">Пример</span><span class="sxs-lookup"><span data-stu-id="625a7-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="625a7-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="625a7-134">Request</span></span>

<span data-ttu-id="625a7-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="625a7-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="625a7-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="625a7-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="625a7-137">C#</span><span class="sxs-lookup"><span data-stu-id="625a7-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="625a7-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="625a7-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="625a7-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="625a7-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="625a7-140">Java</span><span class="sxs-lookup"><span data-stu-id="625a7-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="625a7-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="625a7-141">Response</span></span>

<span data-ttu-id="625a7-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="625a7-142">Here is an example of the response.</span></span> 

><span data-ttu-id="625a7-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="625a7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List devices transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

