---
title: Перечисление заданий
description: Получение списка объектов Привилежедролеассигнмент, связанных с ролью. Каждый объект privilegedRoleAssignment представляет назначение роли пользователю.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 02a282546778e2de558f7f770426969a96441071
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315037"
---
# <a name="list-assignments"></a><span data-ttu-id="67b40-104">Перечисление заданий</span><span class="sxs-lookup"><span data-stu-id="67b40-104">List assignments</span></span>

<span data-ttu-id="67b40-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67b40-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67b40-106">Получение списка объектов [привилежедролеассигнмент](../resources/privilegedroleassignment.md) , связанных с ролью.</span><span class="sxs-lookup"><span data-stu-id="67b40-106">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects that are associated with the role.</span></span> <span data-ttu-id="67b40-107">Каждый [привилежедролеассигнмент](../resources/privilegedroleassignment.md) представляет назначение роли пользователю.</span><span class="sxs-lookup"><span data-stu-id="67b40-107">Each [privilegedRoleAssignment](../resources/privilegedroleassignment.md) represents a role assignment to a user.</span></span>
## <a name="permissions"></a><span data-ttu-id="67b40-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67b40-108">Permissions</span></span>
<span data-ttu-id="67b40-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67b40-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="67b40-111">Запрашивающая сторона должна иметь одну из следующих ролей: _привилегированный администратор ролей_, _глобальный администратор_, _администратор безопасности_или _средство чтения безопасности_.</span><span class="sxs-lookup"><span data-stu-id="67b40-111">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="67b40-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67b40-112">Permission type</span></span>      | <span data-ttu-id="67b40-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67b40-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67b40-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67b40-114">Delegated (work or school account)</span></span> | <span data-ttu-id="67b40-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="67b40-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="67b40-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67b40-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67b40-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67b40-117">Not supported.</span></span>    |
|<span data-ttu-id="67b40-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67b40-118">Application</span></span> | <span data-ttu-id="67b40-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67b40-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="67b40-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67b40-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/assignments
```

<span data-ttu-id="67b40-121">Обратите внимание, что ``{id}`` это идентификатор целевой роли.</span><span class="sxs-lookup"><span data-stu-id="67b40-121">Note that ``{id}`` is the target role id.</span></span>
## <a name="optional-query-parameters"></a><span data-ttu-id="67b40-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="67b40-122">Optional query parameters</span></span>
<span data-ttu-id="67b40-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="67b40-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="67b40-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67b40-124">Request headers</span></span>
| <span data-ttu-id="67b40-125">Имя</span><span class="sxs-lookup"><span data-stu-id="67b40-125">Name</span></span>      |<span data-ttu-id="67b40-126">Описание</span><span class="sxs-lookup"><span data-stu-id="67b40-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="67b40-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67b40-127">Authorization</span></span>  | <span data-ttu-id="67b40-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67b40-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67b40-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67b40-130">Request body</span></span>
<span data-ttu-id="67b40-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="67b40-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67b40-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="67b40-132">Response</span></span>

<span data-ttu-id="67b40-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="67b40-133">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="67b40-134">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="67b40-134">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="67b40-135">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="67b40-135">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="67b40-136">Пример</span><span class="sxs-lookup"><span data-stu-id="67b40-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67b40-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="67b40-137">Request</span></span>
<span data-ttu-id="67b40-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67b40-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="67b40-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="67b40-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/assignments
```
# <a name="c"></a>[<span data-ttu-id="67b40-140">C#</span><span class="sxs-lookup"><span data-stu-id="67b40-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-assignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67b40-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67b40-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-assignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67b40-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67b40-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-assignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="67b40-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="67b40-143">Response</span></span>
<span data-ttu-id="67b40-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67b40-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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