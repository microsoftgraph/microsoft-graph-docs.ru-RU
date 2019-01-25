---
title: Создание объекта Message
description: С помощью этого API можно создать экземпляр Message в mailfolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 868f6e9b753296f6828ec1537eb04ca232c1991e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514931"
---
# <a name="create-message"></a><span data-ttu-id="27123-103">Создание объекта Message</span><span class="sxs-lookup"><span data-stu-id="27123-103">Create Message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27123-104">С помощью этого API можно создать экземпляр Message в mailfolder.</span><span class="sxs-lookup"><span data-stu-id="27123-104">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="27123-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27123-105">Permissions</span></span>
<span data-ttu-id="27123-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27123-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27123-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27123-108">Permission type</span></span>      | <span data-ttu-id="27123-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27123-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27123-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27123-110">Delegated (work or school account)</span></span> | <span data-ttu-id="27123-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27123-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="27123-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27123-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27123-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27123-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="27123-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27123-114">Application</span></span> | <span data-ttu-id="27123-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27123-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="27123-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27123-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="27123-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27123-117">Request headers</span></span>
| <span data-ttu-id="27123-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="27123-118">Header</span></span>       | <span data-ttu-id="27123-119">Значение</span><span class="sxs-lookup"><span data-stu-id="27123-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="27123-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27123-120">Authorization</span></span>  | <span data-ttu-id="27123-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27123-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="27123-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27123-123">Content-Type</span></span>  | <span data-ttu-id="27123-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27123-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="27123-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27123-126">Request body</span></span>
<span data-ttu-id="27123-127">Предоставьте в тексте запроса описание объекта [Message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27123-127">In the request body, supply a JSON representation of [Message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="27123-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="27123-128">Response</span></span>

<span data-ttu-id="27123-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="27123-129">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27123-130">Пример</span><span class="sxs-lookup"><span data-stu-id="27123-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27123-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="27123-131">Request</span></span>
<span data-ttu-id="27123-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27123-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="27123-133">Предоставьте в тексте запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27123-133">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="27123-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="27123-134">Response</span></span>
<span data-ttu-id="27123-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="27123-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-post-messages.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
