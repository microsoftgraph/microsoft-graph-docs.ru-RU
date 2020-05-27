---
title: Список Аппролеассигнментс, назначенных группе
description: Получение списка Аппролеассигнментс, предоставленных группе.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 847eeffdc91ba69aaf53d893888554e7f5bcc02f
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383731"
---
# <a name="list-approleassignments-granted-to-a-group"></a><span data-ttu-id="4c32f-103">Список Аппролеассигнментс, назначенных группе</span><span class="sxs-lookup"><span data-stu-id="4c32f-103">List appRoleAssignments granted to a group</span></span>

<span data-ttu-id="4c32f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c32f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c32f-105">Получение списка [аппролеассигнмент](../resources/approleassignment.md) , предоставленных группе.</span><span class="sxs-lookup"><span data-stu-id="4c32f-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that have been granted to a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c32f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c32f-106">Permissions</span></span>

<span data-ttu-id="4c32f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c32f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c32f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c32f-109">Permission type</span></span>      | <span data-ttu-id="4c32f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c32f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c32f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c32f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4c32f-112">Directory. Read. ALL, Аппролеассигнмент. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="4c32f-112">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="4c32f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c32f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c32f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c32f-114">Not supported.</span></span>    |
|<span data-ttu-id="4c32f-115">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="4c32f-115">Application</span></span> | <span data-ttu-id="4c32f-116">Directory. Read. ALL, Аппролеассигнмент. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4c32f-116">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c32f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c32f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4c32f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4c32f-118">Optional query parameters</span></span>

<span data-ttu-id="4c32f-119">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4c32f-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c32f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c32f-120">Request headers</span></span>

| <span data-ttu-id="4c32f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4c32f-121">Name</span></span>           | <span data-ttu-id="4c32f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4c32f-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="4c32f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c32f-123">Authorization</span></span>  | <span data-ttu-id="4c32f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c32f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4c32f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c32f-126">Request body</span></span>

<span data-ttu-id="4c32f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c32f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c32f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c32f-128">Response</span></span>

<span data-ttu-id="4c32f-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [аппролеассигнмент](../resources/approleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c32f-129">If successful, this method returns a `200 OK` response code and collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c32f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4c32f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c32f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c32f-131">Request</span></span>

<span data-ttu-id="4c32f-132">Ниже приведен пример запроса на получение ролей приложений, назначенных группе.</span><span class="sxs-lookup"><span data-stu-id="4c32f-132">Here is an example of the request to retrieve the app roles which have been assigned to a group.</span></span>


# <a name="http"></a>[<span data-ttu-id="4c32f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c32f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_approleassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/appRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="4c32f-134">C#</span><span class="sxs-lookup"><span data-stu-id="4c32f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c32f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c32f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c32f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c32f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4c32f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c32f-137">Response</span></span>

<span data-ttu-id="4c32f-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4c32f-138">The following is an example of the response.</span></span>

> <span data-ttu-id="4c32f-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c32f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
