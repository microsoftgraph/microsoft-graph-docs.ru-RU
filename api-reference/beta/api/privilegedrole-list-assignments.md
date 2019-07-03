---
title: Перечисление заданий
description: Получение списка объектов Привилежедролеассигнмент, связанных с ролью. Каждый объект privilegedRoleAssignment представляет назначение роли пользователю.
localization_priority: Normal
ms.openlocfilehash: 6f5a41eda5e69a387c11ee0cd8fd2d8b17c98ccc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445032"
---
# <a name="list-assignments"></a><span data-ttu-id="a8c48-104">Перечисление заданий</span><span class="sxs-lookup"><span data-stu-id="a8c48-104">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8c48-105">Получение списка объектов [привилежедролеассигнмент](../resources/privilegedroleassignment.md) , связанных с ролью.</span><span class="sxs-lookup"><span data-stu-id="a8c48-105">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects that are associated with the role.</span></span> <span data-ttu-id="a8c48-106">Каждый [привилежедролеассигнмент](../resources/privilegedroleassignment.md) представляет назначение роли пользователю.</span><span class="sxs-lookup"><span data-stu-id="a8c48-106">Each [privilegedRoleAssignment](../resources/privilegedroleassignment.md) represents a role assignment to a user.</span></span>
## <a name="permissions"></a><span data-ttu-id="a8c48-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8c48-107">Permissions</span></span>
<span data-ttu-id="a8c48-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8c48-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a8c48-110">Запрашивающая сторона должна иметь одну из следующих ролей: привилегированный _Администратор ролей_, _глобальный администратор_, _администратор безопасности_или _средство чтения безопасности_.</span><span class="sxs-lookup"><span data-stu-id="a8c48-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="a8c48-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8c48-111">Permission type</span></span>      | <span data-ttu-id="a8c48-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8c48-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8c48-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8c48-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a8c48-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a8c48-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a8c48-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8c48-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8c48-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8c48-116">Not supported.</span></span>    |
|<span data-ttu-id="a8c48-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8c48-117">Application</span></span> | <span data-ttu-id="a8c48-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8c48-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8c48-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8c48-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/assignments
```

<span data-ttu-id="a8c48-120">Обратите ``<id>`` внимание, что это идентификатор целевой роли.</span><span class="sxs-lookup"><span data-stu-id="a8c48-120">Note that ``<id>`` is the target role id.</span></span>
## <a name="optional-query-parameters"></a><span data-ttu-id="a8c48-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a8c48-121">Optional query parameters</span></span>
<span data-ttu-id="a8c48-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a8c48-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8c48-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8c48-123">Request headers</span></span>
| <span data-ttu-id="a8c48-124">Имя</span><span class="sxs-lookup"><span data-stu-id="a8c48-124">Name</span></span>      |<span data-ttu-id="a8c48-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a8c48-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a8c48-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8c48-126">Authorization</span></span>  | <span data-ttu-id="a8c48-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8c48-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8c48-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a8c48-129">Request body</span></span>
<span data-ttu-id="a8c48-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a8c48-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8c48-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8c48-131">Response</span></span>

<span data-ttu-id="a8c48-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a8c48-132">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="a8c48-133">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="a8c48-133">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="a8c48-134">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="a8c48-134">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="a8c48-135">Пример</span><span class="sxs-lookup"><span data-stu-id="a8c48-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8c48-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8c48-136">Request</span></span>
<span data-ttu-id="a8c48-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8c48-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a8c48-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8c48-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/assignments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a8c48-139">C#</span><span class="sxs-lookup"><span data-stu-id="a8c48-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-assignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8c48-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="a8c48-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-assignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a8c48-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a8c48-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-assignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a8c48-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8c48-142">Response</span></span>
<span data-ttu-id="a8c48-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8c48-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
