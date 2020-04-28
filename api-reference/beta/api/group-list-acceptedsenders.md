---
title: Список acceptedSenders
description: Получение списка пользователей или групп, включенных в список утвержденных отправителей для этой группы.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: de7c7216af4e79547db7963e63d9cd60565740c5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43397192"
---
# <a name="list-acceptedsenders"></a><span data-ttu-id="14a2c-103">Список acceptedSenders</span><span class="sxs-lookup"><span data-stu-id="14a2c-103">List acceptedSenders</span></span>

<span data-ttu-id="14a2c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14a2c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14a2c-105">Получение списка пользователей или групп, включенных в список утвержденных отправителей для этой группы.</span><span class="sxs-lookup"><span data-stu-id="14a2c-105">Get a list of users or groups that are in the accepted-senders list for this group.</span></span>

<span data-ttu-id="14a2c-p101">Пользователи из списка разрешенных отправителей могут отправлять записи в беседы группы (определенные в URL-адресе запроса GET). Убедитесь, что в списках разрешенных и запрещенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="14a2c-p101">Users in the accepted senders list can post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="14a2c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14a2c-108">Permissions</span></span>
<span data-ttu-id="14a2c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14a2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14a2c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14a2c-111">Permission type</span></span>      | <span data-ttu-id="14a2c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14a2c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14a2c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14a2c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="14a2c-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14a2c-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="14a2c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14a2c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14a2c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14a2c-116">Not supported.</span></span>    |
|<span data-ttu-id="14a2c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14a2c-117">Application</span></span> | <span data-ttu-id="14a2c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14a2c-118">Not supported.</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="14a2c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14a2c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/acceptedSenders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="14a2c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="14a2c-120">Optional query parameters</span></span>
<span data-ttu-id="14a2c-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="14a2c-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="14a2c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14a2c-122">Request headers</span></span>
| <span data-ttu-id="14a2c-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14a2c-123">Header</span></span>       | <span data-ttu-id="14a2c-124">Значение</span><span class="sxs-lookup"><span data-stu-id="14a2c-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="14a2c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14a2c-125">Authorization</span></span>  | <span data-ttu-id="14a2c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14a2c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="14a2c-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="14a2c-128">Request body</span></span>
<span data-ttu-id="14a2c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="14a2c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14a2c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="14a2c-130">Response</span></span>
<span data-ttu-id="14a2c-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="14a2c-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14a2c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="14a2c-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="14a2c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="14a2c-133">Request</span></span>
<span data-ttu-id="14a2c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14a2c-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="14a2c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="14a2c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_acceptedsenders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/acceptedSenders
```
# <a name="c"></a>[<span data-ttu-id="14a2c-136">C#</span><span class="sxs-lookup"><span data-stu-id="14a2c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-acceptedsenders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14a2c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14a2c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-acceptedsenders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14a2c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14a2c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-acceptedsenders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="14a2c-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="14a2c-139">Response</span></span>
<span data-ttu-id="14a2c-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="14a2c-140">The following is an example of the response.</span></span>
><span data-ttu-id="14a2c-141">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="14a2c-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="14a2c-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14a2c-142">All the properties will be returned from an actual call.</span></span>
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
