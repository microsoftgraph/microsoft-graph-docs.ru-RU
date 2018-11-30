---
title: Список назначений
description: Получение списка объектов privilegedRoleAssignment, связанных с ролью. Каждый privilegedRoleAssignment представляет назначения ролей для пользователя.
ms.openlocfilehash: 52cc720381baa6b7c82fe3b5c88d469081da3b81
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079533"
---
# <a name="list-assignments"></a><span data-ttu-id="49477-104">Список назначений</span><span class="sxs-lookup"><span data-stu-id="49477-104">List assignments</span></span>

> <span data-ttu-id="49477-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="49477-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49477-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49477-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="49477-107">Получение списка объектов [privilegedRoleAssignment](../resources/privilegedroleassignment.md) , связанных с ролью.</span><span class="sxs-lookup"><span data-stu-id="49477-107">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects that are associated with the role.</span></span> <span data-ttu-id="49477-108">Каждый [privilegedRoleAssignment](../resources/privilegedroleassignment.md) представляет назначения ролей для пользователя.</span><span class="sxs-lookup"><span data-stu-id="49477-108">Each [privilegedRoleAssignment](../resources/privilegedroleassignment.md) represents a role assignment to a user.</span></span>
## <a name="permissions"></a><span data-ttu-id="49477-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49477-109">Permissions</span></span>
<span data-ttu-id="49477-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49477-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="49477-112">Запросившая сторона должен иметь одно из следующих ролей: _Привилегированной роль администратора_, _Глобального администратора_, _Администратора безопасности_или _Безопасности чтения_.</span><span class="sxs-lookup"><span data-stu-id="49477-112">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="49477-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49477-113">Permission type</span></span>      | <span data-ttu-id="49477-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49477-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49477-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49477-115">Delegated (work or school account)</span></span> | <span data-ttu-id="49477-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="49477-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="49477-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49477-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49477-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49477-118">Not supported.</span></span>    |
|<span data-ttu-id="49477-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49477-119">Application</span></span> | <span data-ttu-id="49477-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49477-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49477-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49477-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/assignments
```

<span data-ttu-id="49477-122">Обратите внимание, что ``<id>`` — это идентификатор целевого роли.</span><span class="sxs-lookup"><span data-stu-id="49477-122">Note that ``<id>`` is the target role id.</span></span>
## <a name="optional-query-parameters"></a><span data-ttu-id="49477-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="49477-123">Optional query parameters</span></span>
<span data-ttu-id="49477-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="49477-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49477-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49477-125">Request headers</span></span>
| <span data-ttu-id="49477-126">Имя</span><span class="sxs-lookup"><span data-stu-id="49477-126">Name</span></span>      |<span data-ttu-id="49477-127">Описание</span><span class="sxs-lookup"><span data-stu-id="49477-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="49477-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49477-128">Authorization</span></span>  | <span data-ttu-id="49477-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49477-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49477-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49477-131">Request body</span></span>
<span data-ttu-id="49477-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49477-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49477-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="49477-133">Response</span></span>

<span data-ttu-id="49477-134">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [privilegedRoleAssignment](../resources/privilegedroleassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="49477-134">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="49477-135">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="49477-135">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="49477-136">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="49477-136">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="49477-137">Пример</span><span class="sxs-lookup"><span data-stu-id="49477-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49477-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="49477-138">Request</span></span>
<span data-ttu-id="49477-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49477-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/assignments
```
##### <a name="response"></a><span data-ttu-id="49477-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="49477-140">Response</span></span>
<span data-ttu-id="49477-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="49477-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
