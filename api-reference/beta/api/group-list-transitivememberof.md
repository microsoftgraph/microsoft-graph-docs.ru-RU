---
title: Доверия транзитивных член группы списка
description: Получите административные единиц измерения, которые должна быть членом группы и группы.  Эта операция доверия транзитивных и также будет включать всех групп, которым будет вложенных членом этой группы. В отличие от начало пользователя Office 365 групп, возвращает все типы групп, не только группы Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 95d191973a327e6b3e1b0c7e692e0d581744e0ee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515834"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="5e3ad-105">Доверия транзитивных член группы списка</span><span class="sxs-lookup"><span data-stu-id="5e3ad-105">List group transitive memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e3ad-106">Получите административные единиц измерения, которые должна быть членом группы и группы.</span><span class="sxs-lookup"><span data-stu-id="5e3ad-106">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="5e3ad-107">Эта операция доверия транзитивных и также будет включать всех групп, которым будет вложенных членом этой группы.</span><span class="sxs-lookup"><span data-stu-id="5e3ad-107">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="5e3ad-108">В отличие от начало пользователя Office 365 групп, возвращает все типы групп, не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="5e3ad-108">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e3ad-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5e3ad-109">Permissions</span></span>

<span data-ttu-id="5e3ad-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e3ad-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e3ad-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e3ad-112">Permission type</span></span>      | <span data-ttu-id="5e3ad-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e3ad-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e3ad-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e3ad-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5e3ad-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5e3ad-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5e3ad-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e3ad-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e3ad-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e3ad-117">Not supported.</span></span>    |
|<span data-ttu-id="5e3ad-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e3ad-118">Application</span></span> | <span data-ttu-id="5e3ad-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e3ad-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e3ad-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e3ad-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5e3ad-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5e3ad-121">Optional query parameters</span></span>
<span data-ttu-id="5e3ad-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5e3ad-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e3ad-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e3ad-123">Request headers</span></span>
| <span data-ttu-id="5e3ad-124">Имя</span><span class="sxs-lookup"><span data-stu-id="5e3ad-124">Name</span></span>       | <span data-ttu-id="5e3ad-125">Тип</span><span class="sxs-lookup"><span data-stu-id="5e3ad-125">Type</span></span> | <span data-ttu-id="5e3ad-126">Описание</span><span class="sxs-lookup"><span data-stu-id="5e3ad-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5e3ad-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e3ad-127">Authorization</span></span>  | <span data-ttu-id="5e3ad-128">string</span><span class="sxs-lookup"><span data-stu-id="5e3ad-128">string</span></span>  | <span data-ttu-id="5e3ad-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e3ad-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e3ad-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e3ad-131">Request body</span></span>
<span data-ttu-id="5e3ad-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5e3ad-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e3ad-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="5e3ad-133">Response</span></span>
<span data-ttu-id="5e3ad-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e3ad-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e3ad-135">Пример</span><span class="sxs-lookup"><span data-stu-id="5e3ad-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e3ad-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e3ad-136">Request</span></span>
<span data-ttu-id="5e3ad-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e3ad-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="5e3ad-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="5e3ad-138">Response</span></span>

<span data-ttu-id="5e3ad-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5e3ad-139">The following is an example of the response.</span></span>
><span data-ttu-id="5e3ad-140">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5e3ad-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5e3ad-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e3ad-141">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-transitivememberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
