---
title: 'Оффершифтрекуест: утверждение'
description: Утверждение объекта оффершифтрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d1c7bfc627c6a8ff52fe78807783e0c4b88dc90e
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/09/2020
ms.locfileid: "40994950"
---
# <a name="offershiftrequest-approve"></a><span data-ttu-id="0c5db-103">Оффершифтрекуест: утверждение</span><span class="sxs-lookup"><span data-stu-id="0c5db-103">offerShiftRequest: approve</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c5db-104">Утверждение объекта [оффершифтрекуест](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="0c5db-104">Approve an [offershiftrequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c5db-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c5db-105">Permissions</span></span>

<span data-ttu-id="0c5db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c5db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0c5db-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c5db-108">Permission type</span></span>                        | <span data-ttu-id="0c5db-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c5db-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0c5db-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c5db-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0c5db-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c5db-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="0c5db-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c5db-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c5db-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c5db-113">Not supported.</span></span> |
| <span data-ttu-id="0c5db-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="0c5db-114">Application</span></span>                            | <span data-ttu-id="0c5db-115">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="0c5db-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="0c5db-116">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="0c5db-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="0c5db-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c5db-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/schedule/offerShiftRequests/approve
```

## <a name="request-headers"></a><span data-ttu-id="0c5db-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c5db-118">Request headers</span></span>

| <span data-ttu-id="0c5db-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0c5db-119">Name</span></span>          | <span data-ttu-id="0c5db-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0c5db-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0c5db-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c5db-121">Authorization</span></span> | <span data-ttu-id="0c5db-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c5db-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0c5db-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0c5db-124">Content-type</span></span> | <span data-ttu-id="0c5db-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c5db-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c5db-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c5db-127">Request body</span></span>

<span data-ttu-id="0c5db-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0c5db-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0c5db-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="0c5db-129">Parameter</span></span>    | <span data-ttu-id="0c5db-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0c5db-130">Type</span></span>        | <span data-ttu-id="0c5db-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0c5db-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0c5db-132">message</span><span class="sxs-lookup"><span data-stu-id="0c5db-132">message</span></span>|<span data-ttu-id="0c5db-133">String</span><span class="sxs-lookup"><span data-stu-id="0c5db-133">String</span></span>|<span data-ttu-id="0c5db-134">Пользовательское сообщение отправлено при утверждении.</span><span class="sxs-lookup"><span data-stu-id="0c5db-134">Custom message sent on approval.</span></span>|

## <a name="response"></a><span data-ttu-id="0c5db-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c5db-135">Response</span></span>

<span data-ttu-id="0c5db-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0c5db-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0c5db-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="0c5db-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0c5db-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c5db-139">Request</span></span>

<span data-ttu-id="0c5db-140">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c5db-140">The following example shows a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0c5db-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c5db-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/schedule/offerShiftRequests/approve
Content-type: application/json

{
  "message": "Approved!"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c5db-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c5db-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0c5db-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c5db-143">Response</span></span>

<span data-ttu-id="0c5db-144">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0c5db-144">The following example shows the response.</span></span>
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
