---
title: Список вложений
description: Получите список объектов вложений, присоединенных к Outlook задаче.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 87b7a341be4e280a8b211bf03e814006d8240755
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055479"
---
# <a name="list-attachments-deprecated"></a><span data-ttu-id="a4307-103">Вложения списка (неподготовленные)</span><span class="sxs-lookup"><span data-stu-id="a4307-103">List attachments (deprecated)</span></span>

<span data-ttu-id="a4307-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4307-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="a4307-105">Получите список объектов [вложений,](../resources/attachment.md) присоединенных к Outlook задачи.</span><span class="sxs-lookup"><span data-stu-id="a4307-105">Get a list of [attachment](../resources/attachment.md) objects attached to an Outlook task.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4307-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4307-106">Permissions</span></span>

<span data-ttu-id="a4307-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4307-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4307-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4307-109">Permission type</span></span>      | <span data-ttu-id="a4307-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4307-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4307-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4307-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a4307-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="a4307-112">Tasks.Read</span></span>    |
|<span data-ttu-id="a4307-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4307-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4307-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="a4307-114">Tasks.Read</span></span>    |
|<span data-ttu-id="a4307-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4307-115">Application</span></span> | <span data-ttu-id="a4307-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4307-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4307-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4307-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments
GET /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a4307-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a4307-118">Optional query parameters</span></span>

<span data-ttu-id="a4307-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a4307-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4307-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4307-120">Request headers</span></span>

| <span data-ttu-id="a4307-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a4307-121">Name</span></span>      |<span data-ttu-id="a4307-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a4307-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a4307-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4307-123">Authorization</span></span>  | <span data-ttu-id="a4307-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4307-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4307-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4307-126">Request body</span></span>

<span data-ttu-id="a4307-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a4307-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4307-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4307-128">Response</span></span>

<span data-ttu-id="a4307-129">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` вложений в [](../resources/attachment.md) тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a4307-129">If successful, this method returns a `200 OK` response code and collection of [attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4307-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a4307-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4307-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4307-131">Request</span></span>

<span data-ttu-id="a4307-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4307-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a4307-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4307-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "outlook_task_get_attachments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
```
# <a name="c"></a>[<span data-ttu-id="a4307-134">C#</span><span class="sxs-lookup"><span data-stu-id="a4307-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/outlook-task-get-attachments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4307-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4307-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/outlook-task-get-attachments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4307-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4307-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/outlook-task-get-attachments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4307-137">Java</span><span class="sxs-lookup"><span data-stu-id="a4307-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/outlook-task-get-attachments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a4307-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4307-138">Response</span></span>

<span data-ttu-id="a4307-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a4307-139">Here is an example of the response.</span></span> <span data-ttu-id="a4307-140">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a4307-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "lastModifiedDateTime": "datetime-value",
      "name": "name-value",
      "contentType": "contentType-value",
      "size": 99,
      "isInline": true,
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
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
