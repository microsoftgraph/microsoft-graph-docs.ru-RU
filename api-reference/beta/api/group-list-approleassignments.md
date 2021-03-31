---
title: Список объектов appRoleAssignment, предоставленных для группы
description: Получение списка appRoleAssignment, предоставленного группе.
localization_priority: Priority
doc_type: apiPageType
ms.prod: groups
author: psignoret
ms.openlocfilehash: 16cc5012db3bfd1fde2705974afa6fe23978b90e
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468886"
---
# <a name="list-approleassignments-granted-to-a-group"></a><span data-ttu-id="2798e-103">Список объектов appRoleAssignment, предоставленных для группы</span><span class="sxs-lookup"><span data-stu-id="2798e-103">List appRoleAssignments granted to a group</span></span>

<span data-ttu-id="2798e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2798e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2798e-105">Получение списка [appRoleAssignment](../resources/approleassignment.md), предоставленного группе.</span><span class="sxs-lookup"><span data-stu-id="2798e-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that have been granted to a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="2798e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2798e-106">Permissions</span></span>

<span data-ttu-id="2798e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2798e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2798e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2798e-109">Permission type</span></span>      | <span data-ttu-id="2798e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2798e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2798e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2798e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2798e-112">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2798e-112">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="2798e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2798e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2798e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2798e-114">Not supported.</span></span>    |
|<span data-ttu-id="2798e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2798e-115">Application</span></span> | <span data-ttu-id="2798e-116">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2798e-116">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2798e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2798e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2798e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2798e-118">Optional query parameters</span></span>

<span data-ttu-id="2798e-119">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2798e-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2798e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2798e-120">Request headers</span></span>

| <span data-ttu-id="2798e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2798e-121">Name</span></span>           | <span data-ttu-id="2798e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2798e-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="2798e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2798e-123">Authorization</span></span>  | <span data-ttu-id="2798e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2798e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2798e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2798e-126">Request body</span></span>

<span data-ttu-id="2798e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2798e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2798e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2798e-128">Response</span></span>

<span data-ttu-id="2798e-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [appRoleAssignment](../resources/approleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2798e-129">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2798e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2798e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2798e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2798e-131">Request</span></span>

<span data-ttu-id="2798e-132">В приведенном примере показано, как запросить извлечение ролей приложения, назначенных группе.</span><span class="sxs-lookup"><span data-stu-id="2798e-132">The following example shows a request to retrieve the app roles that have been assigned to a group.</span></span>


# <a name="http"></a>[<span data-ttu-id="2798e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2798e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_approleassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/7679d9a4-2323-44cd-b5c2-673ec88d8b12/appRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="2798e-134">C#</span><span class="sxs-lookup"><span data-stu-id="2798e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2798e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2798e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2798e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2798e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2798e-137">Java</span><span class="sxs-lookup"><span data-stu-id="2798e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-approleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2798e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2798e-138">Response</span></span>

<span data-ttu-id="2798e-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2798e-139">The following is an example of the response.</span></span>

> <span data-ttu-id="2798e-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2798e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('7679d9a4-2323-44cd-b5c2-673ec88d8b12')/appRoleAssignments",
  "value": [
    {
      "id": "pNl5diMjzUS1wmc-yI2LEkGgWqFFrFdLhG2Ly2CysL4",
      "deletedDateTime": null,
      "appRoleId": "00000000-0000-0000-0000-000000000000",
      "creationTimestamp": "2021-02-19T17:55:08.3369542Z",
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

