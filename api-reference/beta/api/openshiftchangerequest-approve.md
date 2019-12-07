---
title: 'Опеншифтчанжерекуест: утверждение'
description: Утверждение запроса опеншифт.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ad2b3acd52bd62a6c16c70708aa2f4b5809b0b09
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895832"
---
# <a name="openshiftchangerequest-approve"></a><span data-ttu-id="bbd6d-103">Опеншифтчанжерекуест: утверждение</span><span class="sxs-lookup"><span data-stu-id="bbd6d-103">openShiftChangeRequest: approve</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbd6d-104">Утверждение объекта [опеншифтчанжерекуест](../resources/openshiftchangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="bbd6d-104">Approve an [openshiftchangerequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbd6d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bbd6d-105">Permissions</span></span>

<span data-ttu-id="bbd6d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbd6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bbd6d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbd6d-108">Permission type</span></span>                        | <span data-ttu-id="bbd6d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbd6d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bbd6d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbd6d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bbd6d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbd6d-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="bbd6d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbd6d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbd6d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbd6d-113">Not supported.</span></span> |
| <span data-ttu-id="bbd6d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bbd6d-114">Application</span></span>                            | <span data-ttu-id="bbd6d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbd6d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbd6d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbd6d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftsChangeRequests/approve
```

## <a name="request-headers"></a><span data-ttu-id="bbd6d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bbd6d-117">Request headers</span></span>

| <span data-ttu-id="bbd6d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bbd6d-118">Name</span></span>          | <span data-ttu-id="bbd6d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bbd6d-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bbd6d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bbd6d-120">Authorization</span></span> | <span data-ttu-id="bbd6d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bbd6d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bbd6d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bbd6d-123">Content-type</span></span> | <span data-ttu-id="bbd6d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bbd6d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbd6d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bbd6d-126">Request body</span></span>

<span data-ttu-id="bbd6d-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="bbd6d-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bbd6d-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="bbd6d-128">Parameter</span></span>    | <span data-ttu-id="bbd6d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bbd6d-129">Type</span></span>        | <span data-ttu-id="bbd6d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bbd6d-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bbd6d-131">message</span><span class="sxs-lookup"><span data-stu-id="bbd6d-131">message</span></span>|<span data-ttu-id="bbd6d-132">String</span><span class="sxs-lookup"><span data-stu-id="bbd6d-132">String</span></span>|<span data-ttu-id="bbd6d-133">Настраиваемое сообщение утверждения.</span><span class="sxs-lookup"><span data-stu-id="bbd6d-133">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="bbd6d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbd6d-134">Response</span></span>

<span data-ttu-id="bbd6d-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bbd6d-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bbd6d-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="bbd6d-137">Examples</span></span>

<span data-ttu-id="bbd6d-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="bbd6d-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="bbd6d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbd6d-139">Request</span></span>

<span data-ttu-id="bbd6d-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bbd6d-140">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftsChangeRequests/approve
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="bbd6d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbd6d-141">Response</span></span>

<span data-ttu-id="bbd6d-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bbd6d-142">The following is an example of the response.</span></span>
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
