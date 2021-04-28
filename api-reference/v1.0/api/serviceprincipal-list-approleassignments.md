---
title: Список объектов appRoleAssignment, предоставленных для субъект-службы
description: Получение списка назначений ролей приложений, предоставленных для субъект-службы.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 4b0d9e0ad43691b1e708bab1f07f57cb6186ea58
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038819"
---
# <a name="list-approleassignments-granted-to-a-service-principal"></a><span data-ttu-id="6fe8d-103">Список объектов appRoleAssignment, предоставленных для субъект-службы</span><span class="sxs-lookup"><span data-stu-id="6fe8d-103">List appRoleAssignments granted to a service principal</span></span>

<span data-ttu-id="6fe8d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fe8d-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="6fe8d-105">Получение списка [appRoleAssignment](../resources/approleassignment.md), предоставленного субъект-службе.</span><span class="sxs-lookup"><span data-stu-id="6fe8d-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that have been granted to a service principal.</span></span>

<span data-ttu-id="6fe8d-106">Роли приложений, назначаемые субъектам-службам, также называются [разрешениями приложений](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="6fe8d-106">App roles that are assigned to service principals are also known as [application permissions](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="6fe8d-107">Разрешения приложений можно предоставлять с помощью создания назначений ролей приложений, а также с помощью [интерфейса согласия](/azure/active-directory/develop/application-consent-experience).</span><span class="sxs-lookup"><span data-stu-id="6fe8d-107">Application permissions can be granted directly by creating app role assignments, or through a [consent experience](/azure/active-directory/develop/application-consent-experience).</span></span>

## <a name="permissions"></a><span data-ttu-id="6fe8d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6fe8d-108">Permissions</span></span>

<span data-ttu-id="6fe8d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fe8d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fe8d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6fe8d-111">Permission type</span></span>      | <span data-ttu-id="6fe8d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6fe8d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fe8d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6fe8d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6fe8d-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6fe8d-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="6fe8d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6fe8d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fe8d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fe8d-116">Not supported.</span></span>    |
|<span data-ttu-id="6fe8d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6fe8d-117">Application</span></span> | <span data-ttu-id="6fe8d-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fe8d-118">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fe8d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6fe8d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6fe8d-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6fe8d-120">Optional query parameters</span></span>

<span data-ttu-id="6fe8d-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="6fe8d-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6fe8d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6fe8d-122">Request headers</span></span>

| <span data-ttu-id="6fe8d-123">Имя</span><span class="sxs-lookup"><span data-stu-id="6fe8d-123">Name</span></span>           | <span data-ttu-id="6fe8d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6fe8d-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="6fe8d-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6fe8d-125">Authorization</span></span>  | <span data-ttu-id="6fe8d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6fe8d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6fe8d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6fe8d-128">Request body</span></span>

<span data-ttu-id="6fe8d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6fe8d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fe8d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fe8d-130">Response</span></span>

<span data-ttu-id="6fe8d-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [appRoleAssignment](../resources/approleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6fe8d-131">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fe8d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6fe8d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fe8d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6fe8d-133">Request</span></span>

<span data-ttu-id="6fe8d-134">В приведенном примере показано, как запросить извлечение ролей приложения, назначенных субъект-службе.</span><span class="sxs-lookup"><span data-stu-id="6fe8d-134">The following is an example of a request to retrieve the app roles that have been assigned to a service principal.</span></span>


# <a name="http"></a>[<span data-ttu-id="6fe8d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fe8d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_approleassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/8e881353-1735-45af-af21-ee1344582a4d/appRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="6fe8d-136">C#</span><span class="sxs-lookup"><span data-stu-id="6fe8d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6fe8d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fe8d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6fe8d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fe8d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6fe8d-139">Java</span><span class="sxs-lookup"><span data-stu-id="6fe8d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-get-approleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6fe8d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fe8d-140">Response</span></span>

<span data-ttu-id="6fe8d-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6fe8d-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="6fe8d-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6fe8d-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appRoleAssignments",
  "value": [
    {
      "id": "UxOIjjUXr0WvIe4TRFgqTY4z9Wu5KxpBtlEpoTGjw-A",
      "createdDateTime": "2021-02-02T04:22:45.4980259Z",
      "appRoleId": "e2a3a72e-5f79-4c64-b1b1-878b674786c9",
      "principalDisplayName": "dxprovisioning-graphapi-client",
      "principalId": "8e881353-1735-45af-af21-ee1344582a4d",
      "principalType": "ServicePrincipal",
      "resourceDisplayName": "Microsoft Graph",
      "resourceId": "fea94d6d-b5bf-44d2-a887-4f72a8d74f44"
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
