---
title: Список сообщений
description: Получение всех сообщений в почтовом ящике вошедшего пользователя или в указанной папке этого почтового ящика.
localization_priority: Priority
ms.openlocfilehash: a58d6e3c51cf85992129b3ba9c8e3996fa9841f8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825370"
---
# <a name="list-messages"></a><span data-ttu-id="be938-103">Список сообщений</span><span class="sxs-lookup"><span data-stu-id="be938-103">List messages</span></span>

<span data-ttu-id="be938-104">Получение всех сообщений в почтовом ящике вошедшего пользователя или в указанной папке этого почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="be938-104">Get all the messages in the signed-in user's mailbox, or those messages in a specified folder in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="be938-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be938-105">Permissions</span></span>
<span data-ttu-id="be938-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be938-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be938-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be938-108">Permission type</span></span>      | <span data-ttu-id="be938-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be938-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be938-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be938-110">Delegated (work or school account)</span></span> | <span data-ttu-id="be938-111">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be938-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="be938-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be938-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be938-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be938-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="be938-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be938-114">Application</span></span> | <span data-ttu-id="be938-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be938-115">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="be938-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be938-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="optional-query-parameters"></a><span data-ttu-id="be938-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="be938-117">Optional query parameters</span></span>
<span data-ttu-id="be938-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="be938-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="be938-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be938-119">Request headers</span></span>
| <span data-ttu-id="be938-120">Имя</span><span class="sxs-lookup"><span data-stu-id="be938-120">Name</span></span>       | <span data-ttu-id="be938-121">Тип</span><span class="sxs-lookup"><span data-stu-id="be938-121">Type</span></span> | <span data-ttu-id="be938-122">Описание</span><span class="sxs-lookup"><span data-stu-id="be938-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="be938-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="be938-123">Authorization</span></span>  | <span data-ttu-id="be938-124">string</span><span class="sxs-lookup"><span data-stu-id="be938-124">string</span></span>  | <span data-ttu-id="be938-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be938-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be938-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="be938-127">Request body</span></span>
<span data-ttu-id="be938-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be938-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be938-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="be938-129">Response</span></span>

<span data-ttu-id="be938-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="be938-130">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="be938-131">Пример</span><span class="sxs-lookup"><span data-stu-id="be938-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be938-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="be938-132">Request</span></span>
<span data-ttu-id="be938-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be938-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
```
##### <a name="response"></a><span data-ttu-id="be938-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="be938-134">Response</span></span>
<span data-ttu-id="be938-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="be938-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
