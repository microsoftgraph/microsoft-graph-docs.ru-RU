---
title: 'Опеншифтчанжерекуест: отклонить'
description: Отклонить запрос опеншифт.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 902b552a8fc6e178c3cef120ace4ea66d954812f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456388"
---
# <a name="openshiftchangerequest-decline"></a><span data-ttu-id="09f39-103">Опеншифтчанжерекуест: отклонить</span><span class="sxs-lookup"><span data-stu-id="09f39-103">openShiftChangeRequest: decline</span></span>

<span data-ttu-id="09f39-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="09f39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09f39-105">Отклонить объект [опеншифтчанжерекуест](../resources/openshiftchangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="09f39-105">Decline an [openshiftchangerequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="09f39-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="09f39-106">Permissions</span></span>

<span data-ttu-id="09f39-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09f39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="09f39-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09f39-109">Permission type</span></span>                        | <span data-ttu-id="09f39-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="09f39-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="09f39-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09f39-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="09f39-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09f39-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="09f39-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09f39-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09f39-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09f39-114">Not supported.</span></span> |
| <span data-ttu-id="09f39-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09f39-115">Application</span></span>                            | <span data-ttu-id="09f39-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09f39-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="09f39-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09f39-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="09f39-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09f39-118">Request headers</span></span>

| <span data-ttu-id="09f39-119">Имя</span><span class="sxs-lookup"><span data-stu-id="09f39-119">Name</span></span>          | <span data-ttu-id="09f39-120">Описание</span><span class="sxs-lookup"><span data-stu-id="09f39-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="09f39-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09f39-121">Authorization</span></span> | <span data-ttu-id="09f39-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09f39-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="09f39-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09f39-124">Request body</span></span>

<span data-ttu-id="09f39-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="09f39-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="09f39-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="09f39-126">Parameter</span></span>    | <span data-ttu-id="09f39-127">Тип</span><span class="sxs-lookup"><span data-stu-id="09f39-127">Type</span></span>        | <span data-ttu-id="09f39-128">Описание</span><span class="sxs-lookup"><span data-stu-id="09f39-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="09f39-129">message</span><span class="sxs-lookup"><span data-stu-id="09f39-129">message</span></span>|<span data-ttu-id="09f39-130">String</span><span class="sxs-lookup"><span data-stu-id="09f39-130">String</span></span>|<span data-ttu-id="09f39-131">Настраиваемое сообщение об отклонении.</span><span class="sxs-lookup"><span data-stu-id="09f39-131">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="09f39-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="09f39-132">Response</span></span>

<span data-ttu-id="09f39-p103">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="09f39-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="09f39-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="09f39-135">Examples</span></span>

<span data-ttu-id="09f39-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="09f39-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="09f39-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="09f39-137">Request</span></span>

<span data-ttu-id="09f39-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09f39-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="09f39-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="09f39-139">Response</span></span>

<span data-ttu-id="09f39-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="09f39-140">The following is an example of the response.</span></span>
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
