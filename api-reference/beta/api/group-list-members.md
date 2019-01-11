---
title: Список членов группы
description: Ознакомьтесь со списком прямое членов группы. Группы могут быть пользователи, контакты, устройств, субъектов-служб и других групп участников. Эта операция не транзитивное.
localization_priority: Normal
ms.openlocfilehash: af54ef994fb0f62af43bf9f9ce3cd5fe5d2b1503
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854140"
---
# <a name="list-group-members"></a><span data-ttu-id="15a16-105">Список членов группы</span><span class="sxs-lookup"><span data-stu-id="15a16-105">List group members</span></span>

> <span data-ttu-id="15a16-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="15a16-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15a16-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15a16-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15a16-108">Ознакомьтесь со списком прямое членов группы.</span><span class="sxs-lookup"><span data-stu-id="15a16-108">Get a list of the group's direct members.</span></span> <span data-ttu-id="15a16-109">Группы могут быть пользователи, контакты, устройств, субъектов-служб и других групп участников.</span><span class="sxs-lookup"><span data-stu-id="15a16-109">A group can have users, contacts, devices, service principals, and other groups as members.</span></span> <span data-ttu-id="15a16-110">Эта операция не транзитивное.</span><span class="sxs-lookup"><span data-stu-id="15a16-110">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="15a16-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15a16-111">Permissions</span></span>

<span data-ttu-id="15a16-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15a16-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15a16-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15a16-114">Permission type</span></span>      | <span data-ttu-id="15a16-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15a16-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15a16-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15a16-116">Delegated (work or school account)</span></span> | <span data-ttu-id="15a16-117">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="15a16-117">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="15a16-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15a16-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15a16-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15a16-119">Not supported.</span></span>    |
|<span data-ttu-id="15a16-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15a16-120">Application</span></span> | <span data-ttu-id="15a16-121">Directory.Read.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="15a16-121">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="15a16-122">Примечание: Чтобы просмотреть список членов группы скрытое членство, Member.Read.Hidden разрешение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="15a16-122">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>
 
## <a name="http-request"></a><span data-ttu-id="15a16-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15a16-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="15a16-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="15a16-124">Optional query parameters</span></span>
<span data-ttu-id="15a16-125">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="15a16-125">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15a16-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15a16-126">Request headers</span></span>
| <span data-ttu-id="15a16-127">Имя</span><span class="sxs-lookup"><span data-stu-id="15a16-127">Name</span></span>       | <span data-ttu-id="15a16-128">Тип</span><span class="sxs-lookup"><span data-stu-id="15a16-128">Type</span></span> | <span data-ttu-id="15a16-129">Описание</span><span class="sxs-lookup"><span data-stu-id="15a16-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="15a16-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="15a16-130">Authorization</span></span>  | <span data-ttu-id="15a16-131">string</span><span class="sxs-lookup"><span data-stu-id="15a16-131">string</span></span>  | <span data-ttu-id="15a16-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15a16-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15a16-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="15a16-134">Request body</span></span>
<span data-ttu-id="15a16-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="15a16-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15a16-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="15a16-136">Response</span></span>
<span data-ttu-id="15a16-137">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="15a16-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15a16-138">Пример</span><span class="sxs-lookup"><span data-stu-id="15a16-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="15a16-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="15a16-139">Request</span></span>
<span data-ttu-id="15a16-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15a16-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_members"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/members
```

#### <a name="response"></a><span data-ttu-id="15a16-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="15a16-141">Response</span></span>
<span data-ttu-id="15a16-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="15a16-142">The following is an example of the response.</span></span>
><span data-ttu-id="15a16-143">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="15a16-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="15a16-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15a16-144">All the properties will be returned from an actual call.</span></span>
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
    "@odata.type": "#microsoft.graph.user",
    {
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
<!-- {
  "type": "#page.annotation",
  "description": "List group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
