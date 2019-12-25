---
title: Список rejectedSenders
description: 'Получение списка пользователей или групп, включенных в список запрещенных отправителей для этой группы. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 70d16e75e54320ecbdf68657abedc33a813c3bda
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864742"
---
# <a name="list-rejectedsenders"></a><span data-ttu-id="ccba3-103">Список rejectedSenders</span><span class="sxs-lookup"><span data-stu-id="ccba3-103">List rejectedSenders</span></span>
<span data-ttu-id="ccba3-104">Получение списка пользователей или групп, включенных в список запрещенных отправителей для этой группы.</span><span class="sxs-lookup"><span data-stu-id="ccba3-104">Get a list of users or groups that are in the rejected-senders list for this group.</span></span> 

<span data-ttu-id="ccba3-p101">Пользователи из списка запрещенных отправителей не могут отправлять записи в беседы группы (определенные в URL-адресе запроса GET). Убедитесь, что в списках запрещенных и разрешенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="ccba3-p101">Users in the rejected senders list cannot post to conversations of the group (identified in the GET request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccba3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ccba3-107">Permissions</span></span>
<span data-ttu-id="ccba3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccba3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccba3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccba3-110">Permission type</span></span>      | <span data-ttu-id="ccba3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccba3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccba3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccba3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ccba3-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccba3-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ccba3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccba3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccba3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccba3-115">Not supported.</span></span>    |
|<span data-ttu-id="ccba3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccba3-116">Application</span></span> | <span data-ttu-id="ccba3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccba3-117">Not supported.</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="ccba3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccba3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/rejectedSenders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ccba3-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ccba3-119">Optional query parameters</span></span>
<span data-ttu-id="ccba3-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ccba3-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ccba3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccba3-121">Request headers</span></span>
| <span data-ttu-id="ccba3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ccba3-122">Header</span></span>       | <span data-ttu-id="ccba3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ccba3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ccba3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ccba3-124">Authorization</span></span>  | <span data-ttu-id="ccba3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccba3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ccba3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ccba3-127">Request body</span></span>
<span data-ttu-id="ccba3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ccba3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccba3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ccba3-129">Response</span></span>
<span data-ttu-id="ccba3-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ccba3-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccba3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ccba3-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ccba3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccba3-132">Request</span></span>
<span data-ttu-id="ccba3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccba3-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ccba3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccba3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rejectedsenders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ccba3-135">C#</span><span class="sxs-lookup"><span data-stu-id="ccba3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rejectedsenders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ccba3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccba3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rejectedsenders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ccba3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccba3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rejectedsenders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ccba3-138">Java</span><span class="sxs-lookup"><span data-stu-id="ccba3-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rejectedsenders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ccba3-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="ccba3-139">Response</span></span>
<span data-ttu-id="ccba3-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ccba3-140">The following is an example of the response.</span></span>
><span data-ttu-id="ccba3-141">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ccba3-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ccba3-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccba3-142">All the properties will be returned from an actual call.</span></span>
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
  "description": "List rejectedSenders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
