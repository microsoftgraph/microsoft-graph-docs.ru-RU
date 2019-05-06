---
title: Перечисление заданий
description: Получение списка объектов Привилежедролеассигнмент, связанных с ролью. Каждый объект privilegedRoleAssignment представляет назначение роли пользователю.
localization_priority: Normal
ms.openlocfilehash: 9c35830d14808b062a13b28778991085ee3d2cf5
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33595594"
---
# <a name="list-assignments"></a><span data-ttu-id="37192-104">Перечисление заданий</span><span class="sxs-lookup"><span data-stu-id="37192-104">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37192-105">Получение списка объектов [привилежедролеассигнмент](../resources/privilegedroleassignment.md) , связанных с ролью.</span><span class="sxs-lookup"><span data-stu-id="37192-105">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects that are associated with the role.</span></span> <span data-ttu-id="37192-106">Каждый [привилежедролеассигнмент](../resources/privilegedroleassignment.md) представляет назначение роли пользователю.</span><span class="sxs-lookup"><span data-stu-id="37192-106">Each [privilegedRoleAssignment](../resources/privilegedroleassignment.md) represents a role assignment to a user.</span></span>
## <a name="permissions"></a><span data-ttu-id="37192-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="37192-107">Permissions</span></span>
<span data-ttu-id="37192-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37192-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="37192-110">Запрашивающая сторона должна иметь одну из следующих ролей: привилегированный _Администратор ролей_, _глобальный администратор_, _администратор безопасности_или _средство чтения безопасности_.</span><span class="sxs-lookup"><span data-stu-id="37192-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="37192-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37192-111">Permission type</span></span>      | <span data-ttu-id="37192-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37192-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37192-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37192-113">Delegated (work or school account)</span></span> | <span data-ttu-id="37192-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="37192-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="37192-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37192-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37192-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37192-116">Not supported.</span></span>    |
|<span data-ttu-id="37192-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37192-117">Application</span></span> | <span data-ttu-id="37192-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37192-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="37192-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37192-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/assignments
```

<span data-ttu-id="37192-120">Обратите ``<id>`` внимание, что это идентификатор целевой роли.</span><span class="sxs-lookup"><span data-stu-id="37192-120">Note that ``<id>`` is the target role id.</span></span>
## <a name="optional-query-parameters"></a><span data-ttu-id="37192-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="37192-121">Optional query parameters</span></span>
<span data-ttu-id="37192-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="37192-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37192-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37192-123">Request headers</span></span>
| <span data-ttu-id="37192-124">Имя</span><span class="sxs-lookup"><span data-stu-id="37192-124">Name</span></span>      |<span data-ttu-id="37192-125">Описание</span><span class="sxs-lookup"><span data-stu-id="37192-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="37192-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37192-126">Authorization</span></span>  | <span data-ttu-id="37192-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37192-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37192-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37192-129">Request body</span></span>
<span data-ttu-id="37192-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="37192-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37192-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="37192-131">Response</span></span>

<span data-ttu-id="37192-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="37192-132">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="37192-133">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="37192-133">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="37192-134">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="37192-134">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="37192-135">Пример</span><span class="sxs-lookup"><span data-stu-id="37192-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37192-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="37192-136">Request</span></span>
<span data-ttu-id="37192-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37192-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/assignments
```
##### <a name="response"></a><span data-ttu-id="37192-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="37192-138">Response</span></span>
<span data-ttu-id="37192-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37192-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="37192-142">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="37192-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="37192-143">Языках</span><span class="sxs-lookup"><span data-stu-id="37192-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_assignments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="37192-144">Язык</span><span class="sxs-lookup"><span data-stu-id="37192-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_assignments-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/privilegedrole-list-assignments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedrole-list-assignments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
