---
title: 'message: send'
description: Отправьте сообщение в папке «Черновики». Черновик сообщения могут быть новый черновик сообщения, ответ черновиков, ответить всем черновиков или
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 5e7689e2b0bdd07c1739b4d3f640eb71b8dd0a35
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516597"
---
# <a name="message-send"></a><span data-ttu-id="9fc25-104">message: send</span><span class="sxs-lookup"><span data-stu-id="9fc25-104">message: send</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fc25-p102">Отправка сообщения из папки черновиков. Черновик сообщения может быть предназначен для нового сообщения, ответа, ответа всем пользователям или пересылки. Затем сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="9fc25-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fc25-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9fc25-108">Permissions</span></span>

<span data-ttu-id="9fc25-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fc25-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fc25-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9fc25-111">Permission type</span></span>      | <span data-ttu-id="9fc25-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9fc25-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fc25-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fc25-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9fc25-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9fc25-114">Mail.Send</span></span>    |
|<span data-ttu-id="9fc25-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fc25-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fc25-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9fc25-116">Mail.Send</span></span>    |
|<span data-ttu-id="9fc25-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9fc25-117">Application</span></span> | <span data-ttu-id="9fc25-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9fc25-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fc25-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fc25-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="9fc25-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9fc25-120">Request headers</span></span>

| <span data-ttu-id="9fc25-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9fc25-121">Name</span></span>       | <span data-ttu-id="9fc25-122">Тип</span><span class="sxs-lookup"><span data-stu-id="9fc25-122">Type</span></span> | <span data-ttu-id="9fc25-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9fc25-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9fc25-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fc25-124">Authorization</span></span>  | <span data-ttu-id="9fc25-125">string</span><span class="sxs-lookup"><span data-stu-id="9fc25-125">string</span></span>  | <span data-ttu-id="9fc25-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fc25-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9fc25-128">Content-Length</span><span class="sxs-lookup"><span data-stu-id="9fc25-128">Content-Length</span></span> | <span data-ttu-id="9fc25-129">число</span><span class="sxs-lookup"><span data-stu-id="9fc25-129">number</span></span> | <span data-ttu-id="9fc25-130">0. требуется.</span><span class="sxs-lookup"><span data-stu-id="9fc25-130">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9fc25-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9fc25-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9fc25-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fc25-132">Response</span></span>

<span data-ttu-id="9fc25-p105">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9fc25-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fc25-135">Пример</span><span class="sxs-lookup"><span data-stu-id="9fc25-135">Example</span></span>

<span data-ttu-id="9fc25-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9fc25-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9fc25-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fc25-137">Request</span></span>

<span data-ttu-id="9fc25-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fc25-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="9fc25-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="9fc25-139">Response</span></span>

<span data-ttu-id="9fc25-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9fc25-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-send.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
