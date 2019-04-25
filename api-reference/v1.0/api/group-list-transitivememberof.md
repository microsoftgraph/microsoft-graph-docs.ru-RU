---
title: Список транзитивных групп memberOf
description: Получение групп, членом которых является группа.  Эта операция является транзитивным и также включает все группы, в которых вложены эти группы. В отличие от извлечения групп Office 365 пользователя, возвращаются все типы групп, а не только группы Office 365.
author: anchanda
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 7134318471101309dcf8f2778106afa549e9aa62
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542020"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="2f906-105">Список транзитивных групп memberOf</span><span class="sxs-lookup"><span data-stu-id="2f906-105">List group transitive memberOf</span></span>

<span data-ttu-id="2f906-106">Получение групп, членом которых является группа.</span><span class="sxs-lookup"><span data-stu-id="2f906-106">Get groups that the group is a member of.</span></span>  <span data-ttu-id="2f906-107">Эта операция является транзитивным и также включает все группы, в которых вложены эти группы.</span><span class="sxs-lookup"><span data-stu-id="2f906-107">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="2f906-108">В отличие от извлечения групп Office 365 пользователя, возвращаются все типы групп, а не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="2f906-108">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f906-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f906-109">Permissions</span></span>

<span data-ttu-id="2f906-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f906-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f906-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f906-112">Permission type</span></span>      | <span data-ttu-id="2f906-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f906-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f906-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f906-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2f906-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2f906-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2f906-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f906-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f906-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f906-117">Not supported.</span></span>    |
|<span data-ttu-id="2f906-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f906-118">Application</span></span> | <span data-ttu-id="2f906-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f906-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f906-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f906-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f906-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2f906-121">Optional query parameters</span></span>
<span data-ttu-id="2f906-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2f906-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f906-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f906-123">Request headers</span></span>
| <span data-ttu-id="2f906-124">Имя</span><span class="sxs-lookup"><span data-stu-id="2f906-124">Name</span></span>       | <span data-ttu-id="2f906-125">Тип</span><span class="sxs-lookup"><span data-stu-id="2f906-125">Type</span></span> | <span data-ttu-id="2f906-126">Описание</span><span class="sxs-lookup"><span data-stu-id="2f906-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2f906-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f906-127">Authorization</span></span>  | <span data-ttu-id="2f906-128">string</span><span class="sxs-lookup"><span data-stu-id="2f906-128">string</span></span>  | <span data-ttu-id="2f906-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f906-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f906-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f906-131">Request body</span></span>
<span data-ttu-id="2f906-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2f906-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f906-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f906-133">Response</span></span>
<span data-ttu-id="2f906-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2f906-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f906-135">Пример</span><span class="sxs-lookup"><span data-stu-id="2f906-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f906-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f906-136">Request</span></span>
<span data-ttu-id="2f906-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f906-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="2f906-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f906-138">Response</span></span>

<span data-ttu-id="2f906-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2f906-139">The following is an example of the response.</span></span>
><span data-ttu-id="2f906-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f906-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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