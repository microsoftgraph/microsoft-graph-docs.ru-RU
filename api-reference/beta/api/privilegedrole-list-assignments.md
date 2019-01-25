---
title: Список назначений
description: Получение списка объектов privilegedRoleAssignment, связанных с ролью. Каждый privilegedRoleAssignment представляет назначения ролей для пользователя.
localization_priority: Normal
ms.openlocfilehash: f7dd2b94c5d3ac49a6a8c9183373801f76e27964
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508274"
---
# <a name="list-assignments"></a><span data-ttu-id="e1b3f-104">Список назначений</span><span class="sxs-lookup"><span data-stu-id="e1b3f-104">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1b3f-105">Получение списка объектов [privilegedRoleAssignment](../resources/privilegedroleassignment.md) , связанных с ролью.</span><span class="sxs-lookup"><span data-stu-id="e1b3f-105">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects that are associated with the role.</span></span> <span data-ttu-id="e1b3f-106">Каждый [privilegedRoleAssignment](../resources/privilegedroleassignment.md) представляет назначения ролей для пользователя.</span><span class="sxs-lookup"><span data-stu-id="e1b3f-106">Each [privilegedRoleAssignment](../resources/privilegedroleassignment.md) represents a role assignment to a user.</span></span>
## <a name="permissions"></a><span data-ttu-id="e1b3f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1b3f-107">Permissions</span></span>
<span data-ttu-id="e1b3f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1b3f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e1b3f-110">Запросившая сторона должен иметь одно из следующих ролей: _Привилегированной роль администратора_, _Глобального администратора_, _Администратора безопасности_или _Безопасности чтения_.</span><span class="sxs-lookup"><span data-stu-id="e1b3f-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="e1b3f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1b3f-111">Permission type</span></span>      | <span data-ttu-id="e1b3f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1b3f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1b3f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1b3f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e1b3f-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e1b3f-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e1b3f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1b3f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1b3f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1b3f-116">Not supported.</span></span>    |
|<span data-ttu-id="e1b3f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1b3f-117">Application</span></span> | <span data-ttu-id="e1b3f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1b3f-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1b3f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1b3f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/assignments
```

<span data-ttu-id="e1b3f-120">Обратите внимание, что ``<id>`` — это идентификатор целевого роли.</span><span class="sxs-lookup"><span data-stu-id="e1b3f-120">Note that ``<id>`` is the target role id.</span></span>
## <a name="optional-query-parameters"></a><span data-ttu-id="e1b3f-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e1b3f-121">Optional query parameters</span></span>
<span data-ttu-id="e1b3f-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e1b3f-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1b3f-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1b3f-123">Request headers</span></span>
| <span data-ttu-id="e1b3f-124">Имя</span><span class="sxs-lookup"><span data-stu-id="e1b3f-124">Name</span></span>      |<span data-ttu-id="e1b3f-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e1b3f-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e1b3f-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1b3f-126">Authorization</span></span>  | <span data-ttu-id="e1b3f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1b3f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1b3f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1b3f-129">Request body</span></span>
<span data-ttu-id="e1b3f-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e1b3f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1b3f-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1b3f-131">Response</span></span>

<span data-ttu-id="e1b3f-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [privilegedRoleAssignment](../resources/privilegedroleassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e1b3f-132">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="e1b3f-133">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="e1b3f-133">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="e1b3f-134">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="e1b3f-134">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="e1b3f-135">Пример</span><span class="sxs-lookup"><span data-stu-id="e1b3f-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1b3f-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1b3f-136">Request</span></span>
<span data-ttu-id="e1b3f-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1b3f-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/assignments
```
##### <a name="response"></a><span data-ttu-id="e1b3f-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1b3f-138">Response</span></span>
<span data-ttu-id="e1b3f-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e1b3f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
