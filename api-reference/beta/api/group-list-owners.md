---
title: Список владельцев
description: Получение списка владельцев группы. Владельцы — это пользователи, которые не являются администраторами и которым разрешено изменять объект группы.
ms.openlocfilehash: 2b3584e5037c9ac36ac4bff97ef64af21643eb31
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082083"
---
# <a name="list-owners"></a><span data-ttu-id="64cc1-104">Список владельцев</span><span class="sxs-lookup"><span data-stu-id="64cc1-104">List owners</span></span>

> <span data-ttu-id="64cc1-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="64cc1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64cc1-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64cc1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="64cc1-p103">Получение списка владельцев группы. Владельцы — это пользователи, которые не являются администраторами и которым разрешено изменять объект группы.</span><span class="sxs-lookup"><span data-stu-id="64cc1-p103">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="64cc1-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64cc1-109">Permissions</span></span>
<span data-ttu-id="64cc1-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64cc1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64cc1-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64cc1-112">Permission type</span></span>      | <span data-ttu-id="64cc1-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64cc1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64cc1-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64cc1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="64cc1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64cc1-115">Not supported.</span></span>    |
|<span data-ttu-id="64cc1-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64cc1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64cc1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64cc1-117">Not supported.</span></span>    |
|<span data-ttu-id="64cc1-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64cc1-118">Application</span></span> | <span data-ttu-id="64cc1-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64cc1-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64cc1-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64cc1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64cc1-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="64cc1-121">Optional query parameters</span></span>
<span data-ttu-id="64cc1-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="64cc1-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64cc1-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64cc1-123">Request headers</span></span>
| <span data-ttu-id="64cc1-124">Имя</span><span class="sxs-lookup"><span data-stu-id="64cc1-124">Name</span></span>       | <span data-ttu-id="64cc1-125">Тип</span><span class="sxs-lookup"><span data-stu-id="64cc1-125">Type</span></span> | <span data-ttu-id="64cc1-126">Описание</span><span class="sxs-lookup"><span data-stu-id="64cc1-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="64cc1-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="64cc1-127">Authorization</span></span>  | <span data-ttu-id="64cc1-128">string</span><span class="sxs-lookup"><span data-stu-id="64cc1-128">string</span></span>  | <span data-ttu-id="64cc1-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64cc1-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64cc1-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64cc1-131">Request body</span></span>
<span data-ttu-id="64cc1-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64cc1-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64cc1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="64cc1-133">Response</span></span>
<span data-ttu-id="64cc1-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="64cc1-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64cc1-135">Пример</span><span class="sxs-lookup"><span data-stu-id="64cc1-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="64cc1-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="64cc1-136">Request</span></span>
<span data-ttu-id="64cc1-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64cc1-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="64cc1-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="64cc1-138">Response</span></span>
<span data-ttu-id="64cc1-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="64cc1-139">The following is an example of the response.</span></span>
><span data-ttu-id="64cc1-140">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="64cc1-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="64cc1-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64cc1-141">All the properties will be returned from an actual call.</span></span>
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
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->