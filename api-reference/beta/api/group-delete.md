---
title: Удаление группы
description: Удаляет группу.
ms.openlocfilehash: 92a15366fefb6ab70c45f664daa28b75bcea5891
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077846"
---
# <a name="delete-group"></a><span data-ttu-id="546a1-103">Удаление группы</span><span class="sxs-lookup"><span data-stu-id="546a1-103">Delete group</span></span>

> <span data-ttu-id="546a1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="546a1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="546a1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="546a1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="546a1-106">Удаляет группу.</span><span class="sxs-lookup"><span data-stu-id="546a1-106">Deletes a group.</span></span>

<span data-ttu-id="546a1-107">При удалении группы элемент добавляется [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="546a1-107">When a group is deleted, the item is added to [deleted items](../resources/directory.md).</span></span> <span data-ttu-id="546a1-108">Группа будет храниться в удаленных элементов до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="546a1-108">The group will remain in deleted items for up to 30 days.</span></span> <span data-ttu-id="546a1-109">Группы могут быть полностью восстановлены из удаленных элементов во время в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="546a1-109">A group can be fully restored from deleted items during the 30 days.</span></span> <span data-ttu-id="546a1-110">Через 30 дней после удаленных элементов без возможности восстановления, удаляются.</span><span class="sxs-lookup"><span data-stu-id="546a1-110">After 30 days, deleted items are permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="546a1-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="546a1-111">Permissions</span></span>
<span data-ttu-id="546a1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="546a1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="546a1-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="546a1-114">Permission type</span></span>      | <span data-ttu-id="546a1-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="546a1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="546a1-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="546a1-116">Delegated (work or school account)</span></span> | <span data-ttu-id="546a1-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="546a1-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="546a1-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="546a1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="546a1-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="546a1-119">Not supported.</span></span>    |
|<span data-ttu-id="546a1-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="546a1-120">Application</span></span> | <span data-ttu-id="546a1-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="546a1-121">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="546a1-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="546a1-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="546a1-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="546a1-123">Request headers</span></span>
| <span data-ttu-id="546a1-124">Имя</span><span class="sxs-lookup"><span data-stu-id="546a1-124">Name</span></span>       | <span data-ttu-id="546a1-125">Тип</span><span class="sxs-lookup"><span data-stu-id="546a1-125">Type</span></span> | <span data-ttu-id="546a1-126">Описание</span><span class="sxs-lookup"><span data-stu-id="546a1-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="546a1-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="546a1-127">Authorization</span></span>  | <span data-ttu-id="546a1-128">string</span><span class="sxs-lookup"><span data-stu-id="546a1-128">string</span></span>  | <span data-ttu-id="546a1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="546a1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="546a1-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="546a1-131">Request body</span></span>
<span data-ttu-id="546a1-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="546a1-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="546a1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="546a1-133">Response</span></span>
<span data-ttu-id="546a1-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="546a1-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="546a1-136">Пример</span><span class="sxs-lookup"><span data-stu-id="546a1-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="546a1-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="546a1-137">Request</span></span>
<span data-ttu-id="546a1-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="546a1-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="546a1-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="546a1-139">Response</span></span>
<span data-ttu-id="546a1-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="546a1-140">The following is an example of the response.</span></span> 
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
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->