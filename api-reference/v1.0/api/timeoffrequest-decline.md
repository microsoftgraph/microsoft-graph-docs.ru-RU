---
title: 'Тимеоффрекуест: отклонить'
description: Отклонить объект тимеоффрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 93d303c4ea1088b8e317ed2845ce99ba59ef76e3
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154313"
---
# <a name="timeoffrequest-decline"></a><span data-ttu-id="3e000-103">Тимеоффрекуест: отклонить</span><span class="sxs-lookup"><span data-stu-id="3e000-103">timeOffRequest: decline</span></span>

<span data-ttu-id="3e000-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e000-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3e000-105">Отклонить объект [тимеоффрекуест](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="3e000-105">Decline a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e000-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e000-106">Permissions</span></span>

<span data-ttu-id="3e000-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e000-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e000-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e000-109">Permission type</span></span>                        | <span data-ttu-id="3e000-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e000-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="3e000-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e000-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3e000-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3e000-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3e000-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e000-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e000-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e000-114">Not supported.</span></span>    |
|<span data-ttu-id="3e000-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e000-115">Application</span></span> | <span data-ttu-id="3e000-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e000-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="3e000-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="3e000-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3e000-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="3e000-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3e000-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e000-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="3e000-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e000-120">Request headers</span></span>

| <span data-ttu-id="3e000-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3e000-121">Name</span></span>          | <span data-ttu-id="3e000-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3e000-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3e000-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e000-123">Authorization</span></span> | <span data-ttu-id="3e000-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e000-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3e000-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3e000-126">Content-type</span></span> | <span data-ttu-id="3e000-127">приложение — JSON.</span><span class="sxs-lookup"><span data-stu-id="3e000-127">application-json.</span></span> <span data-ttu-id="3e000-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="3e000-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e000-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e000-129">Request body</span></span>

<span data-ttu-id="3e000-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3e000-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3e000-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="3e000-131">Parameter</span></span>    | <span data-ttu-id="3e000-132">Тип</span><span class="sxs-lookup"><span data-stu-id="3e000-132">Type</span></span>        | <span data-ttu-id="3e000-133">Описание</span><span class="sxs-lookup"><span data-stu-id="3e000-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3e000-134">message</span><span class="sxs-lookup"><span data-stu-id="3e000-134">message</span></span>|<span data-ttu-id="3e000-135">String</span><span class="sxs-lookup"><span data-stu-id="3e000-135">String</span></span>|<span data-ttu-id="3e000-136">Настраиваемое сообщение об отклонении.</span><span class="sxs-lookup"><span data-stu-id="3e000-136">Custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="3e000-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e000-137">Response</span></span>

<span data-ttu-id="3e000-p105">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3e000-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3e000-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="3e000-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3e000-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e000-141">Request</span></span>

<span data-ttu-id="3e000-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e000-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "timeoffrequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```
---


### <a name="response"></a><span data-ttu-id="3e000-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e000-143">Response</span></span>

<span data-ttu-id="3e000-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3e000-144">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeOffRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
