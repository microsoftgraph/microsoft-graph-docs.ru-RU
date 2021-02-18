---
title: 'openShiftChangeRequest: decline'
description: Отклонение openShiftChangeRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4801239c9d149ce20d056db612e95a3209b8ea5a
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292366"
---
# <a name="openshiftchangerequest-decline"></a><span data-ttu-id="48aa6-103">openShiftChangeRequest: decline</span><span class="sxs-lookup"><span data-stu-id="48aa6-103">openShiftChangeRequest: decline</span></span>

<span data-ttu-id="48aa6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48aa6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="48aa6-105">Отклонение [объекта openShiftChangeRequest.](../resources/openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="48aa6-105">Decline an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="48aa6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48aa6-106">Permissions</span></span>

<span data-ttu-id="48aa6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48aa6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48aa6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48aa6-109">Permission type</span></span>                        | <span data-ttu-id="48aa6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48aa6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="48aa6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48aa6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="48aa6-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48aa6-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="48aa6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48aa6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48aa6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48aa6-114">Not supported.</span></span> |
| <span data-ttu-id="48aa6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48aa6-115">Application</span></span>                            | <span data-ttu-id="48aa6-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48aa6-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="48aa6-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="48aa6-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="48aa6-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="48aa6-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="48aa6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48aa6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="48aa6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48aa6-120">Request headers</span></span>

| <span data-ttu-id="48aa6-121">Имя</span><span class="sxs-lookup"><span data-stu-id="48aa6-121">Name</span></span>          | <span data-ttu-id="48aa6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="48aa6-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="48aa6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48aa6-123">Authorization</span></span> | <span data-ttu-id="48aa6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48aa6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="48aa6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="48aa6-126">Content-type</span></span> | <span data-ttu-id="48aa6-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48aa6-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48aa6-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48aa6-129">Request body</span></span>

<span data-ttu-id="48aa6-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="48aa6-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="48aa6-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="48aa6-131">Parameter</span></span>    | <span data-ttu-id="48aa6-132">Тип</span><span class="sxs-lookup"><span data-stu-id="48aa6-132">Type</span></span>        | <span data-ttu-id="48aa6-133">Описание</span><span class="sxs-lookup"><span data-stu-id="48aa6-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="48aa6-134">message</span><span class="sxs-lookup"><span data-stu-id="48aa6-134">message</span></span>|<span data-ttu-id="48aa6-135">String</span><span class="sxs-lookup"><span data-stu-id="48aa6-135">String</span></span>|<span data-ttu-id="48aa6-136">Пользовательское сообщение об отклонении.</span><span class="sxs-lookup"><span data-stu-id="48aa6-136">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="48aa6-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="48aa6-137">Response</span></span>

<span data-ttu-id="48aa6-p105">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="48aa6-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="48aa6-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="48aa6-140">Examples</span></span>

<span data-ttu-id="48aa6-141">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="48aa6-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="48aa6-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="48aa6-142">Request</span></span>

<span data-ttu-id="48aa6-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48aa6-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="48aa6-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="48aa6-144">Response</span></span>

<span data-ttu-id="48aa6-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="48aa6-145">The following is an example of the response.</span></span>
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
  "description": "openShiftChangeRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

