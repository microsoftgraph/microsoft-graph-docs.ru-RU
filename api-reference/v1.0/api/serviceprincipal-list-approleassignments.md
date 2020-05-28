---
title: Список Аппролеассигнментс, назначенных субъекту службы
description: Получение списка назначений ролей приложений, назначенных участнику службы.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 27b896a8dde36aea3993fb098c22219e13be6b29
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383987"
---
# <a name="list-approleassignments-granted-to-a-service-principal"></a><span data-ttu-id="e639a-103">Список Аппролеассигнментс, назначенных субъекту службы</span><span class="sxs-lookup"><span data-stu-id="e639a-103">List appRoleAssignments granted to a service principal</span></span>

<span data-ttu-id="e639a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e639a-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="e639a-105">Получение списка [аппролеассигнмент](../resources/approleassignment.md) , предоставленных участнику службы.</span><span class="sxs-lookup"><span data-stu-id="e639a-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that have been granted to a service principal.</span></span>

<span data-ttu-id="e639a-106">Роли приложений, назначенные субъектам служб, также называются [разрешениями приложений](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="e639a-106">App roles that are assigned to service principals are also known as [application permissions](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="e639a-107">Разрешения на доступ к приложениям можно предоставить непосредственно путем создания назначений ролей приложений или с помощью [согласия пользователя](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span><span class="sxs-lookup"><span data-stu-id="e639a-107">Application permissions can be granted directly by creating app role assignments, or through a [consent experience](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span></span>

## <a name="permissions"></a><span data-ttu-id="e639a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e639a-108">Permissions</span></span>

<span data-ttu-id="e639a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e639a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e639a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e639a-111">Permission type</span></span>      | <span data-ttu-id="e639a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e639a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e639a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e639a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e639a-114">Application. Read. ALL, Directory. Read. ALL, Application. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="e639a-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="e639a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e639a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e639a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e639a-116">Not supported.</span></span>    |
|<span data-ttu-id="e639a-117">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="e639a-117">Application</span></span> | <span data-ttu-id="e639a-118">Application. Read. ALL, Directory. Read. ALL, Application. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e639a-118">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e639a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e639a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e639a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e639a-120">Optional query parameters</span></span>

<span data-ttu-id="e639a-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e639a-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e639a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e639a-122">Request headers</span></span>

| <span data-ttu-id="e639a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e639a-123">Name</span></span>           | <span data-ttu-id="e639a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e639a-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="e639a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e639a-125">Authorization</span></span>  | <span data-ttu-id="e639a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e639a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e639a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e639a-128">Request body</span></span>

<span data-ttu-id="e639a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e639a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e639a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e639a-130">Response</span></span>

<span data-ttu-id="e639a-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [аппролеассигнмент](../resources/approleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e639a-131">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e639a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e639a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e639a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e639a-133">Request</span></span>

<span data-ttu-id="e639a-134">Ниже приведен пример запроса на получение ролей приложения, назначенных участнику службы.</span><span class="sxs-lookup"><span data-stu-id="e639a-134">The following is an example of a request to retrieve the app roles that have been assigned to a service principal.</span></span>


# <a name="http"></a>[<span data-ttu-id="e639a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e639a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_approleassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/appRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="e639a-136">C#</span><span class="sxs-lookup"><span data-stu-id="e639a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e639a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e639a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e639a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e639a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e639a-139">Java</span><span class="sxs-lookup"><span data-stu-id="e639a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-get-approleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e639a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e639a-140">Response</span></span>

<span data-ttu-id="e639a-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e639a-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="e639a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e639a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
