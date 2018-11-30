---
title: Создать поток разговора
description: Создайте новый поток чата в указанном канала, передав корневой сообщения.
ms.openlocfilehash: 9a2a35a086c6689d1b76a56b70cd3637ec23c3a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075020"
---
# <a name="create-chat-thread"></a><span data-ttu-id="53b89-103">Создать поток разговора</span><span class="sxs-lookup"><span data-stu-id="53b89-103">Create chat thread</span></span>

> <span data-ttu-id="53b89-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="53b89-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53b89-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53b89-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="53b89-106">Создание нового потока чата в указанном [канала](../resources/channel.md) , передав корневой сообщения.</span><span class="sxs-lookup"><span data-stu-id="53b89-106">Create a new chat thread in the specified [channel](../resources/channel.md) by supplying the root messages.</span></span>

## <a name="permissions"></a><span data-ttu-id="53b89-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53b89-107">Permissions</span></span>
<span data-ttu-id="53b89-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53b89-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53b89-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53b89-110">Permission type</span></span>      | <span data-ttu-id="53b89-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53b89-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53b89-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53b89-112">Delegated (work or school account)</span></span> | <span data-ttu-id="53b89-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53b89-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="53b89-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53b89-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53b89-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53b89-115">Not supported.</span></span>    |
|<span data-ttu-id="53b89-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53b89-116">Application</span></span> | <span data-ttu-id="53b89-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53b89-117">Not supported.</span></span> |

> <span data-ttu-id="53b89-118">На данный момент только [делегированных разрешений](/graph/permissions-reference) поддерживаются для этой операции.</span><span class="sxs-lookup"><span data-stu-id="53b89-118">Currently, only [delegated permissions](/graph/permissions-reference) are supported for this operation.</span></span>  <span data-ttu-id="53b89-119">Будущих выпусках обеспечения разрешения приложения.</span><span class="sxs-lookup"><span data-stu-id="53b89-119">Future releases will support application permissions.</span></span> 

## <a name="http-request"></a><span data-ttu-id="53b89-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53b89-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/chatThreads
```
## <a name="request-headers"></a><span data-ttu-id="53b89-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53b89-121">Request headers</span></span>
| <span data-ttu-id="53b89-122">Имя</span><span class="sxs-lookup"><span data-stu-id="53b89-122">Name</span></span>       | <span data-ttu-id="53b89-123">Тип</span><span class="sxs-lookup"><span data-stu-id="53b89-123">Type</span></span> | <span data-ttu-id="53b89-124">Описание</span><span class="sxs-lookup"><span data-stu-id="53b89-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="53b89-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="53b89-125">Authorization</span></span>  | <span data-ttu-id="53b89-126">string</span><span class="sxs-lookup"><span data-stu-id="53b89-126">string</span></span>  | <span data-ttu-id="53b89-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53b89-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53b89-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53b89-129">Request body</span></span>
<span data-ttu-id="53b89-130">В тексте запроса укажите представление JSON объекта [chatThread](../resources/chatthread.md) , который содержит свойство rootMessage.</span><span class="sxs-lookup"><span data-stu-id="53b89-130">In the request body, supply a JSON representation of a [chatThread](../resources/chatthread.md) object that contains the rootMessage property.</span></span>

## <a name="response"></a><span data-ttu-id="53b89-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="53b89-131">Response</span></span>

<span data-ttu-id="53b89-132">Успешно завершена, этот метод возвращает `201 Created` код ответа с помощью тело пустой ответа.</span><span class="sxs-lookup"><span data-stu-id="53b89-132">If successful, this method returns `201 Created` response code with an empty reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="53b89-133">Пример</span><span class="sxs-lookup"><span data-stu-id="53b89-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53b89-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="53b89-134">Request</span></span>
<span data-ttu-id="53b89-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53b89-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_chatthread_from_channel"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/chatThreads
Content-type: application/json

{
  "rootMessage": {
      "body": {
        "contentType": 1,
        "content": "<h1>Hello world</h1>"
      }
  }
}
```

> <span data-ttu-id="53b89-136">На данный момент contentType должно быть указано как целое число, а не строкой: 0 для 1 для «html» или «text».</span><span class="sxs-lookup"><span data-stu-id="53b89-136">Currently, the contentType must be specified as an integer rather than a string: 0 for "text" or 1 for "html".</span></span>  <span data-ttu-id="53b89-137">Это будет исправить будущих выпусках API.</span><span class="sxs-lookup"><span data-stu-id="53b89-137">Future API releases will fix this.</span></span>

##### <a name="response"></a><span data-ttu-id="53b89-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="53b89-138">Response</span></span>

<span data-ttu-id="53b89-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="53b89-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
