---
title: 'Оффершифтрекуест: утверждение'
description: Утверждение объекта Оффершифтрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 98ec1f11b4364b26d478d8830a0e563ad1b7ab6b
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154951"
---
# <a name="offershiftrequest-approve"></a><span data-ttu-id="fe695-103">Оффершифтрекуест: утверждение</span><span class="sxs-lookup"><span data-stu-id="fe695-103">offerShiftRequest: approve</span></span>

<span data-ttu-id="fe695-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe695-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe695-105">Утверждение объекта [оффершифтрекуест](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="fe695-105">Approve an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe695-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe695-106">Permissions</span></span>

<span data-ttu-id="fe695-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe695-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fe695-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe695-109">Permission type</span></span>                        | <span data-ttu-id="fe695-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe695-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fe695-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe695-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe695-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fe695-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="fe695-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe695-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe695-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe695-114">Not supported.</span></span> |
| <span data-ttu-id="fe695-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe695-115">Application</span></span>                            | <span data-ttu-id="fe695-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe695-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="fe695-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="fe695-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="fe695-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="fe695-118">Global admins can access groups that they are not a member of.</span></span>


## <a name="http-request"></a><span data-ttu-id="fe695-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe695-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="fe695-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe695-120">Request headers</span></span>

| <span data-ttu-id="fe695-121">Имя</span><span class="sxs-lookup"><span data-stu-id="fe695-121">Name</span></span>          | <span data-ttu-id="fe695-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fe695-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fe695-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe695-123">Authorization</span></span> | <span data-ttu-id="fe695-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe695-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fe695-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe695-126">Content-type</span></span> | <span data-ttu-id="fe695-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe695-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe695-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe695-129">Request body</span></span>

<span data-ttu-id="fe695-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="fe695-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fe695-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="fe695-131">Parameter</span></span>    | <span data-ttu-id="fe695-132">Тип</span><span class="sxs-lookup"><span data-stu-id="fe695-132">Type</span></span>        | <span data-ttu-id="fe695-133">Описание</span><span class="sxs-lookup"><span data-stu-id="fe695-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fe695-134">message</span><span class="sxs-lookup"><span data-stu-id="fe695-134">message</span></span>|<span data-ttu-id="fe695-135">String</span><span class="sxs-lookup"><span data-stu-id="fe695-135">String</span></span>|<span data-ttu-id="fe695-136">Пользовательское сообщение отправлено при утверждении.</span><span class="sxs-lookup"><span data-stu-id="fe695-136">Custom message sent on approval.</span></span>|

## <a name="response"></a><span data-ttu-id="fe695-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe695-137">Response</span></span>

<span data-ttu-id="fe695-p105">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fe695-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fe695-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="fe695-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fe695-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe695-141">Request</span></span>

<span data-ttu-id="fe695-142">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe695-142">The following example shows a request.</span></span>

<!-- {
  "blockType": "request",
  "name": "offershiftrequest_approve"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/approve
Content-type: application/json

{
  "message": "Approved!"
}
```
---


### <a name="response"></a><span data-ttu-id="fe695-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe695-143">Response</span></span>

<span data-ttu-id="fe695-144">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fe695-144">The following example shows the response.</span></span>
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
  "description": "offerShiftRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
