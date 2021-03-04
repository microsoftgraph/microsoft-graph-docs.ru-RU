---
title: Перечисление заданий
description: Извлечение списка объектов privilegedRoleAssignment, связанных с ролью. Каждый объект privilegedRoleAssignment представляет назначение роли пользователю.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 298742424152f7e483d709b33a6668e61cd866c3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441335"
---
# <a name="list-assignments"></a><span data-ttu-id="111ea-104">Перечисление заданий</span><span class="sxs-lookup"><span data-stu-id="111ea-104">List assignments</span></span>

<span data-ttu-id="111ea-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="111ea-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="111ea-106">Извлечение списка [объектов privilegedRoleAssignment,](../resources/privilegedroleassignment.md) связанных с ролью.</span><span class="sxs-lookup"><span data-stu-id="111ea-106">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects that are associated with the role.</span></span> <span data-ttu-id="111ea-107">Каждое [привилегированное назначениеRoleAssignment](../resources/privilegedroleassignment.md) представляет собой назначение роли пользователю.</span><span class="sxs-lookup"><span data-stu-id="111ea-107">Each [privilegedRoleAssignment](../resources/privilegedroleassignment.md) represents a role assignment to a user.</span></span>
## <a name="permissions"></a><span data-ttu-id="111ea-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="111ea-108">Permissions</span></span>
<span data-ttu-id="111ea-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="111ea-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="111ea-111">У запросителя должна быть одна из следующих ролей: _администратор_ привилегированных _ролей,_ глобальный _администратор,_ администратор безопасности или _читатель безопасности._</span><span class="sxs-lookup"><span data-stu-id="111ea-111">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="111ea-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="111ea-112">Permission type</span></span>      | <span data-ttu-id="111ea-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="111ea-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="111ea-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="111ea-114">Delegated (work or school account)</span></span> | <span data-ttu-id="111ea-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="111ea-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="111ea-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="111ea-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="111ea-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="111ea-117">Not supported.</span></span>    |
|<span data-ttu-id="111ea-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="111ea-118">Application</span></span> | <span data-ttu-id="111ea-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="111ea-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="111ea-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="111ea-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/assignments
```

<span data-ttu-id="111ea-121">Обратите ``{id}`` внимание, что это целевой id роли.</span><span class="sxs-lookup"><span data-stu-id="111ea-121">Note that ``{id}`` is the target role id.</span></span>
## <a name="optional-query-parameters"></a><span data-ttu-id="111ea-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="111ea-122">Optional query parameters</span></span>
<span data-ttu-id="111ea-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="111ea-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="111ea-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="111ea-124">Request headers</span></span>
| <span data-ttu-id="111ea-125">Имя</span><span class="sxs-lookup"><span data-stu-id="111ea-125">Name</span></span>      |<span data-ttu-id="111ea-126">Описание</span><span class="sxs-lookup"><span data-stu-id="111ea-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="111ea-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="111ea-127">Authorization</span></span>  | <span data-ttu-id="111ea-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="111ea-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="111ea-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="111ea-130">Request body</span></span>
<span data-ttu-id="111ea-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="111ea-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="111ea-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="111ea-132">Response</span></span>

<span data-ttu-id="111ea-133">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [privilegedRoleAssignment](../resources/privilegedroleassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="111ea-133">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="111ea-134">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="111ea-134">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="111ea-135">В противном случае код запретного статуса HTTP 403 будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="111ea-135">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="111ea-136">Пример</span><span class="sxs-lookup"><span data-stu-id="111ea-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="111ea-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="111ea-137">Request</span></span>
<span data-ttu-id="111ea-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="111ea-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="111ea-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="111ea-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/assignments
```
# <a name="c"></a>[<span data-ttu-id="111ea-140">C#</span><span class="sxs-lookup"><span data-stu-id="111ea-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-assignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="111ea-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="111ea-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-assignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="111ea-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="111ea-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-assignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="111ea-143">Java</span><span class="sxs-lookup"><span data-stu-id="111ea-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-assignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="111ea-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="111ea-144">Response</span></span>
<span data-ttu-id="111ea-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="111ea-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
