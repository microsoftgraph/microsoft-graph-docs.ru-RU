---
title: Создание беседы в чате
description: Создание новой беседы в чате указанного канала путем предоставления корневых сообщений.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: ef8d341310296c810c433a23f0d29be166ca47c5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511249"
---
# <a name="create-chat-thread"></a><span data-ttu-id="b649d-103">Создание беседы в чате</span><span class="sxs-lookup"><span data-stu-id="b649d-103">Create chat thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b649d-104">Создание новой беседы в чате указанного [канала](../resources/channel.md) путем предоставления корневых сообщений.</span><span class="sxs-lookup"><span data-stu-id="b649d-104">Create a new chat thread in the specified [channel](../resources/channel.md) by supplying the root messages.</span></span>

## <a name="permissions"></a><span data-ttu-id="b649d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b649d-105">Permissions</span></span>
<span data-ttu-id="b649d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b649d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b649d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b649d-108">Permission type</span></span>      | <span data-ttu-id="b649d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b649d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b649d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b649d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b649d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b649d-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b649d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b649d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b649d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b649d-113">Not supported.</span></span>    |
|<span data-ttu-id="b649d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b649d-114">Application</span></span> | <span data-ttu-id="b649d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b649d-115">Not supported.</span></span> |

> <span data-ttu-id="b649d-116">В настоящее время для этой операции поддерживаются только [делегированные разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b649d-116">Currently, only [delegated permissions](/graph/permissions-reference) are supported for this operation.</span></span>  <span data-ttu-id="b649d-117">В будущих выпусках будут поддерживаться разрешения для приложений.</span><span class="sxs-lookup"><span data-stu-id="b649d-117">Future releases will support application permissions.</span></span> 

## <a name="http-request"></a><span data-ttu-id="b649d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b649d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/chatThreads
```
## <a name="request-headers"></a><span data-ttu-id="b649d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b649d-119">Request headers</span></span>
| <span data-ttu-id="b649d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b649d-120">Name</span></span>       | <span data-ttu-id="b649d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="b649d-121">Type</span></span> | <span data-ttu-id="b649d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b649d-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b649d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b649d-123">Authorization</span></span>  | <span data-ttu-id="b649d-124">string</span><span class="sxs-lookup"><span data-stu-id="b649d-124">string</span></span>  | <span data-ttu-id="b649d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b649d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b649d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b649d-127">Request body</span></span>
<span data-ttu-id="b649d-128">В тексте запроса укажите представление в формате JSON объекта [chatThread](../resources/chatthread.md), который содержит свойство rootMessage.</span><span class="sxs-lookup"><span data-stu-id="b649d-128">In the request body, supply a JSON representation of a [chatThread](../resources/chatthread.md) object that contains the rootMessage property.</span></span>

## <a name="response"></a><span data-ttu-id="b649d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b649d-129">Response</span></span>

<span data-ttu-id="b649d-130">При успешном выполнении этот метод возвращает код отклика `201 Created` и пустой текст отклика.</span><span class="sxs-lookup"><span data-stu-id="b649d-130">If successful, this method returns a `201 Created` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="b649d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b649d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b649d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b649d-132">Request</span></span>
<span data-ttu-id="b649d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b649d-133">Here is an example of the request.</span></span>
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

> <span data-ttu-id="b649d-134">В настоящее время contentType должен быть указан в виде целого числа, а не строки: 0 для текста или 1 для html.</span><span class="sxs-lookup"><span data-stu-id="b649d-134">Currently, the contentType must be specified as an integer rather than a string: 0 for "text" or 1 for "html".</span></span>  <span data-ttu-id="b649d-135">Это будет исправлено в будущих выпусках API.</span><span class="sxs-lookup"><span data-stu-id="b649d-135">Future API releases will fix this.</span></span>

##### <a name="response"></a><span data-ttu-id="b649d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b649d-136">Response</span></span>

<span data-ttu-id="b649d-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b649d-137">Here is an example of the response.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-post-chatthreads.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
