---
title: Удаление группы
description: Удаляет группу.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 349900cffa4b0df1763e1ed8b8213ce81ec27351
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529966"
---
# <a name="delete-group"></a><span data-ttu-id="238bb-103">Удаление группы</span><span class="sxs-lookup"><span data-stu-id="238bb-103">Delete group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="238bb-104">Удаляет группу.</span><span class="sxs-lookup"><span data-stu-id="238bb-104">Deletes a group.</span></span>

<span data-ttu-id="238bb-105">При удалении группы элемент добавляется [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="238bb-105">When a group is deleted, the item is added to [deleted items](../resources/directory.md).</span></span> <span data-ttu-id="238bb-106">Группа будет храниться в удаленных элементов до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="238bb-106">The group will remain in deleted items for up to 30 days.</span></span> <span data-ttu-id="238bb-107">Группы могут быть полностью восстановлены из удаленных элементов во время в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="238bb-107">A group can be fully restored from deleted items during the 30 days.</span></span> <span data-ttu-id="238bb-108">Через 30 дней после удаленных элементов без возможности восстановления, удаляются.</span><span class="sxs-lookup"><span data-stu-id="238bb-108">After 30 days, deleted items are permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="238bb-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="238bb-109">Permissions</span></span>
<span data-ttu-id="238bb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="238bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="238bb-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="238bb-112">Permission type</span></span>      | <span data-ttu-id="238bb-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="238bb-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="238bb-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="238bb-114">Delegated (work or school account)</span></span> | <span data-ttu-id="238bb-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="238bb-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="238bb-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="238bb-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="238bb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="238bb-117">Not supported.</span></span>    |
|<span data-ttu-id="238bb-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="238bb-118">Application</span></span> | <span data-ttu-id="238bb-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="238bb-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="238bb-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="238bb-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="238bb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="238bb-121">Request headers</span></span>
| <span data-ttu-id="238bb-122">Имя</span><span class="sxs-lookup"><span data-stu-id="238bb-122">Name</span></span>       | <span data-ttu-id="238bb-123">Тип</span><span class="sxs-lookup"><span data-stu-id="238bb-123">Type</span></span> | <span data-ttu-id="238bb-124">Описание</span><span class="sxs-lookup"><span data-stu-id="238bb-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="238bb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="238bb-125">Authorization</span></span>  | <span data-ttu-id="238bb-126">string</span><span class="sxs-lookup"><span data-stu-id="238bb-126">string</span></span>  | <span data-ttu-id="238bb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="238bb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="238bb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="238bb-129">Request body</span></span>
<span data-ttu-id="238bb-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="238bb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="238bb-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="238bb-131">Response</span></span>
<span data-ttu-id="238bb-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="238bb-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="238bb-134">Пример</span><span class="sxs-lookup"><span data-stu-id="238bb-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="238bb-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="238bb-135">Request</span></span>
<span data-ttu-id="238bb-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="238bb-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="238bb-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="238bb-137">Response</span></span>
<span data-ttu-id="238bb-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="238bb-138">The following is an example of the response.</span></span> 
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
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
