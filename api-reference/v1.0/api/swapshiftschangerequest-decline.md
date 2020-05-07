---
title: 'Свапшифтсчанжерекуест: отклонить'
description: Отклонить запрос на замену.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4f51496f69e4c49f5df4e6ccbec5cad044a79678
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154724"
---
# <a name="swapshiftschangerequest-decline"></a><span data-ttu-id="cdc20-103">Свапшифтсчанжерекуест: отклонить</span><span class="sxs-lookup"><span data-stu-id="cdc20-103">swapShiftsChangeRequest: decline</span></span>

<span data-ttu-id="cdc20-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdc20-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cdc20-105">Отклонить объект [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="cdc20-105">Decline a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdc20-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cdc20-106">Permissions</span></span>

<span data-ttu-id="cdc20-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdc20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cdc20-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdc20-109">Permission type</span></span>                        | <span data-ttu-id="cdc20-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdc20-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="cdc20-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdc20-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cdc20-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cdc20-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cdc20-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdc20-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdc20-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdc20-114">Not supported.</span></span>    |<span data-ttu-id="cdc20-115">s</span><span class="sxs-lookup"><span data-stu-id="cdc20-115">s</span></span>
|<span data-ttu-id="cdc20-116">Application</span><span class="sxs-lookup"><span data-stu-id="cdc20-116">Application</span></span> | <span data-ttu-id="cdc20-117">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdc20-117">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="cdc20-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="cdc20-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="cdc20-119">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="cdc20-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="cdc20-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdc20-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="cdc20-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cdc20-121">Request headers</span></span>

| <span data-ttu-id="cdc20-122">Имя</span><span class="sxs-lookup"><span data-stu-id="cdc20-122">Name</span></span>          | <span data-ttu-id="cdc20-123">Описание</span><span class="sxs-lookup"><span data-stu-id="cdc20-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cdc20-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cdc20-124">Authorization</span></span> | <span data-ttu-id="cdc20-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdc20-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cdc20-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cdc20-127">Content-type</span></span> | <span data-ttu-id="cdc20-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdc20-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cdc20-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cdc20-130">Request body</span></span>

<span data-ttu-id="cdc20-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="cdc20-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cdc20-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="cdc20-132">Parameter</span></span>    | <span data-ttu-id="cdc20-133">Тип</span><span class="sxs-lookup"><span data-stu-id="cdc20-133">Type</span></span>        | <span data-ttu-id="cdc20-134">Описание</span><span class="sxs-lookup"><span data-stu-id="cdc20-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cdc20-135">message</span><span class="sxs-lookup"><span data-stu-id="cdc20-135">message</span></span>|<span data-ttu-id="cdc20-136">String</span><span class="sxs-lookup"><span data-stu-id="cdc20-136">String</span></span>|<span data-ttu-id="cdc20-137">Настраиваемое сообщение об отклонении.</span><span class="sxs-lookup"><span data-stu-id="cdc20-137">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="cdc20-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdc20-138">Response</span></span>

<span data-ttu-id="cdc20-p105">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cdc20-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cdc20-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="cdc20-141">Examples</span></span>

<span data-ttu-id="cdc20-142">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="cdc20-142">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="cdc20-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdc20-143">Request</span></span>

<span data-ttu-id="cdc20-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cdc20-144">The following is an example of a request.</span></span>

<!-- {
  "blockType": "request",
  "name": "swapshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```
---


### <a name="response"></a><span data-ttu-id="cdc20-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdc20-145">Response</span></span>

<span data-ttu-id="cdc20-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cdc20-146">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "swapShiftChangeRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
