---
title: Список транзитивных групп memberOf
description: Получение групп, членом которых является группа.  Эта операция является транзитивным и также включает все группы, в которых вложены эти группы. В отличие от извлечения групп Office 365 пользователя, возвращаются все типы групп, а не только группы Office 365.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6e887543fe02f79d20da83dd8bd3593aa147ca22
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125157"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="26e40-105">Список транзитивных групп memberOf</span><span class="sxs-lookup"><span data-stu-id="26e40-105">List group transitive memberOf</span></span>

<span data-ttu-id="26e40-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26e40-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="26e40-107">Получение групп, членом которых является группа.</span><span class="sxs-lookup"><span data-stu-id="26e40-107">Get groups that the group is a member of.</span></span>  <span data-ttu-id="26e40-108">Эта операция является транзитивным и также включает все группы, в которых вложены эти группы.</span><span class="sxs-lookup"><span data-stu-id="26e40-108">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="26e40-109">В отличие от извлечения групп Office 365 пользователя, возвращаются все типы групп, а не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="26e40-109">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="26e40-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26e40-110">Permissions</span></span>

<span data-ttu-id="26e40-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26e40-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26e40-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26e40-113">Permission type</span></span>      | <span data-ttu-id="26e40-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26e40-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26e40-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26e40-115">Delegated (work or school account)</span></span> | <span data-ttu-id="26e40-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="26e40-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="26e40-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26e40-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26e40-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26e40-118">Not supported.</span></span>    |
|<span data-ttu-id="26e40-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26e40-119">Application</span></span> | <span data-ttu-id="26e40-120">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26e40-120">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="26e40-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26e40-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="26e40-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="26e40-122">Optional query parameters</span></span>
<span data-ttu-id="26e40-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="26e40-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="26e40-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26e40-124">Request headers</span></span>
| <span data-ttu-id="26e40-125">Имя</span><span class="sxs-lookup"><span data-stu-id="26e40-125">Name</span></span>       | <span data-ttu-id="26e40-126">Тип</span><span class="sxs-lookup"><span data-stu-id="26e40-126">Type</span></span> | <span data-ttu-id="26e40-127">Описание</span><span class="sxs-lookup"><span data-stu-id="26e40-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="26e40-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="26e40-128">Authorization</span></span>  | <span data-ttu-id="26e40-129">string</span><span class="sxs-lookup"><span data-stu-id="26e40-129">string</span></span>  | <span data-ttu-id="26e40-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26e40-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26e40-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26e40-132">Request body</span></span>
<span data-ttu-id="26e40-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26e40-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26e40-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="26e40-134">Response</span></span>
<span data-ttu-id="26e40-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="26e40-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26e40-136">Пример</span><span class="sxs-lookup"><span data-stu-id="26e40-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="26e40-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="26e40-137">Request</span></span>
<span data-ttu-id="26e40-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26e40-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26e40-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="26e40-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="26e40-140">C#</span><span class="sxs-lookup"><span data-stu-id="26e40-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26e40-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26e40-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26e40-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26e40-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26e40-143">Java</span><span class="sxs-lookup"><span data-stu-id="26e40-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="26e40-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="26e40-144">Response</span></span>

<span data-ttu-id="26e40-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="26e40-145">The following is an example of the response.</span></span>
><span data-ttu-id="26e40-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26e40-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
