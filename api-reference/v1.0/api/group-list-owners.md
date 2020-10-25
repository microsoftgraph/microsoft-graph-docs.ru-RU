---
title: Список владельцев
description: 'Получение списка владельцев группы. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект группы. '
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f5190563b412fd5ae99c62a955981913acda1a0f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690254"
---
# <a name="list-owners"></a><span data-ttu-id="416ba-104">Список владельцев</span><span class="sxs-lookup"><span data-stu-id="416ba-104">List owners</span></span>

<span data-ttu-id="416ba-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="416ba-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="416ba-106">Получение списка владельцев группы.</span><span class="sxs-lookup"><span data-stu-id="416ba-106">Retrieve a list of the group's owners.</span></span> <span data-ttu-id="416ba-107">Владельцы — это группа пользователей или субъектов-служб, которым разрешено изменять этот групповой объект.</span><span class="sxs-lookup"><span data-stu-id="416ba-107">The owners are a set of users or service principals who are allowed to modify the group object.</span></span> <span data-ttu-id="416ba-108">В настоящий момент в Microsoft Graph недоступны владельцы для групп, созданных в Exchange или синхронизированных из локальной среды.</span><span class="sxs-lookup"><span data-stu-id="416ba-108">Owners are currently not available in Microsoft Graph for groups that were created in Exchange or groups that are synchronized from an on-premises environment.</span></span>

><span data-ttu-id="416ba-109">**Примечание.** В настоящее время субъекты-службы не указаны как владельцы группы благодаря поэтапному развертыванию субъектов-служб в конечной точке Microsoft Graph версии 1.0.</span><span class="sxs-lookup"><span data-stu-id="416ba-109">**Note:** Currently, service principals are not listed as group owners due to the staged rollout of service principals to the Microsoft Graph v1.0 endpoint.</span></span>

## <a name="permissions"></a><span data-ttu-id="416ba-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="416ba-110">Permissions</span></span>
<span data-ttu-id="416ba-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="416ba-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="416ba-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="416ba-113">Permission type</span></span>      | <span data-ttu-id="416ba-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="416ba-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="416ba-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="416ba-115">Delegated (work or school account)</span></span> | <span data-ttu-id="416ba-116">Group.Read.All и User.ReadBasic.All, Group.Read.All и User.Read.All, Group.Read.All и User.ReadWrite.All, Group.Read.All и User.Read.All и Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="416ba-116">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span>   |
|<span data-ttu-id="416ba-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="416ba-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="416ba-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="416ba-118">Not supported.</span></span>    |
|<span data-ttu-id="416ba-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="416ba-119">Application</span></span> | <span data-ttu-id="416ba-120">Group.Read.All и User.Read.All, Group.Read.All и User.ReadWrite.All, Group.Read.All и User.Read.All и Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="416ba-120">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="416ba-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="416ba-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="416ba-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="416ba-122">Optional query parameters</span></span>
<span data-ttu-id="416ba-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="416ba-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="416ba-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="416ba-124">Request headers</span></span>
| <span data-ttu-id="416ba-125">Имя</span><span class="sxs-lookup"><span data-stu-id="416ba-125">Name</span></span>       | <span data-ttu-id="416ba-126">Тип</span><span class="sxs-lookup"><span data-stu-id="416ba-126">Type</span></span> | <span data-ttu-id="416ba-127">Описание</span><span class="sxs-lookup"><span data-stu-id="416ba-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="416ba-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="416ba-128">Authorization</span></span>  | <span data-ttu-id="416ba-129">string</span><span class="sxs-lookup"><span data-stu-id="416ba-129">string</span></span>  | <span data-ttu-id="416ba-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="416ba-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="416ba-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="416ba-132">Request body</span></span>
<span data-ttu-id="416ba-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="416ba-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="416ba-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="416ba-134">Response</span></span>
<span data-ttu-id="416ba-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="416ba-135">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="416ba-136">Пример</span><span class="sxs-lookup"><span data-stu-id="416ba-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="416ba-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="416ba-137">Request</span></span>
<span data-ttu-id="416ba-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="416ba-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="416ba-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="416ba-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="416ba-140">C#</span><span class="sxs-lookup"><span data-stu-id="416ba-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="416ba-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="416ba-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="416ba-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="416ba-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="416ba-143">Java</span><span class="sxs-lookup"><span data-stu-id="416ba-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="416ba-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="416ba-144">Response</span></span>
<span data-ttu-id="416ba-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="416ba-145">The following is an example of the response.</span></span>
><span data-ttu-id="416ba-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="416ba-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.user"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

