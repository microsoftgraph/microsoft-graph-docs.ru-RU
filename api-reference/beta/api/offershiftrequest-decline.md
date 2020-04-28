---
title: 'Оффершифтрекуест: отклонить'
description: Отклонить запрос на смену предложения.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 33d837aa24e7c13bf47821ca90417407de81c97a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456602"
---
# <a name="offershiftrequest-decline"></a><span data-ttu-id="a66bf-103">Оффершифтрекуест: отклонить</span><span class="sxs-lookup"><span data-stu-id="a66bf-103">offerShiftRequest: decline</span></span>

<span data-ttu-id="a66bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a66bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a66bf-105">Отклонить объект [оффершифтрекуест](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="a66bf-105">Decline an [offershiftrequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a66bf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a66bf-106">Permissions</span></span>

<span data-ttu-id="a66bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a66bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a66bf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a66bf-109">Permission type</span></span>                        | <span data-ttu-id="a66bf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a66bf-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a66bf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a66bf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a66bf-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a66bf-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="a66bf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a66bf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a66bf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a66bf-114">Not supported.</span></span> |
| <span data-ttu-id="a66bf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a66bf-115">Application</span></span>                            | <span data-ttu-id="a66bf-116">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="a66bf-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="a66bf-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="a66bf-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="a66bf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a66bf-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/schedule/offerShiftRequests/decline
```

## <a name="request-headers"></a><span data-ttu-id="a66bf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a66bf-119">Request headers</span></span>

| <span data-ttu-id="a66bf-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a66bf-120">Name</span></span>          | <span data-ttu-id="a66bf-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a66bf-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a66bf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a66bf-122">Authorization</span></span> | <span data-ttu-id="a66bf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a66bf-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a66bf-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a66bf-125">Content-type</span></span> | <span data-ttu-id="a66bf-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a66bf-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a66bf-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a66bf-128">Request body</span></span>

<span data-ttu-id="a66bf-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a66bf-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a66bf-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="a66bf-130">Parameter</span></span>    | <span data-ttu-id="a66bf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a66bf-131">Type</span></span>        | <span data-ttu-id="a66bf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a66bf-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a66bf-133">message</span><span class="sxs-lookup"><span data-stu-id="a66bf-133">message</span></span>|<span data-ttu-id="a66bf-134">String</span><span class="sxs-lookup"><span data-stu-id="a66bf-134">String</span></span>|<span data-ttu-id="a66bf-135">Настраиваемое сообщение, отправленное при отклонении.</span><span class="sxs-lookup"><span data-stu-id="a66bf-135">Custom message sent on decline.</span></span>|

## <a name="response"></a><span data-ttu-id="a66bf-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a66bf-136">Response</span></span>

<span data-ttu-id="a66bf-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a66bf-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a66bf-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="a66bf-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a66bf-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="a66bf-140">Request</span></span>

<span data-ttu-id="a66bf-141">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a66bf-141">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a66bf-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="a66bf-142">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="a66bf-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a66bf-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a66bf-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="a66bf-144">Response</span></span>

<span data-ttu-id="a66bf-145">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a66bf-145">The following example shows the response.</span></span>
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
