---
title: Перечисление заданий
description: Получение списка объектов Привилежедролеассигнмент, связанных с ролью. Каждый объект privilegedRoleAssignment представляет назначение роли пользователю.
localization_priority: Normal
ms.openlocfilehash: f7dd2b94c5d3ac49a6a8c9183373801f76e27964
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546569"
---
# <a name="list-assignments"></a><span data-ttu-id="4da8b-104">Перечисление заданий</span><span class="sxs-lookup"><span data-stu-id="4da8b-104">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4da8b-105">Получение списка объектов [привилежедролеассигнмент](../resources/privilegedroleassignment.md) , связанных с ролью.</span><span class="sxs-lookup"><span data-stu-id="4da8b-105">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects that are associated with the role.</span></span> <span data-ttu-id="4da8b-106">Каждый [привилежедролеассигнмент](../resources/privilegedroleassignment.md) представляет назначение роли пользователю.</span><span class="sxs-lookup"><span data-stu-id="4da8b-106">Each [privilegedRoleAssignment](../resources/privilegedroleassignment.md) represents a role assignment to a user.</span></span>
## <a name="permissions"></a><span data-ttu-id="4da8b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4da8b-107">Permissions</span></span>
<span data-ttu-id="4da8b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4da8b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4da8b-110">Запрашивающая сторона должна иметь одну из следующих ролей: привилегированный _Администратор ролей_, _глобальный администратор_, _администратор безопасности_или _средство чтения безопасности_.</span><span class="sxs-lookup"><span data-stu-id="4da8b-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="4da8b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4da8b-111">Permission type</span></span>      | <span data-ttu-id="4da8b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4da8b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4da8b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4da8b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4da8b-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4da8b-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4da8b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4da8b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4da8b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4da8b-116">Not supported.</span></span>    |
|<span data-ttu-id="4da8b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4da8b-117">Application</span></span> | <span data-ttu-id="4da8b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4da8b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4da8b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4da8b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/assignments
```

<span data-ttu-id="4da8b-120">Обратите ``<id>`` внимание, что это идентификатор целевой роли.</span><span class="sxs-lookup"><span data-stu-id="4da8b-120">Note that ``<id>`` is the target role id.</span></span>
## <a name="optional-query-parameters"></a><span data-ttu-id="4da8b-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4da8b-121">Optional query parameters</span></span>
<span data-ttu-id="4da8b-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4da8b-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4da8b-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4da8b-123">Request headers</span></span>
| <span data-ttu-id="4da8b-124">Имя</span><span class="sxs-lookup"><span data-stu-id="4da8b-124">Name</span></span>      |<span data-ttu-id="4da8b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="4da8b-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4da8b-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4da8b-126">Authorization</span></span>  | <span data-ttu-id="4da8b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4da8b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4da8b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4da8b-129">Request body</span></span>
<span data-ttu-id="4da8b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4da8b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4da8b-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="4da8b-131">Response</span></span>

<span data-ttu-id="4da8b-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [привилежедролеассигнмент](../resources/privilegedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4da8b-132">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="4da8b-133">Обратите внимание, что клиент должен быть зарегистрирован в PIM.</span><span class="sxs-lookup"><span data-stu-id="4da8b-133">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="4da8b-134">В противном случае будет возвращен код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="4da8b-134">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="4da8b-135">Пример</span><span class="sxs-lookup"><span data-stu-id="4da8b-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4da8b-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="4da8b-136">Request</span></span>
<span data-ttu-id="4da8b-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4da8b-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/assignments
```
##### <a name="response"></a><span data-ttu-id="4da8b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4da8b-138">Response</span></span>
<span data-ttu-id="4da8b-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4da8b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/privilegedrole-list-assignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
