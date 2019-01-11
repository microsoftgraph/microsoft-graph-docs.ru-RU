---
title: Создание объекта Message
description: С помощью этого API можно создать экземпляр Message в mailfolder.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 3d4bd1783d5ad2e04f99e1e3d3231a0aa9bd31fb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878955"
---
# <a name="create-message"></a><span data-ttu-id="fbcc2-103">Создание объекта Message</span><span class="sxs-lookup"><span data-stu-id="fbcc2-103">Create Message</span></span>

> <span data-ttu-id="fbcc2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fbcc2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbcc2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbcc2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fbcc2-106">С помощью этого API можно создать экземпляр Message в mailfolder.</span><span class="sxs-lookup"><span data-stu-id="fbcc2-106">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="fbcc2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fbcc2-107">Permissions</span></span>
<span data-ttu-id="fbcc2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbcc2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbcc2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbcc2-110">Permission type</span></span>      | <span data-ttu-id="fbcc2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbcc2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbcc2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbcc2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fbcc2-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fbcc2-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fbcc2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbcc2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbcc2-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fbcc2-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fbcc2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fbcc2-116">Application</span></span> | <span data-ttu-id="fbcc2-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fbcc2-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbcc2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbcc2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="fbcc2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fbcc2-119">Request headers</span></span>
| <span data-ttu-id="fbcc2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fbcc2-120">Header</span></span>       | <span data-ttu-id="fbcc2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fbcc2-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fbcc2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fbcc2-122">Authorization</span></span>  | <span data-ttu-id="fbcc2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbcc2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fbcc2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fbcc2-125">Content-Type</span></span>  | <span data-ttu-id="fbcc2-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbcc2-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fbcc2-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fbcc2-128">Request body</span></span>
<span data-ttu-id="fbcc2-129">Предоставьте в тексте запроса описание объекта [Message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbcc2-129">In the request body, supply a JSON representation of [Message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fbcc2-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbcc2-130">Response</span></span>

<span data-ttu-id="fbcc2-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fbcc2-131">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbcc2-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fbcc2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fbcc2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbcc2-133">Request</span></span>
<span data-ttu-id="fbcc2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbcc2-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/messages
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```
<span data-ttu-id="fbcc2-135">Предоставьте в тексте запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbcc2-135">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fbcc2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbcc2-136">Response</span></span>
<span data-ttu-id="fbcc2-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fbcc2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
