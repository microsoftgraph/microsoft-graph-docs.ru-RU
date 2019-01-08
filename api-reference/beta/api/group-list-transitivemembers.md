---
title: Доверия транзитивных членов группы списка
description: Получите список членов группы. Группы могут быть пользователи, контакты, устройства, субъектов-служб и других групп участников. Эта операция доверия транзитивных и возвратит списка всех вложенных элементов.
ms.openlocfilehash: 703515f4549e409d3711699c79671ed0b1a93cb3
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748558"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="247dc-105">Доверия транзитивных членов группы списка</span><span class="sxs-lookup"><span data-stu-id="247dc-105">List group transitive members</span></span>

> <span data-ttu-id="247dc-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="247dc-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="247dc-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="247dc-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="247dc-108">Получите список членов группы.</span><span class="sxs-lookup"><span data-stu-id="247dc-108">Get a list of the group's members.</span></span> <span data-ttu-id="247dc-109">Группы могут быть пользователи, контакты, устройства, субъектов-служб и других групп участников.</span><span class="sxs-lookup"><span data-stu-id="247dc-109">A group can have users, contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="247dc-110">Эта операция доверия транзитивных и возвратит списка всех вложенных элементов.</span><span class="sxs-lookup"><span data-stu-id="247dc-110">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="247dc-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="247dc-111">Permissions</span></span>

<span data-ttu-id="247dc-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="247dc-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="247dc-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="247dc-114">Permission type</span></span>      | <span data-ttu-id="247dc-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="247dc-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="247dc-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="247dc-116">Delegated (work or school account)</span></span> | <span data-ttu-id="247dc-117">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="247dc-117">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="247dc-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="247dc-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="247dc-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="247dc-119">Not supported.</span></span>    |
|<span data-ttu-id="247dc-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="247dc-120">Application</span></span> | <span data-ttu-id="247dc-121">Directory.Read.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="247dc-121">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="247dc-122">Примечание: Чтобы просмотреть список членов группы скрытое членство, Member.Read.Hidden разрешение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="247dc-122">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="247dc-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="247dc-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="247dc-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="247dc-124">Optional query parameters</span></span>

<span data-ttu-id="247dc-125">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="247dc-125">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="247dc-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="247dc-126">Request headers</span></span>

| <span data-ttu-id="247dc-127">Имя</span><span class="sxs-lookup"><span data-stu-id="247dc-127">Name</span></span>       | <span data-ttu-id="247dc-128">Тип</span><span class="sxs-lookup"><span data-stu-id="247dc-128">Type</span></span> | <span data-ttu-id="247dc-129">Описание</span><span class="sxs-lookup"><span data-stu-id="247dc-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="247dc-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="247dc-130">Authorization</span></span>  | <span data-ttu-id="247dc-131">string</span><span class="sxs-lookup"><span data-stu-id="247dc-131">string</span></span>  | <span data-ttu-id="247dc-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="247dc-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="247dc-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="247dc-134">Request body</span></span>

<span data-ttu-id="247dc-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="247dc-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="247dc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="247dc-136">Response</span></span>

<span data-ttu-id="247dc-137">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="247dc-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="247dc-138">Пример</span><span class="sxs-lookup"><span data-stu-id="247dc-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="247dc-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="247dc-139">Request</span></span>

<span data-ttu-id="247dc-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="247dc-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```

### <a name="response"></a><span data-ttu-id="247dc-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="247dc-141">Response</span></span>

<span data-ttu-id="247dc-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="247dc-142">The following is an example of the response.</span></span>
><span data-ttu-id="247dc-143">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="247dc-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="247dc-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="247dc-144">All the properties will be returned from an actual call.</span></span>
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
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
