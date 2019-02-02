---
title: Доверия транзитивных членов группы списка
description: Получите список членов группы. Группы могут быть пользователи, устройств и других групп участников. Эта операция доверия транзитивных и возвратит списка всех вложенных элементов.
author: anchanda
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: dd6417916a7d1e2f79735db3dce4f1c3465d6577
ms.sourcegitcommit: d6209114cbbe8072e3ecf7eba23819ae5ace7db5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2019
ms.locfileid: "29694505"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="98cdf-105">Доверия транзитивных членов группы списка</span><span class="sxs-lookup"><span data-stu-id="98cdf-105">List group transitive members</span></span>

<span data-ttu-id="98cdf-106">Получите список членов группы.</span><span class="sxs-lookup"><span data-stu-id="98cdf-106">Get a list of the group's members.</span></span> <span data-ttu-id="98cdf-107">Группы могут быть пользователи, устройств и других групп участников.</span><span class="sxs-lookup"><span data-stu-id="98cdf-107">A group can have users, devices and other groups as members.</span></span> <span data-ttu-id="98cdf-108">Эта операция доверия транзитивных и возвратит списка всех вложенных элементов.</span><span class="sxs-lookup"><span data-stu-id="98cdf-108">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="98cdf-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98cdf-109">Permissions</span></span>

<span data-ttu-id="98cdf-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98cdf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98cdf-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98cdf-112">Permission type</span></span>      | <span data-ttu-id="98cdf-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98cdf-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98cdf-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98cdf-114">Delegated (work or school account)</span></span> | <span data-ttu-id="98cdf-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="98cdf-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="98cdf-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98cdf-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98cdf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98cdf-117">Not supported.</span></span>    |
|<span data-ttu-id="98cdf-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98cdf-118">Application</span></span> | <span data-ttu-id="98cdf-119">Directory.Read.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="98cdf-119">Directory.Read.All, User.Read.All</span></span> |

><span data-ttu-id="98cdf-120">**Примечание:** Чтобы получить список членов группы скрытое членство, Member.Read.Hidden разрешение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="98cdf-120">**Note:** To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="98cdf-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98cdf-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="98cdf-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="98cdf-122">Optional query parameters</span></span>

<span data-ttu-id="98cdf-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="98cdf-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="98cdf-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98cdf-124">Request headers</span></span>

| <span data-ttu-id="98cdf-125">Имя</span><span class="sxs-lookup"><span data-stu-id="98cdf-125">Name</span></span>       | <span data-ttu-id="98cdf-126">Тип</span><span class="sxs-lookup"><span data-stu-id="98cdf-126">Type</span></span> | <span data-ttu-id="98cdf-127">Описание</span><span class="sxs-lookup"><span data-stu-id="98cdf-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="98cdf-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="98cdf-128">Authorization</span></span>  | <span data-ttu-id="98cdf-129">string</span><span class="sxs-lookup"><span data-stu-id="98cdf-129">string</span></span>  | <span data-ttu-id="98cdf-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98cdf-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98cdf-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98cdf-132">Request body</span></span>

<span data-ttu-id="98cdf-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98cdf-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98cdf-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="98cdf-134">Response</span></span>

<span data-ttu-id="98cdf-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="98cdf-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98cdf-136">Пример</span><span class="sxs-lookup"><span data-stu-id="98cdf-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="98cdf-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="98cdf-137">Request</span></span>

<span data-ttu-id="98cdf-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98cdf-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMembers
```

### <a name="response"></a><span data-ttu-id="98cdf-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="98cdf-139">Response</span></span>

<span data-ttu-id="98cdf-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="98cdf-140">The following is an example of the response.</span></span>
><span data-ttu-id="98cdf-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98cdf-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
