---
title: Группа списка memberOf
description: Получение групп и административных единиц, непосредственным участником которых является группа.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4b4edb12a1b620c77f844d1e2a5d5f5a7751a249
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419438"
---
# <a name="list-group-memberof"></a><span data-ttu-id="a4213-103">Группа списка memberOf</span><span class="sxs-lookup"><span data-stu-id="a4213-103">List group memberOf</span></span>

<span data-ttu-id="a4213-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a4213-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4213-105">Получение групп и административных единиц, непосредственным участником которых является группа.</span><span class="sxs-lookup"><span data-stu-id="a4213-105">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="a4213-106">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="a4213-106">This operation is not transitive.</span></span> <span data-ttu-id="a4213-107">В отличие от извлечения групп Office 365 пользователя, возвращаются все типы групп, а не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="a4213-107">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a4213-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4213-108">Permissions</span></span>

<span data-ttu-id="a4213-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4213-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4213-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4213-111">Permission type</span></span>      | <span data-ttu-id="a4213-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4213-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4213-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4213-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a4213-114">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a4213-114">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a4213-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4213-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4213-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4213-116">Not supported.</span></span>    |
|<span data-ttu-id="a4213-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="a4213-117">Application</span></span> | <span data-ttu-id="a4213-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4213-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="a4213-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4213-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a4213-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a4213-120">Optional query parameters</span></span>
<span data-ttu-id="a4213-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a4213-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4213-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4213-122">Request headers</span></span>
| <span data-ttu-id="a4213-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a4213-123">Name</span></span>       | <span data-ttu-id="a4213-124">Тип</span><span class="sxs-lookup"><span data-stu-id="a4213-124">Type</span></span> | <span data-ttu-id="a4213-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a4213-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a4213-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4213-126">Authorization</span></span>  | <span data-ttu-id="a4213-127">string</span><span class="sxs-lookup"><span data-stu-id="a4213-127">string</span></span>  | <span data-ttu-id="a4213-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4213-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4213-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4213-130">Request body</span></span>
<span data-ttu-id="a4213-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a4213-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4213-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4213-132">Response</span></span>
<span data-ttu-id="a4213-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a4213-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4213-134">Пример</span><span class="sxs-lookup"><span data-stu-id="a4213-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4213-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4213-135">Request</span></span>

<span data-ttu-id="a4213-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4213-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a4213-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4213-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="a4213-138">C#</span><span class="sxs-lookup"><span data-stu-id="a4213-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4213-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4213-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4213-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4213-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a4213-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4213-141">Response</span></span>

<span data-ttu-id="a4213-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a4213-142">The following is an example of the response.</span></span>
><span data-ttu-id="a4213-143">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a4213-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a4213-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4213-144">All the properties will be returned from an actual call.</span></span>
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
