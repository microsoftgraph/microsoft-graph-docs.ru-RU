---
title: 'Оффершифтрекуест: отклонить'
description: Отклонить запрос на смену предложения.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c3edf437b87af8bc222a51c1532367e12ad44953
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217010"
---
# <a name="offershiftrequest-decline"></a><span data-ttu-id="53e22-103">Оффершифтрекуест: отклонить</span><span class="sxs-lookup"><span data-stu-id="53e22-103">offerShiftRequest: decline</span></span>

<span data-ttu-id="53e22-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53e22-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53e22-105">Отклонить объект [оффершифтрекуест](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="53e22-105">Decline an [offershiftrequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="53e22-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53e22-106">Permissions</span></span>

<span data-ttu-id="53e22-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53e22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53e22-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53e22-109">Permission type</span></span>                        | <span data-ttu-id="53e22-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53e22-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="53e22-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53e22-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="53e22-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53e22-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="53e22-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53e22-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53e22-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53e22-114">Not supported.</span></span> |
| <span data-ttu-id="53e22-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53e22-115">Application</span></span>                            | <span data-ttu-id="53e22-116">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="53e22-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="53e22-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="53e22-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="53e22-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53e22-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="53e22-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53e22-119">Request headers</span></span>

| <span data-ttu-id="53e22-120">Имя</span><span class="sxs-lookup"><span data-stu-id="53e22-120">Name</span></span>          | <span data-ttu-id="53e22-121">Описание</span><span class="sxs-lookup"><span data-stu-id="53e22-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="53e22-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53e22-122">Authorization</span></span> | <span data-ttu-id="53e22-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53e22-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53e22-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53e22-125">Content-type</span></span> | <span data-ttu-id="53e22-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53e22-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53e22-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53e22-128">Request body</span></span>

<span data-ttu-id="53e22-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="53e22-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="53e22-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="53e22-130">Parameter</span></span>    | <span data-ttu-id="53e22-131">Тип</span><span class="sxs-lookup"><span data-stu-id="53e22-131">Type</span></span>        | <span data-ttu-id="53e22-132">Описание</span><span class="sxs-lookup"><span data-stu-id="53e22-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="53e22-133">message</span><span class="sxs-lookup"><span data-stu-id="53e22-133">message</span></span>|<span data-ttu-id="53e22-134">String</span><span class="sxs-lookup"><span data-stu-id="53e22-134">String</span></span>|<span data-ttu-id="53e22-135">Настраиваемое сообщение, отправленное при отклонении.</span><span class="sxs-lookup"><span data-stu-id="53e22-135">Custom message sent on decline.</span></span>|

## <a name="response"></a><span data-ttu-id="53e22-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="53e22-136">Response</span></span>

<span data-ttu-id="53e22-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="53e22-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53e22-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="53e22-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="53e22-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="53e22-140">Request</span></span>

<span data-ttu-id="53e22-141">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53e22-141">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="53e22-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="53e22-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
Content-type: application/json

{
  "message": "Sorry, you can't offer this shift."
}
```
# <a name="javascript"></a>[<span data-ttu-id="53e22-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53e22-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="53e22-144">C#</span><span class="sxs-lookup"><span data-stu-id="53e22-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/offershiftrequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53e22-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53e22-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/offershiftrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="53e22-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="53e22-146">Response</span></span>

<span data-ttu-id="53e22-147">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="53e22-147">The following example shows the response.</span></span>
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
