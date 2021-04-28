---
title: Список объектов appRoleAssignment, предоставленных субъект-службе
description: Получение списка назначенных ролей приложения, предоставленных субъект-службе.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 9a9cfd5330d21fe8e8199c9a7fec58c8bb470e7d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049431"
---
# <a name="list-approleassignments-granted-for-a-service-principal"></a><span data-ttu-id="72194-103">Список объектов appRoleAssignment, предоставленных субъект-службе</span><span class="sxs-lookup"><span data-stu-id="72194-103">List appRoleAssignments granted for a service principal</span></span>

<span data-ttu-id="72194-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72194-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="72194-105">Получение списка [appRoleAssignment](../resources/approleassignment.md), предоставленного пользователям, группам или субъект-службам клиента для заданной субъект-службы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="72194-105">Retrieve a list of [appRoleAssignment](../resources/approleassignment.md) that users, groups, or client service principals have been granted for the given resource service principal.</span></span>

<span data-ttu-id="72194-106">Например, если ресурс субъект-службы является субъект-службой API Microsoft Graph, все субъект-службы, которым были предоставлены разрешения только для приложений на Microsoft Graph будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="72194-106">For example, if the resource service principal is the service principal for the Microsoft Graph API, this will return all service principals that have been granted any app-only permissions to Microsoft Graph.</span></span>

<span data-ttu-id="72194-107">Если ресурс субъект-службы является приложением, имеющим роли приложений, предоставленные пользователям и группам, все назначенные им роли для приложения будут возвращены.</span><span class="sxs-lookup"><span data-stu-id="72194-107">If the resource service principal is an application that has app roles granted to users and groups, this will return all the users and groups assigned app roles for this application.</span></span>

## <a name="permissions"></a><span data-ttu-id="72194-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72194-108">Permissions</span></span>

<span data-ttu-id="72194-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72194-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72194-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72194-111">Permission type</span></span>      | <span data-ttu-id="72194-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72194-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72194-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72194-113">Delegated (work or school account)</span></span> | <span data-ttu-id="72194-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="72194-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="72194-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72194-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72194-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72194-116">Not supported.</span></span>    |
|<span data-ttu-id="72194-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72194-117">Application</span></span> | <span data-ttu-id="72194-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72194-118">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="72194-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72194-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignedTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72194-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="72194-120">Optional query parameters</span></span>

<span data-ttu-id="72194-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="72194-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72194-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72194-122">Request headers</span></span>

| <span data-ttu-id="72194-123">Имя</span><span class="sxs-lookup"><span data-stu-id="72194-123">Name</span></span>           | <span data-ttu-id="72194-124">Описание</span><span class="sxs-lookup"><span data-stu-id="72194-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="72194-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72194-125">Authorization</span></span>  | <span data-ttu-id="72194-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72194-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="72194-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72194-128">Request body</span></span>

<span data-ttu-id="72194-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72194-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72194-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="72194-130">Response</span></span>

<span data-ttu-id="72194-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [appRoleAssignment](../resources/approleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="72194-131">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72194-132">Пример</span><span class="sxs-lookup"><span data-stu-id="72194-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="72194-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="72194-133">Request</span></span>

<span data-ttu-id="72194-134">В приведенном примере показано, как запросить извлечение назначений ролей приложения, предоставленных для заданного ресурса субъект-службы.</span><span class="sxs-lookup"><span data-stu-id="72194-134">The following is an example of the request to retrieve the app roles assignments that have been granted for a given resource service principal.</span></span>


# <a name="http"></a>[<span data-ttu-id="72194-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="72194-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_approleassignedto"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/8e881353-1735-45af-af21-ee1344582a4d/appRoleAssignedTo
```
# <a name="c"></a>[<span data-ttu-id="72194-136">C#</span><span class="sxs-lookup"><span data-stu-id="72194-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-get-approleassignedto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72194-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72194-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-get-approleassignedto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72194-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72194-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-get-approleassignedto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72194-139">Java</span><span class="sxs-lookup"><span data-stu-id="72194-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-get-approleassignedto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="72194-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="72194-140">Response</span></span>

<span data-ttu-id="72194-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="72194-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="72194-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="72194-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#servicePrincipals('8e881353-1735-45af-af21-ee1344582a4d')/appRoleAssignedTo",
  "value": [
    {
      "id": "41W1zT6z1U-kJxf62svfp1HFE8pMZhxDun-ThPczmJE",
      "deletedDateTime": null,
      "appRoleId": "00000000-0000-0000-0000-000000000000",
      "createdDateTime": "2021-02-02T04:22:45.9480566Z",
      "principalDisplayName": "MOD Administrator",
      "principalId": "cdb555e3-b33e-4fd5-a427-17fadacbdfa7",
      "principalType": "User",
      "resourceDisplayName": "dxprovisioning-graphapi-client",
      "resourceId": "8e881353-1735-45af-af21-ee1344582a4d"
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

