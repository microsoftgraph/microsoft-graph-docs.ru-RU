---
title: Список владельцев
description: Получение списка владельцев группы.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 29352a52e6e50c788bd1457f3038c6389356303f
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271976"
---
# <a name="list-owners"></a><span data-ttu-id="d4565-103">Список владельцев</span><span class="sxs-lookup"><span data-stu-id="d4565-103">List owners</span></span>

<span data-ttu-id="d4565-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4565-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4565-105">Получение списка владельцев группы.</span><span class="sxs-lookup"><span data-stu-id="d4565-105">Retrieve a list of the group's owners.</span></span> <span data-ttu-id="d4565-106">Владельцы — это набор пользователей, которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="d4565-106">The owners are a set of users who are allowed to modify the group object.</span></span> <span data-ttu-id="d4565-107">Владельцы в настоящее время недоступны в Microsoft Graph для групп, созданных в Exchange или синхронизированных из локальной среды.</span><span class="sxs-lookup"><span data-stu-id="d4565-107">Owners are currently not available in Microsoft Graph for groups that were created in Exchange or groups that are synchronized from an on-premises environment.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d4565-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4565-108">Permissions</span></span>
<span data-ttu-id="d4565-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4565-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4565-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4565-111">Permission type</span></span>      | <span data-ttu-id="d4565-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4565-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4565-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4565-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d4565-114">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d4565-114">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="d4565-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4565-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4565-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4565-116">Not supported.</span></span>    |
|<span data-ttu-id="d4565-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4565-117">Application</span></span> | <span data-ttu-id="d4565-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d4565-118">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>  |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="d4565-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4565-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4565-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d4565-120">Optional query parameters</span></span>
<span data-ttu-id="d4565-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d4565-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4565-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4565-122">Request headers</span></span>
| <span data-ttu-id="d4565-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d4565-123">Name</span></span>       | <span data-ttu-id="d4565-124">Тип</span><span class="sxs-lookup"><span data-stu-id="d4565-124">Type</span></span> | <span data-ttu-id="d4565-125">Описание</span><span class="sxs-lookup"><span data-stu-id="d4565-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d4565-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4565-126">Authorization</span></span>  | <span data-ttu-id="d4565-127">string</span><span class="sxs-lookup"><span data-stu-id="d4565-127">string</span></span>  | <span data-ttu-id="d4565-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4565-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4565-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d4565-130">Request body</span></span>
<span data-ttu-id="d4565-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d4565-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4565-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4565-132">Response</span></span>
<span data-ttu-id="d4565-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4565-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4565-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d4565-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d4565-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4565-135">Request</span></span>
<span data-ttu-id="d4565-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4565-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d4565-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4565-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="d4565-138">C#</span><span class="sxs-lookup"><span data-stu-id="d4565-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4565-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4565-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4565-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4565-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d4565-141">Java</span><span class="sxs-lookup"><span data-stu-id="d4565-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d4565-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4565-142">Response</span></span>
<span data-ttu-id="d4565-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d4565-143">The following is an example of the response.</span></span>
><span data-ttu-id="d4565-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4565-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


