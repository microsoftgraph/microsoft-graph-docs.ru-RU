---
title: Удаление цепочки беседы
description: Удаление объекта thread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: c852e6e292980eb60c753a727a1daf2dd0316459
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526041"
---
# <a name="delete-conversation-thread"></a><span data-ttu-id="c109a-103">Удаление цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="c109a-103">Delete conversation thread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c109a-104">Удаление объекта [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="c109a-104">Delete a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c109a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c109a-105">Permissions</span></span>
<span data-ttu-id="c109a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c109a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c109a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c109a-108">Permission type</span></span>      | <span data-ttu-id="c109a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c109a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c109a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c109a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c109a-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c109a-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c109a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c109a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c109a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c109a-113">Not supported.</span></span>    |
|<span data-ttu-id="c109a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c109a-114">Application</span></span> | <span data-ttu-id="c109a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c109a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c109a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c109a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c109a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c109a-117">Request headers</span></span>
| <span data-ttu-id="c109a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c109a-118">Name</span></span>       | <span data-ttu-id="c109a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c109a-119">Type</span></span> | <span data-ttu-id="c109a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c109a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c109a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c109a-121">Authorization</span></span>  | <span data-ttu-id="c109a-122">string</span><span class="sxs-lookup"><span data-stu-id="c109a-122">string</span></span>  | <span data-ttu-id="c109a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c109a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c109a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c109a-125">Request body</span></span>
<span data-ttu-id="c109a-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c109a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c109a-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="c109a-127">Response</span></span>
<span data-ttu-id="c109a-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c109a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c109a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c109a-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c109a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c109a-131">Request</span></span>
<span data-ttu-id="c109a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c109a-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_thread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="c109a-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="c109a-133">Response</span></span>
<span data-ttu-id="c109a-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c109a-134">The following is an example of the response.</span></span> 
><span data-ttu-id="c109a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c109a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete-thread.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
