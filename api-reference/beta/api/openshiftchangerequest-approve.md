---
title: 'openShiftChangeRequest: утвердить'
description: Утверждение запроса openshift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6ee856fef01a992eb5a1e82776d44a414ed9f888
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292450"
---
# <a name="openshiftchangerequest-approve"></a><span data-ttu-id="2a810-103">openShiftChangeRequest: утвердить</span><span class="sxs-lookup"><span data-stu-id="2a810-103">openShiftChangeRequest: approve</span></span>

<span data-ttu-id="2a810-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a810-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a810-105">Утверждение объекта [openshiftchangerequest.](../resources/openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="2a810-105">Approve an [openshiftchangerequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a810-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a810-106">Permissions</span></span>

<span data-ttu-id="2a810-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a810-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a810-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a810-109">Permission type</span></span>                        | <span data-ttu-id="2a810-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a810-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2a810-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a810-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a810-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a810-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="2a810-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a810-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a810-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a810-114">Not supported.</span></span> |
| <span data-ttu-id="2a810-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a810-115">Application</span></span>                            | <span data-ttu-id="2a810-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a810-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a810-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a810-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="2a810-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a810-118">Request headers</span></span>

| <span data-ttu-id="2a810-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2a810-119">Name</span></span>          | <span data-ttu-id="2a810-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2a810-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2a810-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a810-121">Authorization</span></span> | <span data-ttu-id="2a810-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a810-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2a810-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a810-124">Content-type</span></span> | <span data-ttu-id="2a810-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a810-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a810-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a810-127">Request body</span></span>

<span data-ttu-id="2a810-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2a810-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2a810-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="2a810-129">Parameter</span></span>    | <span data-ttu-id="2a810-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2a810-130">Type</span></span>        | <span data-ttu-id="2a810-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2a810-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2a810-132">message</span><span class="sxs-lookup"><span data-stu-id="2a810-132">message</span></span>|<span data-ttu-id="2a810-133">String</span><span class="sxs-lookup"><span data-stu-id="2a810-133">String</span></span>|<span data-ttu-id="2a810-134">Пользовательское сообщение об утверждении.</span><span class="sxs-lookup"><span data-stu-id="2a810-134">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="2a810-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a810-135">Response</span></span>

<span data-ttu-id="2a810-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2a810-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a810-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="2a810-138">Examples</span></span>

<span data-ttu-id="2a810-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="2a810-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="2a810-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a810-140">Request</span></span>

<span data-ttu-id="2a810-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a810-141">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="2a810-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a810-142">Response</span></span>

<span data-ttu-id="2a810-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2a810-143">The following is an example of the response.</span></span>
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


