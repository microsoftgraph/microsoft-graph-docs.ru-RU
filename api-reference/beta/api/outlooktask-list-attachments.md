---
title: Список вложений
description: Получите список объектов вложения, подключенного к задачи Outlook.
author: angelgolfer-ms
ms.openlocfilehash: b998f6f7d3356728400cc7c609dd1014467ae4d6
ms.sourcegitcommit: 6b1ba9b3be038cd6247de54a255bad560034fe42
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2019
ms.locfileid: "27771795"
---
# <a name="list-attachments"></a><span data-ttu-id="171c7-103">Список вложений</span><span class="sxs-lookup"><span data-stu-id="171c7-103">List attachments</span></span>

> <span data-ttu-id="171c7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="171c7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="171c7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="171c7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="171c7-106">Получите список объектов [вложения](../resources/attachment.md) , подключенного к задачи Outlook.</span><span class="sxs-lookup"><span data-stu-id="171c7-106">Get a list of [attachment](../resources/attachment.md) objects attached to an Outlook task.</span></span>

## <a name="permissions"></a><span data-ttu-id="171c7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="171c7-107">Permissions</span></span>

<span data-ttu-id="171c7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="171c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="171c7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="171c7-110">Permission type</span></span>      | <span data-ttu-id="171c7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="171c7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="171c7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="171c7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="171c7-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="171c7-113">Tasks.Read</span></span>    |
|<span data-ttu-id="171c7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="171c7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="171c7-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="171c7-115">Tasks.Read</span></span>    |
|<span data-ttu-id="171c7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="171c7-116">Application</span></span> | <span data-ttu-id="171c7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="171c7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="171c7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="171c7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments
GET /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="171c7-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="171c7-119">Optional query parameters</span></span>

<span data-ttu-id="171c7-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="171c7-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="171c7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="171c7-121">Request headers</span></span>

| <span data-ttu-id="171c7-122">Имя</span><span class="sxs-lookup"><span data-stu-id="171c7-122">Name</span></span>      |<span data-ttu-id="171c7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="171c7-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="171c7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="171c7-124">Authorization</span></span>  | <span data-ttu-id="171c7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="171c7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="171c7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="171c7-127">Request body</span></span>

<span data-ttu-id="171c7-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="171c7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="171c7-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="171c7-129">Response</span></span>

<span data-ttu-id="171c7-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [вложения](../resources/attachment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="171c7-130">If successful, this method returns a `200 OK` response code and collection of [attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="171c7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="171c7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="171c7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="171c7-132">Request</span></span>

<span data-ttu-id="171c7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="171c7-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
```

### <a name="response"></a><span data-ttu-id="171c7-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="171c7-134">Response</span></span>

<span data-ttu-id="171c7-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="171c7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->