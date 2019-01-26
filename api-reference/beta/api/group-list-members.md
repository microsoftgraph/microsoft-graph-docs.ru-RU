---
title: Список членов группы
description: Ознакомьтесь со списком прямое членов группы. Группы могут быть пользователи, контакты, устройств, субъектов-служб и других групп участников. Эта операция не транзитивное.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 07004a315bc2b35777c080f7bbdbab8f433f0942
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577454"
---
# <a name="list-group-members"></a><span data-ttu-id="30abf-105">Список членов группы</span><span class="sxs-lookup"><span data-stu-id="30abf-105">List group members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30abf-106">Ознакомьтесь со списком прямое членов группы.</span><span class="sxs-lookup"><span data-stu-id="30abf-106">Get a list of the group's direct members.</span></span> <span data-ttu-id="30abf-107">Группы могут быть пользователи, контакты, устройств, субъектов-служб и других групп участников.</span><span class="sxs-lookup"><span data-stu-id="30abf-107">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="30abf-108">Эта операция не транзитивное.</span><span class="sxs-lookup"><span data-stu-id="30abf-108">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="30abf-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30abf-109">Permissions</span></span>

<span data-ttu-id="30abf-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30abf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30abf-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30abf-112">Permission type</span></span>      | <span data-ttu-id="30abf-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30abf-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30abf-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30abf-114">Delegated (work or school account)</span></span> | <span data-ttu-id="30abf-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="30abf-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="30abf-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30abf-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30abf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30abf-117">Not supported.</span></span>    |
|<span data-ttu-id="30abf-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30abf-118">Application</span></span> | <span data-ttu-id="30abf-119">Directory.Read.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="30abf-119">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="30abf-120">Примечание: Чтобы просмотреть список членов группы скрытое членство, Member.Read.Hidden разрешение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="30abf-120">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>
 
## <a name="http-request"></a><span data-ttu-id="30abf-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30abf-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="30abf-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="30abf-122">Optional query parameters</span></span>
<span data-ttu-id="30abf-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="30abf-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30abf-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30abf-124">Request headers</span></span>
| <span data-ttu-id="30abf-125">Имя</span><span class="sxs-lookup"><span data-stu-id="30abf-125">Name</span></span>       | <span data-ttu-id="30abf-126">Тип</span><span class="sxs-lookup"><span data-stu-id="30abf-126">Type</span></span> | <span data-ttu-id="30abf-127">Описание</span><span class="sxs-lookup"><span data-stu-id="30abf-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="30abf-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="30abf-128">Authorization</span></span>  | <span data-ttu-id="30abf-129">string</span><span class="sxs-lookup"><span data-stu-id="30abf-129">string</span></span>  | <span data-ttu-id="30abf-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30abf-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30abf-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30abf-132">Request body</span></span>
<span data-ttu-id="30abf-133">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30abf-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30abf-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="30abf-134">Response</span></span>
<span data-ttu-id="30abf-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30abf-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30abf-136">Пример</span><span class="sxs-lookup"><span data-stu-id="30abf-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="30abf-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="30abf-137">Request</span></span>
<span data-ttu-id="30abf-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30abf-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/members
```

#### <a name="response"></a><span data-ttu-id="30abf-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="30abf-139">Response</span></span>
<span data-ttu-id="30abf-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="30abf-140">The following is an example of the response.</span></span>
><span data-ttu-id="30abf-141">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="30abf-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="30abf-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30abf-142">All the properties will be returned from an actual call.</span></span>
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
  "description": "List group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
