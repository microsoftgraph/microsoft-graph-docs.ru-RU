---
title: Список вложений
description: Получение списка объектов вложений.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 7799c0d5adffca64e56c10e9ea49b5d5944bc6eb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815885"
---
# <a name="list-attachments"></a><span data-ttu-id="1a3da-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="1a3da-103">List attachments</span></span>

<span data-ttu-id="1a3da-104">Получение списка объектов вложений.</span><span class="sxs-lookup"><span data-stu-id="1a3da-104">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="1a3da-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a3da-105">Permissions</span></span>
<span data-ttu-id="1a3da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a3da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a3da-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a3da-108">Permission type</span></span>      | <span data-ttu-id="1a3da-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a3da-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a3da-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a3da-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1a3da-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1a3da-111">Mail.Read</span></span>    |
|<span data-ttu-id="1a3da-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a3da-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a3da-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1a3da-113">Mail.Read</span></span>    |
|<span data-ttu-id="1a3da-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a3da-114">Application</span></span> | <span data-ttu-id="1a3da-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1a3da-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a3da-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a3da-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1a3da-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1a3da-117">Optional query parameters</span></span>
<span data-ttu-id="1a3da-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1a3da-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a3da-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a3da-119">Request headers</span></span>
| <span data-ttu-id="1a3da-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1a3da-120">Name</span></span>       | <span data-ttu-id="1a3da-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1a3da-121">Type</span></span> | <span data-ttu-id="1a3da-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1a3da-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1a3da-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a3da-123">Authorization</span></span>  | <span data-ttu-id="1a3da-124">string</span><span class="sxs-lookup"><span data-stu-id="1a3da-124">string</span></span>  | <span data-ttu-id="1a3da-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a3da-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a3da-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1a3da-127">Request body</span></span>
<span data-ttu-id="1a3da-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1a3da-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a3da-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a3da-129">Response</span></span>

<span data-ttu-id="1a3da-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1a3da-130">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1a3da-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1a3da-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a3da-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a3da-132">Request</span></span>
<span data-ttu-id="1a3da-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a3da-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="1a3da-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="1a3da-134">Response</span></span>
<span data-ttu-id="1a3da-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1a3da-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attachment)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "microsoft.graph.fileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "base64-contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
