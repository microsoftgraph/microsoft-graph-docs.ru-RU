---
title: 'Опеншифтчанжерекуест: утверждение'
description: Утверждение запроса опеншифт.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 37af35af00f6c5f0253580f5d5034cfbd8e1f3bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019910"
---
# <a name="openshiftchangerequest-approve"></a><span data-ttu-id="ca5c8-103">Опеншифтчанжерекуест: утверждение</span><span class="sxs-lookup"><span data-stu-id="ca5c8-103">openShiftChangeRequest: approve</span></span>

<span data-ttu-id="ca5c8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca5c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca5c8-105">Утверждение объекта [опеншифтчанжерекуест](../resources/openshiftchangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="ca5c8-105">Approve an [openshiftchangerequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca5c8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca5c8-106">Permissions</span></span>

<span data-ttu-id="ca5c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca5c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ca5c8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca5c8-109">Permission type</span></span>                        | <span data-ttu-id="ca5c8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca5c8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ca5c8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca5c8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca5c8-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca5c8-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="ca5c8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca5c8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca5c8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca5c8-114">Not supported.</span></span> |
| <span data-ttu-id="ca5c8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca5c8-115">Application</span></span>                            | <span data-ttu-id="ca5c8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca5c8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca5c8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca5c8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="ca5c8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca5c8-118">Request headers</span></span>

| <span data-ttu-id="ca5c8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ca5c8-119">Name</span></span>          | <span data-ttu-id="ca5c8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ca5c8-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ca5c8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca5c8-121">Authorization</span></span> | <span data-ttu-id="ca5c8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca5c8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ca5c8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca5c8-124">Content-type</span></span> | <span data-ttu-id="ca5c8-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca5c8-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca5c8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca5c8-127">Request body</span></span>

<span data-ttu-id="ca5c8-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ca5c8-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ca5c8-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="ca5c8-129">Parameter</span></span>    | <span data-ttu-id="ca5c8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ca5c8-130">Type</span></span>        | <span data-ttu-id="ca5c8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ca5c8-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ca5c8-132">message</span><span class="sxs-lookup"><span data-stu-id="ca5c8-132">message</span></span>|<span data-ttu-id="ca5c8-133">String</span><span class="sxs-lookup"><span data-stu-id="ca5c8-133">String</span></span>|<span data-ttu-id="ca5c8-134">Настраиваемое сообщение утверждения.</span><span class="sxs-lookup"><span data-stu-id="ca5c8-134">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="ca5c8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca5c8-135">Response</span></span>

<span data-ttu-id="ca5c8-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ca5c8-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ca5c8-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="ca5c8-138">Examples</span></span>

<span data-ttu-id="ca5c8-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="ca5c8-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="ca5c8-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca5c8-140">Request</span></span>

<span data-ttu-id="ca5c8-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca5c8-141">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="ca5c8-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca5c8-142">Response</span></span>

<span data-ttu-id="ca5c8-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ca5c8-143">The following is an example of the response.</span></span>
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
  "description": "openShiftChangeRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


