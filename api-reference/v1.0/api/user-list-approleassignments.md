---
title: Список Аппролеассигнментс, назначенных пользователю
description: Получение списка назначений ролей приложений, назначенных пользователю.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: daae2378b844d057fb6103f3392f40ff84688ac9
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290959"
---
# <a name="list-approleassignments-granted-to-a-user"></a><span data-ttu-id="308c6-103">Список Аппролеассигнментс, назначенных пользователю</span><span class="sxs-lookup"><span data-stu-id="308c6-103">List appRoleAssignments granted to a user</span></span>

<span data-ttu-id="308c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="308c6-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="308c6-105">Получение списка [аппролеассигнмент](../resources/approleassignment.md) , предоставленных пользователю.</span><span class="sxs-lookup"><span data-stu-id="308c6-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that a user has been granted.</span></span> <span data-ttu-id="308c6-106">Эта операция также возвращает роли приложения, назначенные группам, непосредственно участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="308c6-106">This operation also returns app roles assigned to groups that the user is a direct member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="308c6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="308c6-107">Permissions</span></span>

<span data-ttu-id="308c6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="308c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="308c6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="308c6-110">Permission type</span></span>      | <span data-ttu-id="308c6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="308c6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="308c6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="308c6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="308c6-113">Directory. Read. ALL, Аппролеассигнмент. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="308c6-113">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="308c6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="308c6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="308c6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="308c6-115">Not supported.</span></span>    |
|<span data-ttu-id="308c6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="308c6-116">Application</span></span> | <span data-ttu-id="308c6-117">Directory. Read. ALL, Аппролеассигнмент. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="308c6-117">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="308c6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="308c6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="308c6-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="308c6-119">Optional query parameters</span></span>

<span data-ttu-id="308c6-120">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="308c6-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="308c6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="308c6-121">Request headers</span></span>

| <span data-ttu-id="308c6-122">Имя</span><span class="sxs-lookup"><span data-stu-id="308c6-122">Name</span></span>           | <span data-ttu-id="308c6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="308c6-123">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="308c6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="308c6-124">Authorization</span></span>  | <span data-ttu-id="308c6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="308c6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="308c6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="308c6-127">Request body</span></span>

<span data-ttu-id="308c6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="308c6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="308c6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="308c6-129">Response</span></span>

<span data-ttu-id="308c6-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [аппролеассигнмент](../resources/approleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="308c6-130">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="308c6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="308c6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="308c6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="308c6-132">Request</span></span>

<span data-ttu-id="308c6-133">Ниже приведен пример запроса на получение ролей приложения, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="308c6-133">Here is an example of the request to retrieve the app roles that have been assigned to a user.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_approleassignments"
}-->

```http
GET https://graph.microsoft.com/v1.0/users/{id}/appRoleAssignments
```

### <a name="response"></a><span data-ttu-id="308c6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="308c6-134">Response</span></span>

<span data-ttu-id="308c6-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="308c6-135">The following is an example of the response.</span></span> 

> <span data-ttu-id="308c6-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="308c6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 306

{
  "value": [
    {
      "creationTimestamp": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalDisplayName": "principalDisplayName-value",
      "principalId": "principalId-value",
      "principalType": "principalType-value",
      "resourceDisplayName": "resourceDisplayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
