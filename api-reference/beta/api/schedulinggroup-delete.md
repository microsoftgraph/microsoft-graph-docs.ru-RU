---
title: Удаление объекта schedulingGroup
description: Пометка элемента Счедулингграуп как неактивного путем задания его свойства "свойство Active"
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 04a5ffce59f56f17f749c9cc69ff34e7d401c6fd
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263996"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="f0ecf-103">Удаление объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="f0ecf-103">Delete schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0ecf-104">Помечайте [счедулингграуп](../resources/schedulinggroup.md) как неактивную \*\*\*\* , устанавливая его свойство GetProperty.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-104">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="f0ecf-105">Этот метод не удаляет [счедулингграуп](../resources/schedulinggroup.md) из расписания.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-105">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="f0ecf-106">Существующие [сменные](../resources/shift.md) экземпляры, назначенные группе планирования, не входят в группу.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-106">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0ecf-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f0ecf-107">Permissions</span></span>

<span data-ttu-id="f0ecf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0ecf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0ecf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0ecf-110">Permission type</span></span>      | <span data-ttu-id="f0ecf-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0ecf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0ecf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0ecf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f0ecf-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0ecf-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f0ecf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0ecf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0ecf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-115">Not supported.</span></span>    |
|<span data-ttu-id="f0ecf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0ecf-116">Application</span></span> | <span data-ttu-id="f0ecf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-117">Not supported.</span></span> |

> <span data-ttu-id="f0ecf-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f0ecf-119">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f0ecf-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0ecf-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="f0ecf-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0ecf-121">Request headers</span></span>

| <span data-ttu-id="f0ecf-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0ecf-122">Header</span></span>       | <span data-ttu-id="f0ecf-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f0ecf-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f0ecf-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0ecf-124">Authorization</span></span>  | <span data-ttu-id="f0ecf-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f0ecf-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f0ecf-127">Content-Type</span></span>  | <span data-ttu-id="f0ecf-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f0ecf-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f0ecf-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f0ecf-129">Request body</span></span>
<span data-ttu-id="f0ecf-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0ecf-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0ecf-131">Response</span></span>

<span data-ttu-id="f0ecf-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0ecf-134">Пример</span><span class="sxs-lookup"><span data-stu-id="f0ecf-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f0ecf-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0ecf-135">Request</span></span>

<span data-ttu-id="f0ecf-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

#### <a name="response"></a><span data-ttu-id="f0ecf-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0ecf-137">Response</span></span>

<span data-ttu-id="f0ecf-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-138">The following is an example of the response.</span></span> 

><span data-ttu-id="f0ecf-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f0ecf-141">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="f0ecf-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f0ecf-142">C#</span><span class="sxs-lookup"><span data-stu-id="f0ecf-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/schedule-delete-schedulinggroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f0ecf-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="f0ecf-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/schedule-delete-schedulinggroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f0ecf-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f0ecf-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/schedule-delete-schedulinggroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/schedulinggroup-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/schedulinggroup-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/schedulinggroup-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
