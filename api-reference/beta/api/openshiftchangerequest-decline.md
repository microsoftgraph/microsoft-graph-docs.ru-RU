---
title: 'Опеншифтчанжерекуест: отклонить'
description: Отклонить запрос опеншифт.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3b59bd65a79c7a8185749639ef725504c80424ee
ms.sourcegitcommit: 31a9b4cb3d0f905f123475a4c1a86f5b1e59b935
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2020
ms.locfileid: "42219659"
---
# <a name="openshiftchangerequest-decline"></a><span data-ttu-id="4de17-103">Опеншифтчанжерекуест: отклонить</span><span class="sxs-lookup"><span data-stu-id="4de17-103">openShiftChangeRequest: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4de17-104">Отклонить объект [опеншифтчанжерекуест](../resources/openshiftchangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="4de17-104">Decline an [openshiftchangerequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4de17-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4de17-105">Permissions</span></span>

<span data-ttu-id="4de17-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4de17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4de17-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4de17-108">Permission type</span></span>                        | <span data-ttu-id="4de17-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4de17-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4de17-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4de17-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4de17-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4de17-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="4de17-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4de17-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4de17-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4de17-113">Not supported.</span></span> |
| <span data-ttu-id="4de17-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4de17-114">Application</span></span>                            | <span data-ttu-id="4de17-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4de17-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4de17-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4de17-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftsChangeRequests/{openShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="4de17-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4de17-117">Request headers</span></span>

| <span data-ttu-id="4de17-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4de17-118">Name</span></span>          | <span data-ttu-id="4de17-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4de17-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4de17-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4de17-120">Authorization</span></span> | <span data-ttu-id="4de17-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4de17-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4de17-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4de17-123">Request body</span></span>

<span data-ttu-id="4de17-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4de17-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4de17-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="4de17-125">Parameter</span></span>    | <span data-ttu-id="4de17-126">Тип</span><span class="sxs-lookup"><span data-stu-id="4de17-126">Type</span></span>        | <span data-ttu-id="4de17-127">Описание</span><span class="sxs-lookup"><span data-stu-id="4de17-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4de17-128">message</span><span class="sxs-lookup"><span data-stu-id="4de17-128">message</span></span>|<span data-ttu-id="4de17-129">String</span><span class="sxs-lookup"><span data-stu-id="4de17-129">String</span></span>|<span data-ttu-id="4de17-130">Настраиваемое сообщение об отклонении.</span><span class="sxs-lookup"><span data-stu-id="4de17-130">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="4de17-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4de17-131">Response</span></span>

<span data-ttu-id="4de17-p103">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4de17-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4de17-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="4de17-134">Examples</span></span>

<span data-ttu-id="4de17-135">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="4de17-135">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="4de17-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="4de17-136">Request</span></span>

<span data-ttu-id="4de17-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4de17-137">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4de17-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4de17-138">Response</span></span>

<span data-ttu-id="4de17-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4de17-139">The following is an example of the response.</span></span>
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
