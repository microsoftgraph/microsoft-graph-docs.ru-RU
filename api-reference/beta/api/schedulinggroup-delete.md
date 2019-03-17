---
title: Удаление Счедулингграуп
description: ПоМетка элемента Счедулингграуп как неактивного путем задания его свойства "свойство Active"
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bb29270cdf246924f0c6a9293611bec82dac5cc3
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657716"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="27a69-103">Удаление Счедулингграуп</span><span class="sxs-lookup"><span data-stu-id="27a69-103">Delete schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27a69-104">ПоМечайте [счедулингграуп](../resources/schedulinggroup.md) как неактивную \*\*\*\* , устанавливая его свойство GetProperty.</span><span class="sxs-lookup"><span data-stu-id="27a69-104">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="27a69-105">Этот метод не удаляет [счедулингграуп](../resources/schedulinggroup.md) из расписания.</span><span class="sxs-lookup"><span data-stu-id="27a69-105">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="27a69-106">Существующие [сменные](../resources/shift.md) экземпляры, назначенные группе планирования, не входят в группу.</span><span class="sxs-lookup"><span data-stu-id="27a69-106">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="27a69-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27a69-107">Permissions</span></span>

<span data-ttu-id="27a69-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27a69-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27a69-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27a69-110">Permission type</span></span>      | <span data-ttu-id="27a69-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27a69-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27a69-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27a69-112">Delegated (work or school account)</span></span> | <span data-ttu-id="27a69-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27a69-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="27a69-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27a69-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27a69-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27a69-115">Not supported.</span></span>    |
|<span data-ttu-id="27a69-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27a69-116">Application</span></span> | <span data-ttu-id="27a69-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27a69-117">Not supported.</span></span> |

> <span data-ttu-id="27a69-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="27a69-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="27a69-119">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="27a69-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="27a69-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27a69-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="27a69-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27a69-121">Request headers</span></span>

| <span data-ttu-id="27a69-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="27a69-122">Header</span></span>       | <span data-ttu-id="27a69-123">Значение</span><span class="sxs-lookup"><span data-stu-id="27a69-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="27a69-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27a69-124">Authorization</span></span>  | <span data-ttu-id="27a69-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27a69-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="27a69-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27a69-127">Content-Type</span></span>  | <span data-ttu-id="27a69-128">application/json</span><span class="sxs-lookup"><span data-stu-id="27a69-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="27a69-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27a69-129">Request body</span></span>
<span data-ttu-id="27a69-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="27a69-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27a69-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="27a69-131">Response</span></span>

<span data-ttu-id="27a69-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="27a69-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27a69-134">Пример</span><span class="sxs-lookup"><span data-stu-id="27a69-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="27a69-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="27a69-135">Request</span></span>

<span data-ttu-id="27a69-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27a69-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

#### <a name="response"></a><span data-ttu-id="27a69-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="27a69-137">Response</span></span>

<span data-ttu-id="27a69-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="27a69-138">The following is an example of the response.</span></span> 

><span data-ttu-id="27a69-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="27a69-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/schedule-delete-schedulinggroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
