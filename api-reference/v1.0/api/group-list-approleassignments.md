---
title: Список объектов appRoleAssignment, предоставленных для группы
description: Получение списка appRoleAssignment, предоставленного группе.
localization_priority: Priority
doc_type: apiPageType
ms.prod: groups
author: psignoret
ms.openlocfilehash: 90c8b025b739722b927e9b2f0ac63d6bca51294e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052350"
---
# <a name="list-approleassignments-granted-to-a-group"></a><span data-ttu-id="7719d-103">Список объектов appRoleAssignment, предоставленных для группы</span><span class="sxs-lookup"><span data-stu-id="7719d-103">List appRoleAssignments granted to a group</span></span>

<span data-ttu-id="7719d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7719d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7719d-105">Получение списка [appRoleAssignment](../resources/approleassignment.md), предоставленного группе.</span><span class="sxs-lookup"><span data-stu-id="7719d-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that have been granted to a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="7719d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7719d-106">Permissions</span></span>

<span data-ttu-id="7719d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7719d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7719d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7719d-109">Permission type</span></span>      | <span data-ttu-id="7719d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7719d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7719d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7719d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7719d-112">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7719d-112">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="7719d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7719d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7719d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7719d-114">Not supported.</span></span>    |
|<span data-ttu-id="7719d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7719d-115">Application</span></span> | <span data-ttu-id="7719d-116">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7719d-116">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7719d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7719d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7719d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7719d-118">Optional query parameters</span></span>

<span data-ttu-id="7719d-119">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7719d-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7719d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7719d-120">Request headers</span></span>

| <span data-ttu-id="7719d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="7719d-121">Name</span></span>           | <span data-ttu-id="7719d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7719d-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="7719d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7719d-123">Authorization</span></span>  | <span data-ttu-id="7719d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7719d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7719d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7719d-126">Request body</span></span>

<span data-ttu-id="7719d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7719d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7719d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7719d-128">Response</span></span>

<span data-ttu-id="7719d-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [appRoleAssignment](../resources/approleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7719d-129">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7719d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7719d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7719d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7719d-131">Request</span></span>

<span data-ttu-id="7719d-132">В приведенном примере показано, как запросить извлечение ролей приложения, назначенных группе.</span><span class="sxs-lookup"><span data-stu-id="7719d-132">The following example shows a request to retrieve the app roles that have been assigned to a group.</span></span>


# <a name="http"></a>[<span data-ttu-id="7719d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7719d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_approleassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/7679d9a4-2323-44cd-b5c2-673ec88d8b12/appRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="7719d-134">C#</span><span class="sxs-lookup"><span data-stu-id="7719d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7719d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7719d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7719d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7719d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7719d-137">Java</span><span class="sxs-lookup"><span data-stu-id="7719d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-approleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7719d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7719d-138">Response</span></span>

<span data-ttu-id="7719d-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7719d-139">The following is an example of the response.</span></span>

> <span data-ttu-id="7719d-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7719d-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('7679d9a4-2323-44cd-b5c2-673ec88d8b12')/appRoleAssignments",
  "value": [
    {
      "id": "pNl5diMjzUS1wmc-yI2LEkGgWqFFrFdLhG2Ly2CysL4",
      "deletedDateTime": null,
      "appRoleId": "00000000-0000-0000-0000-000000000000",
      "createdDateTime": "2021-02-19T17:55:08.3369542Z",
      "principalDisplayName": "Young techmakers",
      "principalId": "7679d9a4-2323-44cd-b5c2-673ec88d8b12",
      "principalType": "Group",
      "resourceDisplayName": "Yammer",
      "resourceId": "076e8b57-bac8-49d7-9396-e3449b685055"
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

