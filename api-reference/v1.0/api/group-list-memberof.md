---
title: Список memberOf
description: 'Получение групп, непосредственным членом которых является данная группа. '
ms.openlocfilehash: 9733fd1bc2def3642913887a228275744e17b61c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026000"
---
# <a name="list-memberof"></a><span data-ttu-id="fe5b9-103">Список memberOf</span><span class="sxs-lookup"><span data-stu-id="fe5b9-103">List memberOf</span></span>
<span data-ttu-id="fe5b9-104">Получение групп, непосредственным членом которых является данная группа.</span><span class="sxs-lookup"><span data-stu-id="fe5b9-104">Get groups that the group is a direct member of.</span></span> 

<span data-ttu-id="fe5b9-p101">Эта операция не является транзитивной. В отличие от аналогичной операции для функции "Группы Office 365", эта операция возвращает группы всех типов, а не только группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="fe5b9-p101">This operation is not transitive. Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe5b9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe5b9-107">Permissions</span></span>
<span data-ttu-id="fe5b9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe5b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe5b9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe5b9-110">Permission type</span></span>      | <span data-ttu-id="fe5b9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe5b9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe5b9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe5b9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fe5b9-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe5b9-113">Group.Read.All</span></span>    |
|<span data-ttu-id="fe5b9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe5b9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe5b9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe5b9-115">Not supported.</span></span>    |
|<span data-ttu-id="fe5b9-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="fe5b9-116">Application</span></span> | <span data-ttu-id="fe5b9-117">Group.Read.All Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe5b9-117">Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe5b9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe5b9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe5b9-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fe5b9-119">Optional query parameters</span></span>
<span data-ttu-id="fe5b9-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fe5b9-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe5b9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe5b9-121">Request headers</span></span>
| <span data-ttu-id="fe5b9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="fe5b9-122">Name</span></span>       | <span data-ttu-id="fe5b9-123">Тип</span><span class="sxs-lookup"><span data-stu-id="fe5b9-123">Type</span></span> | <span data-ttu-id="fe5b9-124">Описание</span><span class="sxs-lookup"><span data-stu-id="fe5b9-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fe5b9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe5b9-125">Authorization</span></span>  | <span data-ttu-id="fe5b9-126">string</span><span class="sxs-lookup"><span data-stu-id="fe5b9-126">string</span></span>  | <span data-ttu-id="fe5b9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe5b9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe5b9-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe5b9-129">Request body</span></span>
<span data-ttu-id="fe5b9-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fe5b9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe5b9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe5b9-131">Response</span></span>
<span data-ttu-id="fe5b9-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe5b9-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe5b9-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fe5b9-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fe5b9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe5b9-134">Request</span></span>
<span data-ttu-id="fe5b9-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe5b9-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/memberOf
```

#### <a name="response"></a><span data-ttu-id="fe5b9-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe5b9-136">Response</span></span>
<span data-ttu-id="fe5b9-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fe5b9-137">The following is an example of the response.</span></span>
><span data-ttu-id="fe5b9-138">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="fe5b9-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fe5b9-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe5b9-139">All the properties will be returned from an actual call.</span></span>
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