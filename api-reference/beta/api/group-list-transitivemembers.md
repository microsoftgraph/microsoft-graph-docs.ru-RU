---
title: Список транзитивных членов группы
description: Получение списка членов группы.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9116569521cb024cd6501e448f8dccad61f64260
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43396819"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="73bf0-103">Список транзитивных членов группы</span><span class="sxs-lookup"><span data-stu-id="73bf0-103">List group transitive members</span></span>

<span data-ttu-id="73bf0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73bf0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73bf0-105">Получение списка членов группы.</span><span class="sxs-lookup"><span data-stu-id="73bf0-105">Get a list of the group's members.</span></span> <span data-ttu-id="73bf0-106">У группы могут быть пользователи, контакты, устройства, субъекты служб и другие группы в качестве участников.</span><span class="sxs-lookup"><span data-stu-id="73bf0-106">A group can have users, contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="73bf0-107">Эта операция является транзитивным и также возвращает плоский список всех вложенных элементов.</span><span class="sxs-lookup"><span data-stu-id="73bf0-107">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="73bf0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73bf0-108">Permissions</span></span>

<span data-ttu-id="73bf0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73bf0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73bf0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73bf0-111">Permission type</span></span>      | <span data-ttu-id="73bf0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73bf0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73bf0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73bf0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="73bf0-114">Directory. Read. ALL, Directory. AccessAsUser. ALL, User. ReadBasic. ALL, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="73bf0-114">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="73bf0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73bf0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73bf0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73bf0-116">Not supported.</span></span>    |
|<span data-ttu-id="73bf0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73bf0-117">Application</span></span> | <span data-ttu-id="73bf0-118">Directory. Read. ALL, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="73bf0-118">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="73bf0-119">Note: чтобы получить список членов скрытой группы членства, требуется разрешение Member. Read. Hidden.</span><span class="sxs-lookup"><span data-stu-id="73bf0-119">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="73bf0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73bf0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73bf0-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="73bf0-121">Optional query parameters</span></span>

<span data-ttu-id="73bf0-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="73bf0-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73bf0-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73bf0-123">Request headers</span></span>

| <span data-ttu-id="73bf0-124">Имя</span><span class="sxs-lookup"><span data-stu-id="73bf0-124">Name</span></span>       | <span data-ttu-id="73bf0-125">Тип</span><span class="sxs-lookup"><span data-stu-id="73bf0-125">Type</span></span> | <span data-ttu-id="73bf0-126">Описание</span><span class="sxs-lookup"><span data-stu-id="73bf0-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="73bf0-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="73bf0-127">Authorization</span></span>  | <span data-ttu-id="73bf0-128">string</span><span class="sxs-lookup"><span data-stu-id="73bf0-128">string</span></span>  | <span data-ttu-id="73bf0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73bf0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73bf0-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="73bf0-131">Request body</span></span>

<span data-ttu-id="73bf0-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73bf0-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73bf0-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="73bf0-133">Response</span></span>

<span data-ttu-id="73bf0-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="73bf0-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73bf0-135">Пример</span><span class="sxs-lookup"><span data-stu-id="73bf0-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="73bf0-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="73bf0-136">Request</span></span>

<span data-ttu-id="73bf0-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73bf0-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="73bf0-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="73bf0-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="73bf0-139">C#</span><span class="sxs-lookup"><span data-stu-id="73bf0-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73bf0-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73bf0-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73bf0-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73bf0-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="73bf0-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="73bf0-142">Response</span></span>

<span data-ttu-id="73bf0-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="73bf0-143">The following is an example of the response.</span></span>
><span data-ttu-id="73bf0-144">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="73bf0-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="73bf0-145">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73bf0-145">All the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
