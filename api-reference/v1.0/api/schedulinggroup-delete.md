---
title: Удаление объекта schedulingGroup
description: Пометка элемента Счедулингграуп как неактивного путем задания его свойства "свойство Active"
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7c7aae33e48ca3170cdc2ce06e96d704139ec13f
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155140"
---
# <a name="delete-schedulinggroup"></a><span data-ttu-id="13a82-103">Удаление объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="13a82-103">Delete schedulingGroup</span></span>

<span data-ttu-id="13a82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13a82-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="13a82-105">Помечайте [счедулингграуп](../resources/schedulinggroup.md) как неактивную, устанавливая **его свойство** GetProperty.</span><span class="sxs-lookup"><span data-stu-id="13a82-105">Mark a [schedulingGroup](../resources/schedulinggroup.md) as inactive by setting its **isActive** property.</span></span>
<span data-ttu-id="13a82-106">Этот метод не удаляет [счедулингграуп](../resources/schedulinggroup.md) из расписания.</span><span class="sxs-lookup"><span data-stu-id="13a82-106">This method does not remove the [schedulingGroup](../resources/schedulinggroup.md) from the schedule.</span></span> <span data-ttu-id="13a82-107">Существующие [сменные](../resources/shift.md) экземпляры, назначенные группе планирования, не входят в группу.</span><span class="sxs-lookup"><span data-stu-id="13a82-107">Existing [shift](../resources/shift.md) instances assigned to the scheduling group remain part of the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="13a82-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="13a82-108">Permissions</span></span>

<span data-ttu-id="13a82-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13a82-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13a82-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13a82-111">Permission type</span></span>      | <span data-ttu-id="13a82-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13a82-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13a82-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13a82-113">Delegated (work or school account)</span></span> | <span data-ttu-id="13a82-114">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="13a82-114">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="13a82-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13a82-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13a82-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13a82-116">Not supported.</span></span>    |
|<span data-ttu-id="13a82-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13a82-117">Application</span></span> | <span data-ttu-id="13a82-118">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13a82-118">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="13a82-119">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="13a82-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="13a82-120">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="13a82-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="13a82-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13a82-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="13a82-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13a82-122">Request headers</span></span>

| <span data-ttu-id="13a82-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13a82-123">Header</span></span>       | <span data-ttu-id="13a82-124">Значение</span><span class="sxs-lookup"><span data-stu-id="13a82-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="13a82-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13a82-125">Authorization</span></span>  | <span data-ttu-id="13a82-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13a82-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="13a82-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13a82-128">Request body</span></span>
<span data-ttu-id="13a82-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="13a82-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13a82-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="13a82-130">Response</span></span>

<span data-ttu-id="13a82-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="13a82-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13a82-133">Пример</span><span class="sxs-lookup"><span data-stu-id="13a82-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="13a82-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="13a82-134">Request</span></span>

<span data-ttu-id="13a82-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13a82-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "schedule-delete-schedulinggroups"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
---


### <a name="response"></a><span data-ttu-id="13a82-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="13a82-136">Response</span></span>

<span data-ttu-id="13a82-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="13a82-137">The following is an example of the response.</span></span> 

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
