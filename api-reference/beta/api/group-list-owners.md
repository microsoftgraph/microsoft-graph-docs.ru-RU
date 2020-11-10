---
title: Список владельцев
description: Получение списка владельцев группы.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0f3e76c321cd6732a0a2a0c3944e1df02cba92fb
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953991"
---
# <a name="list-owners"></a><span data-ttu-id="55758-103">Список владельцев</span><span class="sxs-lookup"><span data-stu-id="55758-103">List owners</span></span>

<span data-ttu-id="55758-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55758-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55758-105">Получение списка владельцев группы.</span><span class="sxs-lookup"><span data-stu-id="55758-105">Retrieve a list of the group's owners.</span></span> <span data-ttu-id="55758-106">Владельцы — это набор пользователей, которым разрешено изменять объект Group.</span><span class="sxs-lookup"><span data-stu-id="55758-106">The owners are a set of users who are allowed to modify the group object.</span></span> <span data-ttu-id="55758-107">В настоящий момент в Microsoft Graph недоступны владельцы для групп, созданных в Exchange или синхронизированных из локальной среды.</span><span class="sxs-lookup"><span data-stu-id="55758-107">Owners are currently not available in Microsoft Graph for groups that were created in Exchange or groups that are synchronized from an on-premises environment.</span></span> 

## <a name="permissions"></a><span data-ttu-id="55758-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55758-108">Permissions</span></span>
<span data-ttu-id="55758-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55758-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55758-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55758-111">Permission type</span></span>      | <span data-ttu-id="55758-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55758-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55758-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55758-113">Delegated (work or school account)</span></span> | <span data-ttu-id="55758-114">Group.Read.All и User.ReadBasic.All, Group.Read.All и User.Read.All, Group.Read.All и User.ReadWrite.All, Group.Read.All и User.Read.All и Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="55758-114">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span>  |
|<span data-ttu-id="55758-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55758-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55758-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55758-116">Not supported.</span></span>    |
|<span data-ttu-id="55758-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55758-117">Application</span></span> | <span data-ttu-id="55758-118">Group.Read.All и User.Read.All, Group.Read.All и User.ReadWrite.All, Group.Read.All и User.Read.All и Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="55758-118">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="55758-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55758-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55758-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="55758-120">Optional query parameters</span></span>
<span data-ttu-id="55758-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="55758-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55758-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55758-122">Request headers</span></span>
| <span data-ttu-id="55758-123">Имя</span><span class="sxs-lookup"><span data-stu-id="55758-123">Name</span></span>       | <span data-ttu-id="55758-124">Тип</span><span class="sxs-lookup"><span data-stu-id="55758-124">Type</span></span> | <span data-ttu-id="55758-125">Описание</span><span class="sxs-lookup"><span data-stu-id="55758-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="55758-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="55758-126">Authorization</span></span>  | <span data-ttu-id="55758-127">string</span><span class="sxs-lookup"><span data-stu-id="55758-127">string</span></span>  | <span data-ttu-id="55758-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55758-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55758-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55758-130">Request body</span></span>
<span data-ttu-id="55758-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="55758-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55758-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="55758-132">Response</span></span>
<span data-ttu-id="55758-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="55758-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55758-134">Пример</span><span class="sxs-lookup"><span data-stu-id="55758-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="55758-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="55758-135">Request</span></span>
<span data-ttu-id="55758-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55758-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55758-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="55758-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="55758-138">C#</span><span class="sxs-lookup"><span data-stu-id="55758-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55758-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55758-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55758-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55758-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55758-141">Java</span><span class="sxs-lookup"><span data-stu-id="55758-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="55758-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="55758-142">Response</span></span>
<span data-ttu-id="55758-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="55758-143">The following is an example of the response.</span></span>
><span data-ttu-id="55758-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55758-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


