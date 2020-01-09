---
title: 'Оффершифтрекуест: отклонить'
description: Отклонить запрос на смену предложения.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 92a085bb089c549bf4860dcbce135cd4f887ea48
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/09/2020
ms.locfileid: "40994936"
---
# <a name="offershiftrequest-decline"></a><span data-ttu-id="63b78-103">Оффершифтрекуест: отклонить</span><span class="sxs-lookup"><span data-stu-id="63b78-103">offerShiftRequest: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63b78-104">Отклонить объект [оффершифтрекуест](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="63b78-104">Decline an [offershiftrequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="63b78-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63b78-105">Permissions</span></span>

<span data-ttu-id="63b78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63b78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="63b78-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63b78-108">Permission type</span></span>                        | <span data-ttu-id="63b78-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63b78-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="63b78-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63b78-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="63b78-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63b78-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="63b78-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63b78-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63b78-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63b78-113">Not supported.</span></span> |
| <span data-ttu-id="63b78-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="63b78-114">Application</span></span>                            | <span data-ttu-id="63b78-115">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="63b78-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="63b78-116">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="63b78-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="63b78-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63b78-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/schedule/offerShiftRequests/decline
```

## <a name="request-headers"></a><span data-ttu-id="63b78-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63b78-118">Request headers</span></span>

| <span data-ttu-id="63b78-119">Имя</span><span class="sxs-lookup"><span data-stu-id="63b78-119">Name</span></span>          | <span data-ttu-id="63b78-120">Описание</span><span class="sxs-lookup"><span data-stu-id="63b78-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="63b78-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63b78-121">Authorization</span></span> | <span data-ttu-id="63b78-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63b78-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="63b78-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="63b78-124">Content-type</span></span> | <span data-ttu-id="63b78-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63b78-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63b78-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63b78-127">Request body</span></span>

<span data-ttu-id="63b78-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="63b78-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="63b78-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="63b78-129">Parameter</span></span>    | <span data-ttu-id="63b78-130">Тип</span><span class="sxs-lookup"><span data-stu-id="63b78-130">Type</span></span>        | <span data-ttu-id="63b78-131">Описание</span><span class="sxs-lookup"><span data-stu-id="63b78-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="63b78-132">message</span><span class="sxs-lookup"><span data-stu-id="63b78-132">message</span></span>|<span data-ttu-id="63b78-133">String</span><span class="sxs-lookup"><span data-stu-id="63b78-133">String</span></span>|<span data-ttu-id="63b78-134">Настраиваемое сообщение, отправленное при отклонении.</span><span class="sxs-lookup"><span data-stu-id="63b78-134">Custom message sent on decline.</span></span>|

## <a name="response"></a><span data-ttu-id="63b78-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="63b78-135">Response</span></span>

<span data-ttu-id="63b78-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="63b78-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63b78-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="63b78-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="63b78-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="63b78-139">Request</span></span>

<span data-ttu-id="63b78-140">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63b78-140">The following example shows a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="63b78-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="63b78-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/schedule/offerShiftRequests/decline
Content-type: application/json

{
  "message": "Sorry, you can't offer this shift."
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="63b78-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63b78-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="63b78-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="63b78-143">Response</span></span>

<span data-ttu-id="63b78-144">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="63b78-144">The following example shows the response.</span></span>
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
