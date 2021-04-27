---
title: Получение privilegedRoleAssignment
description: Извлечение свойств и связей объекта privilegedRoleAssignment.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 8a2369d9745a9df0b689a589ab75c7a10d51147c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055234"
---
# <a name="get-privilegedroleassignment"></a><span data-ttu-id="151d6-103">Получение privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="151d6-103">Get privilegedRoleAssignment</span></span>

<span data-ttu-id="151d6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="151d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="151d6-105">Извлечение свойств и связей объекта privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="151d6-105">Retrieve the properties and relationships of privilegedRoleAssignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="151d6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="151d6-106">Permissions</span></span>
<span data-ttu-id="151d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="151d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="151d6-109">У запросителя должна быть одна из следующих ролей: _администратор_ привилегированных _ролей,_ глобальный _администратор,_ администратор безопасности или _читатель безопасности._</span><span class="sxs-lookup"><span data-stu-id="151d6-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="151d6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="151d6-110">Permission type</span></span>      | <span data-ttu-id="151d6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="151d6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="151d6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="151d6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="151d6-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="151d6-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="151d6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="151d6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="151d6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="151d6-115">Not supported.</span></span>    |
|<span data-ttu-id="151d6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="151d6-116">Application</span></span> | <span data-ttu-id="151d6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="151d6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="151d6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="151d6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="151d6-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="151d6-119">Optional query parameters</span></span>
<span data-ttu-id="151d6-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="151d6-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="151d6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="151d6-121">Request headers</span></span>
| <span data-ttu-id="151d6-122">Имя</span><span class="sxs-lookup"><span data-stu-id="151d6-122">Name</span></span>      |<span data-ttu-id="151d6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="151d6-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="151d6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="151d6-124">Authorization</span></span>  | <span data-ttu-id="151d6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="151d6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="151d6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="151d6-127">Request body</span></span>
<span data-ttu-id="151d6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="151d6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="151d6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="151d6-129">Response</span></span>

<span data-ttu-id="151d6-130">В случае успешного выполнения этот метод возвращает код ответа и объект `200 OK` [privilegedRoleAssignment](../resources/privilegedroleassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="151d6-130">If successful, this method returns a `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="151d6-131">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="151d6-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="151d6-132">В противном случае код запретного статуса HTTP 403 будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="151d6-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="151d6-133">Пример</span><span class="sxs-lookup"><span data-stu-id="151d6-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="151d6-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="151d6-134">Request</span></span>
<span data-ttu-id="151d6-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="151d6-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="151d6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="151d6-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="151d6-137">C#</span><span class="sxs-lookup"><span data-stu-id="151d6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="151d6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="151d6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="151d6-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="151d6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="151d6-140">Java</span><span class="sxs-lookup"><span data-stu-id="151d6-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="151d6-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="151d6-141">Response</span></span>
<span data-ttu-id="151d6-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="151d6-142">Here is an example of the response.</span></span> <span data-ttu-id="151d6-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="151d6-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
