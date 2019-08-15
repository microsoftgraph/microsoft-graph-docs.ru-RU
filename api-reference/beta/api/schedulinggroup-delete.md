---
title: Удаление объекта schedulingGroup
description: Пометка элемента Счедулингграуп как неактивного путем задания его свойства "свойство Active"
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a36cbbacc931f6bd00b7aa8f228429943ddad712
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410677"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="28956-103">Удаление объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="28956-103">Delete schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28956-104">Помечайте [счедулингграуп](../resources/schedulinggroup.md) как неактивную \*\*\*\* , устанавливая его свойство GetProperty.</span><span class="sxs-lookup"><span data-stu-id="28956-104">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="28956-105">Этот метод не удаляет [счедулингграуп](../resources/schedulinggroup.md) из расписания.</span><span class="sxs-lookup"><span data-stu-id="28956-105">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="28956-106">Существующие [сменные](../resources/shift.md) экземпляры, назначенные группе планирования, не входят в группу.</span><span class="sxs-lookup"><span data-stu-id="28956-106">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="28956-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28956-107">Permissions</span></span>

<span data-ttu-id="28956-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28956-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28956-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28956-110">Permission type</span></span>      | <span data-ttu-id="28956-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28956-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28956-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28956-112">Delegated (work or school account)</span></span> | <span data-ttu-id="28956-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28956-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="28956-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28956-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28956-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28956-115">Not supported.</span></span>    |
|<span data-ttu-id="28956-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28956-116">Application</span></span> | <span data-ttu-id="28956-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28956-117">Not supported.</span></span> |

> <span data-ttu-id="28956-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="28956-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="28956-119">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="28956-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="28956-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28956-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="28956-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28956-121">Request headers</span></span>

| <span data-ttu-id="28956-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28956-122">Header</span></span>       | <span data-ttu-id="28956-123">Значение</span><span class="sxs-lookup"><span data-stu-id="28956-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="28956-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28956-124">Authorization</span></span>  | <span data-ttu-id="28956-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28956-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="28956-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="28956-127">Content-Type</span></span>  | <span data-ttu-id="28956-128">application/json</span><span class="sxs-lookup"><span data-stu-id="28956-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="28956-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="28956-129">Request body</span></span>
<span data-ttu-id="28956-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28956-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28956-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="28956-131">Response</span></span>

<span data-ttu-id="28956-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="28956-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28956-134">Пример</span><span class="sxs-lookup"><span data-stu-id="28956-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="28956-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="28956-135">Request</span></span>

<span data-ttu-id="28956-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28956-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="28956-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="28956-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="28956-138">C#</span><span class="sxs-lookup"><span data-stu-id="28956-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-delete-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="28956-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28956-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-delete-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="28956-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="28956-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-delete-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="28956-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="28956-141">Response</span></span>

<span data-ttu-id="28956-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="28956-142">The following is an example of the response.</span></span> 

><span data-ttu-id="28956-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28956-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Marks a schedulingGroup as inactive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
