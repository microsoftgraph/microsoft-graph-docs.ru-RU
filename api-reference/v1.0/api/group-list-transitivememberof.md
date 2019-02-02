---
title: Доверия транзитивных член группы списка
description: Получите групп, которые должна быть членом группы.  Эта операция доверия транзитивных и также будет включать всех групп, которым будет вложенных членом этой группы. В отличие от начало пользователя Office 365 групп, возвращает все типы групп, не только группы Office 365.
author: anchanda
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 7134318471101309dcf8f2778106afa549e9aa62
ms.sourcegitcommit: d6209114cbbe8072e3ecf7eba23819ae5ace7db5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2019
ms.locfileid: "29694512"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="86ff6-105">Доверия транзитивных член группы списка</span><span class="sxs-lookup"><span data-stu-id="86ff6-105">List group transitive memberOf</span></span>

<span data-ttu-id="86ff6-106">Получите групп, которые должна быть членом группы.</span><span class="sxs-lookup"><span data-stu-id="86ff6-106">Get groups that the group is a member of.</span></span>  <span data-ttu-id="86ff6-107">Эта операция доверия транзитивных и также будет включать всех групп, которым будет вложенных членом этой группы.</span><span class="sxs-lookup"><span data-stu-id="86ff6-107">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="86ff6-108">В отличие от начало пользователя Office 365 групп, возвращает все типы групп, не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="86ff6-108">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="86ff6-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86ff6-109">Permissions</span></span>

<span data-ttu-id="86ff6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86ff6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86ff6-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86ff6-112">Permission type</span></span>      | <span data-ttu-id="86ff6-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86ff6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86ff6-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86ff6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="86ff6-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="86ff6-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="86ff6-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86ff6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86ff6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86ff6-117">Not supported.</span></span>    |
|<span data-ttu-id="86ff6-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86ff6-118">Application</span></span> | <span data-ttu-id="86ff6-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86ff6-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="86ff6-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86ff6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="86ff6-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="86ff6-121">Optional query parameters</span></span>
<span data-ttu-id="86ff6-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="86ff6-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86ff6-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86ff6-123">Request headers</span></span>
| <span data-ttu-id="86ff6-124">Имя</span><span class="sxs-lookup"><span data-stu-id="86ff6-124">Name</span></span>       | <span data-ttu-id="86ff6-125">Тип</span><span class="sxs-lookup"><span data-stu-id="86ff6-125">Type</span></span> | <span data-ttu-id="86ff6-126">Описание</span><span class="sxs-lookup"><span data-stu-id="86ff6-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="86ff6-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="86ff6-127">Authorization</span></span>  | <span data-ttu-id="86ff6-128">string</span><span class="sxs-lookup"><span data-stu-id="86ff6-128">string</span></span>  | <span data-ttu-id="86ff6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86ff6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86ff6-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86ff6-131">Request body</span></span>
<span data-ttu-id="86ff6-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="86ff6-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86ff6-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="86ff6-133">Response</span></span>
<span data-ttu-id="86ff6-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="86ff6-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86ff6-135">Пример</span><span class="sxs-lookup"><span data-stu-id="86ff6-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="86ff6-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="86ff6-136">Request</span></span>
<span data-ttu-id="86ff6-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86ff6-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="86ff6-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="86ff6-138">Response</span></span>

<span data-ttu-id="86ff6-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="86ff6-139">The following is an example of the response.</span></span>
><span data-ttu-id="86ff6-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86ff6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->