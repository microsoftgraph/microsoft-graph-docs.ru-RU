---
title: Список acceptedSenders
description: Получение списка пользователей или групп, включенных в список утвержденных отправителей для этой группы.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: cca956fdfc67a667133ba7ac6248402a734454d9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48012623"
---
# <a name="list-acceptedsenders"></a><span data-ttu-id="bb358-103">Список acceptedSenders</span><span class="sxs-lookup"><span data-stu-id="bb358-103">List acceptedSenders</span></span>

<span data-ttu-id="bb358-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb358-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb358-105">Получение списка пользователей или групп, включенных в список утвержденных отправителей для этой группы.</span><span class="sxs-lookup"><span data-stu-id="bb358-105">Get a list of users or groups that are in the accepted-senders list for this group.</span></span>

<span data-ttu-id="bb358-p101">Пользователи из списка разрешенных отправителей могут отправлять записи в беседы группы (определенные в URL-адресе запроса GET). Убедитесь, что в списках разрешенных и запрещенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="bb358-p101">Users in the accepted senders list can post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb358-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb358-108">Permissions</span></span>
<span data-ttu-id="bb358-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb358-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb358-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb358-111">Permission type</span></span>      | <span data-ttu-id="bb358-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb358-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb358-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb358-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bb358-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb358-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bb358-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb358-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb358-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb358-116">Not supported.</span></span>    |
|<span data-ttu-id="bb358-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb358-117">Application</span></span> | <span data-ttu-id="bb358-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb358-118">Not supported.</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="bb358-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb358-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/acceptedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bb358-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bb358-120">Optional query parameters</span></span>
<span data-ttu-id="bb358-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bb358-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb358-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb358-122">Request headers</span></span>
| <span data-ttu-id="bb358-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb358-123">Header</span></span>       | <span data-ttu-id="bb358-124">Значение</span><span class="sxs-lookup"><span data-stu-id="bb358-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bb358-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb358-125">Authorization</span></span>  | <span data-ttu-id="bb358-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb358-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bb358-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bb358-128">Request body</span></span>
<span data-ttu-id="bb358-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bb358-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb358-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb358-130">Response</span></span>
<span data-ttu-id="bb358-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb358-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb358-132">Пример</span><span class="sxs-lookup"><span data-stu-id="bb358-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bb358-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb358-133">Request</span></span>
<span data-ttu-id="bb358-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb358-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bb358-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb358-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_acceptedsenders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/acceptedSenders
```
# <a name="c"></a>[<span data-ttu-id="bb358-136">C#</span><span class="sxs-lookup"><span data-stu-id="bb358-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-acceptedsenders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb358-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb358-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-acceptedsenders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb358-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb358-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-acceptedsenders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bb358-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb358-139">Response</span></span>
<span data-ttu-id="bb358-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bb358-140">The following is an example of the response.</span></span>
><span data-ttu-id="bb358-141">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bb358-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bb358-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb358-142">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List acceptedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


