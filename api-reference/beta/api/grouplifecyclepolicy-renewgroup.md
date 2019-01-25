---
title: 'groupLifecyclePolicy: renewGroup'
description: Обновляет срок действия группы. Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 7eb0ef44a5e07c8c293ba804cc8ec31a8312576d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520874"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="e2d26-104">groupLifecyclePolicy: renewGroup</span><span class="sxs-lookup"><span data-stu-id="e2d26-104">groupLifecyclePolicy: renewGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2d26-105">Обновляет срок действия группы.</span><span class="sxs-lookup"><span data-stu-id="e2d26-105">Renews a group's expiration.</span></span> <span data-ttu-id="e2d26-106">Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.</span><span class="sxs-lookup"><span data-stu-id="e2d26-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="e2d26-107">**Примечание:** В версии 1.0, [Используйте группы ресурсов следует обновить запросы](/graph/api/group-renew?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="e2d26-107">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="e2d26-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e2d26-108">Permissions</span></span>

<span data-ttu-id="e2d26-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2d26-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="e2d26-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2d26-111">Permission type</span></span>      | <span data-ttu-id="e2d26-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2d26-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2d26-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2d26-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e2d26-114">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2d26-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="e2d26-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2d26-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2d26-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e2d26-116">Not supported</span></span> |
|<span data-ttu-id="e2d26-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="e2d26-117">Application</span></span> | <span data-ttu-id="e2d26-118">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2d26-118">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2d26-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2d26-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="e2d26-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2d26-120">Request headers</span></span>

| <span data-ttu-id="e2d26-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e2d26-121">Name</span></span> | <span data-ttu-id="e2d26-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e2d26-122">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e2d26-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2d26-123">Authorization</span></span> | <span data-ttu-id="e2d26-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2d26-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e2d26-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e2d26-126">Content-Type</span></span>  | <span data-ttu-id="e2d26-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e2d26-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2d26-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2d26-128">Request body</span></span>
<span data-ttu-id="e2d26-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e2d26-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e2d26-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="e2d26-130">Parameter</span></span> | <span data-ttu-id="e2d26-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e2d26-131">Type</span></span> | <span data-ttu-id="e2d26-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e2d26-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e2d26-133">groupId</span><span class="sxs-lookup"><span data-stu-id="e2d26-133">groupId</span></span>|<span data-ttu-id="e2d26-134">GUID</span><span class="sxs-lookup"><span data-stu-id="e2d26-134">Guid</span></span>| <span data-ttu-id="e2d26-135">Идентификатор группы для обновления.</span><span class="sxs-lookup"><span data-stu-id="e2d26-135">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="e2d26-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2d26-136">Response</span></span>

<span data-ttu-id="e2d26-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e2d26-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2d26-139">Пример</span><span class="sxs-lookup"><span data-stu-id="e2d26-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e2d26-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2d26-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "grouplifecyclepolicy_renewgroup"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/renewGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a><span data-ttu-id="e2d26-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="e2d26-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: renewgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-renewgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
