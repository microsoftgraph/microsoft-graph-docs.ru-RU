---
title: 'Оффершифтрекуест: отклонить'
description: Отклонить запрос на смену предложения.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 94daed01b2b7d4131a09504773c5377889b7e587
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154944"
---
# <a name="offershiftrequest-decline"></a><span data-ttu-id="e131e-103">Оффершифтрекуест: отклонить</span><span class="sxs-lookup"><span data-stu-id="e131e-103">offerShiftRequest: decline</span></span>

<span data-ttu-id="e131e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e131e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e131e-105">Отклонить объект [оффершифтрекуест](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="e131e-105">Decline an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e131e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e131e-106">Permissions</span></span>

<span data-ttu-id="e131e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e131e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e131e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e131e-109">Permission type</span></span>                        | <span data-ttu-id="e131e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e131e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e131e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e131e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e131e-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e131e-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="e131e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e131e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e131e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e131e-114">Not supported.</span></span> |
| <span data-ttu-id="e131e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e131e-115">Application</span></span>                            | <span data-ttu-id="e131e-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e131e-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="e131e-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="e131e-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e131e-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="e131e-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e131e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e131e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="e131e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e131e-120">Request headers</span></span>

| <span data-ttu-id="e131e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e131e-121">Name</span></span>          | <span data-ttu-id="e131e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e131e-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e131e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e131e-123">Authorization</span></span> | <span data-ttu-id="e131e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e131e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e131e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e131e-126">Content-type</span></span> | <span data-ttu-id="e131e-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e131e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e131e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e131e-129">Request body</span></span>

<span data-ttu-id="e131e-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e131e-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e131e-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="e131e-131">Parameter</span></span>    | <span data-ttu-id="e131e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e131e-132">Type</span></span>        | <span data-ttu-id="e131e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e131e-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e131e-134">message</span><span class="sxs-lookup"><span data-stu-id="e131e-134">message</span></span>|<span data-ttu-id="e131e-135">String</span><span class="sxs-lookup"><span data-stu-id="e131e-135">String</span></span>|<span data-ttu-id="e131e-136">Настраиваемое сообщение, отправленное при отклонении.</span><span class="sxs-lookup"><span data-stu-id="e131e-136">Custom message sent on decline.</span></span>|

## <a name="response"></a><span data-ttu-id="e131e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e131e-137">Response</span></span>

<span data-ttu-id="e131e-p105">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e131e-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e131e-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="e131e-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e131e-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="e131e-141">Request</span></span>

<span data-ttu-id="e131e-142">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e131e-142">The following example shows a request.</span></span>

<!-- {
  "blockType": "request",
  "name": "offershiftrequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
Content-type: application/json

{
  "message": "Sorry, you can't offer this shift."
}
```

---


### <a name="response"></a><span data-ttu-id="e131e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e131e-143">Response</span></span>

<span data-ttu-id="e131e-144">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e131e-144">The following example shows the response.</span></span>
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
  "description": "offerShiftRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
