---
title: Удаление Тимеоффреасон
description: Помечайте Тимеоффреасон как неактивную, устанавливая свойство.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5ce465f3fc1d870ab54e9534c001f21dde72e375
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44155014"
---
# <a name="delete-timeoffreason"></a><span data-ttu-id="962fd-103">Удаление Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="962fd-103">Delete timeOffReason</span></span>

<span data-ttu-id="962fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="962fd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="962fd-105">Помечайте Тимеоффреасон как неактивную **isActive** , устанавливая свойство [timeOffReason](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="962fd-105">Mark a [timeOffReason](../resources/timeoffreason.md) as inactive by setting the **isActive** property.</span></span> <span data-ttu-id="962fd-106">Каждая команда должна включать по крайней мере одну причину тимеофф.</span><span class="sxs-lookup"><span data-stu-id="962fd-106">Every team must include at least one timeoff reason.</span></span>

<span data-ttu-id="962fd-107">Этот метод не удаляет указанный экземпляр [тимеоффреасон](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="962fd-107">This method does not remove the specified [timeOffReason](../resources/timeoffreason.md) instance.</span></span> <span data-ttu-id="962fd-108">экземпляры [тимеоффитем](../resources/timeoffitem.md) , которым назначена эта причина, остались назначенными по этой причине.</span><span class="sxs-lookup"><span data-stu-id="962fd-108">[timeOffItem](../resources/timeoffitem.md) instances that have been assigned this reason remain assigned to this reason.</span></span>

## <a name="permissions"></a><span data-ttu-id="962fd-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="962fd-109">Permissions</span></span>

<span data-ttu-id="962fd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="962fd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="962fd-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="962fd-112">Permission type</span></span>      | <span data-ttu-id="962fd-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="962fd-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="962fd-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="962fd-114">Delegated (work or school account)</span></span> | <span data-ttu-id="962fd-115">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="962fd-115">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="962fd-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="962fd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="962fd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="962fd-117">Not supported.</span></span>    |
|<span data-ttu-id="962fd-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="962fd-118">Application</span></span> | <span data-ttu-id="962fd-119">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="962fd-119">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="962fd-120">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="962fd-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="962fd-121">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="962fd-121">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="962fd-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="962fd-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="962fd-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="962fd-123">Request headers</span></span>

| <span data-ttu-id="962fd-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="962fd-124">Header</span></span>       | <span data-ttu-id="962fd-125">Значение</span><span class="sxs-lookup"><span data-stu-id="962fd-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="962fd-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="962fd-126">Authorization</span></span>  | <span data-ttu-id="962fd-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="962fd-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="962fd-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="962fd-129">Request body</span></span>
<span data-ttu-id="962fd-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="962fd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="962fd-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="962fd-131">Response</span></span>

<span data-ttu-id="962fd-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="962fd-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="962fd-134">Пример</span><span class="sxs-lookup"><span data-stu-id="962fd-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="962fd-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="962fd-135">Request</span></span>

<span data-ttu-id="962fd-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="962fd-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
---


### <a name="response"></a><span data-ttu-id="962fd-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="962fd-137">Response</span></span>

<span data-ttu-id="962fd-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="962fd-138">The following is an example of the response.</span></span> 

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
  "description": "Marks a timeOffReason as inactive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
