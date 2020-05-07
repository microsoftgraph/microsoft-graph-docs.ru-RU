---
title: Удаление смены
description: Удалить смену из расписания.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f3e08c9a8624787c0ce961dd4558bd3b21453667
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154117"
---
# <a name="delete-shift"></a><span data-ttu-id="7591b-103">Удаление смены</span><span class="sxs-lookup"><span data-stu-id="7591b-103">Delete shift</span></span>

<span data-ttu-id="7591b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7591b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7591b-105">Удалить [смену](../resources/shift.md) из расписания.</span><span class="sxs-lookup"><span data-stu-id="7591b-105">Delete a [shift](../resources/shift.md) from the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="7591b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7591b-106">Permissions</span></span>

<span data-ttu-id="7591b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7591b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7591b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7591b-109">Permission type</span></span>      | <span data-ttu-id="7591b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7591b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7591b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7591b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7591b-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7591b-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7591b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7591b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7591b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7591b-114">Not supported.</span></span>    |
|<span data-ttu-id="7591b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7591b-115">Application</span></span> | <span data-ttu-id="7591b-116">Schedule. Read. ALL, Schedule. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7591b-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="7591b-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="7591b-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="7591b-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="7591b-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="7591b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7591b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="7591b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7591b-120">Request headers</span></span>

| <span data-ttu-id="7591b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7591b-121">Header</span></span>       | <span data-ttu-id="7591b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7591b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7591b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7591b-123">Authorization</span></span>  | <span data-ttu-id="7591b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7591b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7591b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7591b-126">Request body</span></span>
<span data-ttu-id="7591b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7591b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7591b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7591b-128">Response</span></span>

<span data-ttu-id="7591b-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7591b-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7591b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7591b-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7591b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7591b-132">Request</span></span>

<span data-ttu-id="7591b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7591b-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "shift-delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/shifts/{shiftId}
```
---


#### <a name="response"></a><span data-ttu-id="7591b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7591b-134">Response</span></span>

<span data-ttu-id="7591b-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7591b-135">The following is an example of the response.</span></span> 

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
  "description": "Deletes a shift from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
