---
title: Список Аппролеассигнментс, назначенных субъекту службы
description: Получение списка назначений ролей приложений, назначенных субъекту службы.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: a30c80bd2dff43db3a505f593c0b30780565eef1
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291239"
---
# <a name="list-approleassignments-granted-for-a-service-principal"></a><span data-ttu-id="f6528-103">Список Аппролеассигнментс, назначенных субъекту службы</span><span class="sxs-lookup"><span data-stu-id="f6528-103">List appRoleAssignments granted for a service principal</span></span>

<span data-ttu-id="f6528-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6528-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6528-105">Получение списка [аппролеассигнмент](../resources/approleassignment.md) , которым были предоставлены пользователи, группы или субъекты службы клиента для данного субъекта службы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f6528-105">Retrieve a list of [appRoleAssignment](../resources/approleassignment.md) that users, groups, or client service principals have been granted for the given resource service principal.</span></span>

<span data-ttu-id="f6528-106">Например, если участник службы ресурсов является субъектом-службой для API Microsoft Graph, будут возвращены все субъекты-службы, которым были предоставлены разрешения только для приложения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f6528-106">For example, if the resource service principal is the service principal for the Microsoft Graph API, this will return all service principals that have been granted any app-only permissions to Microsoft Graph.</span></span>

<span data-ttu-id="f6528-107">Если участником службы ресурсов является приложение, которому назначены роли приложений для пользователей и групп, будут возвращены все пользователи и группы, которым назначены роли приложений для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="f6528-107">If the resource service principal is an application that has app roles granted to users and groups, this will return all the users and groups assigned app roles for this application.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6528-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6528-108">Permissions</span></span>

<span data-ttu-id="f6528-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6528-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6528-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6528-111">Permission type</span></span>      | <span data-ttu-id="f6528-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6528-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6528-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6528-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f6528-114">Directory. Read. ALL, Аппролеассигнмент. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="f6528-114">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="f6528-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6528-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6528-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6528-116">Not supported.</span></span>    |
|<span data-ttu-id="f6528-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6528-117">Application</span></span> | <span data-ttu-id="f6528-118">Directory. Read. ALL, Аппролеассигнмент. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f6528-118">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6528-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6528-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignedTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6528-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f6528-120">Optional query parameters</span></span>

<span data-ttu-id="f6528-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f6528-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6528-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6528-122">Request headers</span></span>

| <span data-ttu-id="f6528-123">Имя</span><span class="sxs-lookup"><span data-stu-id="f6528-123">Name</span></span>           | <span data-ttu-id="f6528-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f6528-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="f6528-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6528-125">Authorization</span></span>  | <span data-ttu-id="f6528-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6528-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f6528-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f6528-128">Request body</span></span>

<span data-ttu-id="f6528-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6528-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6528-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6528-130">Response</span></span>

<span data-ttu-id="f6528-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [аппролеассигнмент](../resources/approleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6528-131">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6528-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f6528-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6528-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6528-133">Request</span></span>

<span data-ttu-id="f6528-134">Ниже приведен пример запроса на получение назначений ролей приложения, предоставленных для данного субъекта-службы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f6528-134">The following is an example of the request to retrieve the app roles assignments that have been granted for a given resource service principal.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_approleassignedto"
}-->

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignedTo
```

### <a name="response"></a><span data-ttu-id="f6528-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6528-135">Response</span></span>

<span data-ttu-id="f6528-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f6528-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="f6528-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6528-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
