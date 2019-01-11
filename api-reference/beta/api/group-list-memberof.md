---
title: Член группы списка
description: Получите административные единиц измерения, которые группа является непосредственным членом и группы.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 8a1badf9e52c9d0bc3319178f36d62d1327d3c63
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853335"
---
# <a name="list-group-memberof"></a><span data-ttu-id="4f093-103">Член группы списка</span><span class="sxs-lookup"><span data-stu-id="4f093-103">List group memberOf</span></span>

> <span data-ttu-id="4f093-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4f093-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f093-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f093-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4f093-106">Получите административные единиц измерения, которые группа является непосредственным членом и группы.</span><span class="sxs-lookup"><span data-stu-id="4f093-106">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="4f093-107">Эта операция не транзитивное.</span><span class="sxs-lookup"><span data-stu-id="4f093-107">This operation is not transitive.</span></span> <span data-ttu-id="4f093-108">В отличие от начало пользователя Office 365 групп, возвращает все типы групп, не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="4f093-108">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4f093-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f093-109">Permissions</span></span>

<span data-ttu-id="4f093-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f093-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f093-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f093-112">Permission type</span></span>      | <span data-ttu-id="4f093-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f093-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f093-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f093-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4f093-115">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4f093-115">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4f093-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f093-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f093-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f093-117">Not supported.</span></span>    |
|<span data-ttu-id="4f093-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f093-118">Application</span></span> | <span data-ttu-id="4f093-119">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f093-119">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f093-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f093-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f093-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4f093-121">Optional query parameters</span></span>
<span data-ttu-id="4f093-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4f093-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f093-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f093-123">Request headers</span></span>
| <span data-ttu-id="4f093-124">Имя</span><span class="sxs-lookup"><span data-stu-id="4f093-124">Name</span></span>       | <span data-ttu-id="4f093-125">Тип</span><span class="sxs-lookup"><span data-stu-id="4f093-125">Type</span></span> | <span data-ttu-id="4f093-126">Описание</span><span class="sxs-lookup"><span data-stu-id="4f093-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4f093-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f093-127">Authorization</span></span>  | <span data-ttu-id="4f093-128">string</span><span class="sxs-lookup"><span data-stu-id="4f093-128">string</span></span>  | <span data-ttu-id="4f093-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f093-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f093-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4f093-131">Request body</span></span>
<span data-ttu-id="4f093-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f093-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f093-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f093-133">Response</span></span>
<span data-ttu-id="4f093-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4f093-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f093-135">Пример</span><span class="sxs-lookup"><span data-stu-id="4f093-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f093-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f093-136">Request</span></span>

<span data-ttu-id="4f093-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f093-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="4f093-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f093-138">Response</span></span>

<span data-ttu-id="4f093-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4f093-139">The following is an example of the response.</span></span>
><span data-ttu-id="4f093-140">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="4f093-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4f093-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f093-141">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
