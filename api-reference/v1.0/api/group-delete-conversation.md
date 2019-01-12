---
title: Удаление беседы
description: Удаление объекта conversation.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f470fb1ed55237e968b0277f30a67f4c212b1493
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954969"
---
# <a name="delete-conversation"></a><span data-ttu-id="e5c17-103">Удаление беседы</span><span class="sxs-lookup"><span data-stu-id="e5c17-103">Delete conversation</span></span>
<span data-ttu-id="e5c17-104">Удаление объекта [conversation](../resources/conversation.md).</span><span class="sxs-lookup"><span data-stu-id="e5c17-104">Delete a [conversation](../resources/conversation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5c17-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5c17-105">Permissions</span></span>
<span data-ttu-id="e5c17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5c17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5c17-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5c17-108">Permission type</span></span>      | <span data-ttu-id="e5c17-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5c17-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5c17-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5c17-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e5c17-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5c17-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e5c17-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5c17-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5c17-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5c17-113">Not supported.</span></span>    |
|<span data-ttu-id="e5c17-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5c17-114">Application</span></span> | <span data-ttu-id="e5c17-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5c17-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5c17-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5c17-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e5c17-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5c17-117">Request headers</span></span>
| <span data-ttu-id="e5c17-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e5c17-118">Name</span></span>       | <span data-ttu-id="e5c17-119">Тип</span><span class="sxs-lookup"><span data-stu-id="e5c17-119">Type</span></span> | <span data-ttu-id="e5c17-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e5c17-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e5c17-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5c17-121">Authorization</span></span>  | <span data-ttu-id="e5c17-122">string</span><span class="sxs-lookup"><span data-stu-id="e5c17-122">string</span></span>  | <span data-ttu-id="e5c17-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5c17-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5c17-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e5c17-125">Request body</span></span>
<span data-ttu-id="e5c17-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5c17-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5c17-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5c17-127">Response</span></span>
<span data-ttu-id="e5c17-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e5c17-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5c17-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e5c17-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e5c17-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5c17-131">Request</span></span>
<span data-ttu-id="e5c17-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5c17-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU="],
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="e5c17-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5c17-133">Response</span></span>
<span data-ttu-id="e5c17-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e5c17-134">The following is an example of the response.</span></span> 
><span data-ttu-id="e5c17-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5c17-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
