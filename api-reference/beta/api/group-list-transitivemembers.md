---
title: Список транзитивных членов группы
description: Получение списка членов группы. У группы могут быть пользователи, контакты, устройства, субъекты служб и другие группы в качестве участников. Эта операция является транзитивным и также возвращает плоский список всех вложенных элементов.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: fad3ad81268de77116b912153541ca7d147c563a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592782"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="16025-105">Список транзитивных членов группы</span><span class="sxs-lookup"><span data-stu-id="16025-105">List group transitive members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16025-106">Получение списка членов группы.</span><span class="sxs-lookup"><span data-stu-id="16025-106">Get a list of the group's members.</span></span> <span data-ttu-id="16025-107">У группы могут быть пользователи, контакты, устройства, субъекты служб и другие группы в качестве участников.</span><span class="sxs-lookup"><span data-stu-id="16025-107">A group can have users, contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="16025-108">Эта операция является транзитивным и также возвращает плоский список всех вложенных элементов.</span><span class="sxs-lookup"><span data-stu-id="16025-108">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="16025-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16025-109">Permissions</span></span>

<span data-ttu-id="16025-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16025-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16025-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16025-112">Permission type</span></span>      | <span data-ttu-id="16025-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16025-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16025-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16025-114">Delegated (work or school account)</span></span> | <span data-ttu-id="16025-115">Directory. Read. ALL, Directory. AccessAsUser. ALL, User. ReadBasic. ALL, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="16025-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="16025-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16025-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16025-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16025-117">Not supported.</span></span>    |
|<span data-ttu-id="16025-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16025-118">Application</span></span> | <span data-ttu-id="16025-119">Directory. Read. ALL, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="16025-119">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="16025-120">Note: чтобы получить список членов скрытой группы членства, требуется разрешение Member. Read. Hidden.</span><span class="sxs-lookup"><span data-stu-id="16025-120">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="16025-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16025-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16025-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="16025-122">Optional query parameters</span></span>

<span data-ttu-id="16025-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="16025-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16025-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16025-124">Request headers</span></span>

| <span data-ttu-id="16025-125">Имя</span><span class="sxs-lookup"><span data-stu-id="16025-125">Name</span></span>       | <span data-ttu-id="16025-126">Тип</span><span class="sxs-lookup"><span data-stu-id="16025-126">Type</span></span> | <span data-ttu-id="16025-127">Описание</span><span class="sxs-lookup"><span data-stu-id="16025-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="16025-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="16025-128">Authorization</span></span>  | <span data-ttu-id="16025-129">string</span><span class="sxs-lookup"><span data-stu-id="16025-129">string</span></span>  | <span data-ttu-id="16025-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16025-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16025-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16025-132">Request body</span></span>

<span data-ttu-id="16025-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16025-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16025-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="16025-134">Response</span></span>

<span data-ttu-id="16025-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16025-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16025-136">Пример</span><span class="sxs-lookup"><span data-stu-id="16025-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="16025-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="16025-137">Request</span></span>

<span data-ttu-id="16025-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16025-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```

### <a name="response"></a><span data-ttu-id="16025-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="16025-139">Response</span></span>

<span data-ttu-id="16025-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="16025-140">The following is an example of the response.</span></span>
><span data-ttu-id="16025-141">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="16025-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="16025-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16025-142">All the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.user",
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="16025-143">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="16025-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="16025-144">Языках</span><span class="sxs-lookup"><span data-stu-id="16025-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_transitivemembers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="16025-145">Язык</span><span class="sxs-lookup"><span data-stu-id="16025-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_transitivemembers-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-transitivemembers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-transitivemembers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
