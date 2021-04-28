---
title: 'вызов: updateRecordingStatus'
description: Обновление состояния записи приложения, связанного с вызовом.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: f9581584e415bd52b402ab6c677378e7f4cb8d8d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052490"
---
# <a name="call-updaterecordingstatus"></a><span data-ttu-id="cbbf0-103">вызов: updateRecordingStatus</span><span class="sxs-lookup"><span data-stu-id="cbbf0-103">call: updateRecordingStatus</span></span>

<span data-ttu-id="cbbf0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbbf0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cbbf0-105">Обновление состояния записи приложения, связанного с вызовом.</span><span class="sxs-lookup"><span data-stu-id="cbbf0-105">Update the application's recording status associated with a call.</span></span> <span data-ttu-id="cbbf0-106">Это требует использования решения записи [Teams на основе политики.](/MicrosoftTeams/teams-recording-policy)</span><span class="sxs-lookup"><span data-stu-id="cbbf0-106">This requires the use of the [Teams policy-based recording](/MicrosoftTeams/teams-recording-policy) solution.</span></span>

> <span data-ttu-id="cbbf0-107">Дополнительное **ограничение.** Вы не можете использовать API доступа к мультимедиа для записи или иного сохраняемой медиаконтента из звонков или собраний, к которые ваше приложение получает доступ, или данных, полученных из этого медиаконтента ("запись" или "запись"), без вызова API **updateRecordingStatus,** чтобы указать, что запись началась, и получить ответ на успех от этого API.</span><span class="sxs-lookup"><span data-stu-id="cbbf0-107">**Additional Restriction**: You may NOT use the Media Access API to record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content ("record" or "recording"), without first calling the **updateRecordingStatus** API to indicate that recording has begun, and receiving a success reply from that API.</span></span> <span data-ttu-id="cbbf0-108">Если ваше приложение начинает записывать любое собрание, оно должно закончить запись перед вызовом **API updateRecordingStatus,** чтобы указать, что запись завершена.</span><span class="sxs-lookup"><span data-stu-id="cbbf0-108">If your application begins recording any meeting, it must end the recording prior to calling the **updateRecordingStatus** API to indicate that the recording has ended.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbbf0-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cbbf0-109">Permissions</span></span>
<span data-ttu-id="cbbf0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbbf0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cbbf0-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cbbf0-112">Permission type</span></span>                        | <span data-ttu-id="cbbf0-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cbbf0-113">Permissions (from least to most privileged)</span></span>      |
|:---------------------------------------|:-------------------------------------------------|
| <span data-ttu-id="cbbf0-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cbbf0-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="cbbf0-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cbbf0-115">Not Supported</span></span>                                    |
| <span data-ttu-id="cbbf0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cbbf0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbbf0-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cbbf0-117">Not Supported</span></span>                                    |
| <span data-ttu-id="cbbf0-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cbbf0-118">Application</span></span>                            | <span data-ttu-id="cbbf0-119">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="cbbf0-119">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="cbbf0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cbbf0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/updateRecordingStatus
```

## <a name="request-headers"></a><span data-ttu-id="cbbf0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cbbf0-121">Request headers</span></span>
| <span data-ttu-id="cbbf0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="cbbf0-122">Name</span></span>          | <span data-ttu-id="cbbf0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="cbbf0-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="cbbf0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cbbf0-124">Authorization</span></span> | <span data-ttu-id="cbbf0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cbbf0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cbbf0-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cbbf0-127">Content-type</span></span> | <span data-ttu-id="cbbf0-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cbbf0-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cbbf0-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cbbf0-130">Request body</span></span>
<span data-ttu-id="cbbf0-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="cbbf0-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cbbf0-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="cbbf0-132">Parameter</span></span>       | <span data-ttu-id="cbbf0-133">Тип</span><span class="sxs-lookup"><span data-stu-id="cbbf0-133">Type</span></span>    | <span data-ttu-id="cbbf0-134">Описание</span><span class="sxs-lookup"><span data-stu-id="cbbf0-134">Description</span></span>                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| <span data-ttu-id="cbbf0-135">clientContext</span><span class="sxs-lookup"><span data-stu-id="cbbf0-135">clientContext</span></span>   | <span data-ttu-id="cbbf0-136">String</span><span class="sxs-lookup"><span data-stu-id="cbbf0-136">String</span></span>  | <span data-ttu-id="cbbf0-137">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="cbbf0-137">Unique client context string.</span></span> <span data-ttu-id="cbbf0-138">Максимальное ограничение — 256 шаров.</span><span class="sxs-lookup"><span data-stu-id="cbbf0-138">Max limit is 256 chars.</span></span>                                 |
| <span data-ttu-id="cbbf0-139">status</span><span class="sxs-lookup"><span data-stu-id="cbbf0-139">status</span></span>          | <span data-ttu-id="cbbf0-140">String</span><span class="sxs-lookup"><span data-stu-id="cbbf0-140">String</span></span>  | <span data-ttu-id="cbbf0-141">Состояние записи.</span><span class="sxs-lookup"><span data-stu-id="cbbf0-141">The recording status.</span></span> <span data-ttu-id="cbbf0-142">Возможные значения: `notRecording`, `recording` или `failed`.</span><span class="sxs-lookup"><span data-stu-id="cbbf0-142">Possible values are: `notRecording`, `recording`, or `failed`.</span></span>  |

## <a name="response"></a><span data-ttu-id="cbbf0-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbbf0-143">Response</span></span>
<span data-ttu-id="cbbf0-144">Этот метод возвращает код ответа и загорелый загорелый код расположения с URI к объекту `200 OK` [updateRecordingStatusOperation,](../resources/updaterecordingstatusoperation.md) созданному для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="cbbf0-144">This method returns a `200 OK` response code and a Location header with a URI to the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="cbbf0-145">Пример</span><span class="sxs-lookup"><span data-stu-id="cbbf0-145">Example</span></span>
<span data-ttu-id="cbbf0-146">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="cbbf0-146">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="cbbf0-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbbf0-147">Request</span></span>
<span data-ttu-id="cbbf0-148">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbbf0-148">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cbbf0-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="cbbf0-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-updateRecordingStatus"
}-->
```http
POST https://graph.microsoft.com/v1.0/communications/calls/{id}/updateRecordingStatus
Content-Type: application/json
Content-Length: 79

{
  "clientContext": "clientContext-value",
  "status": "notRecording | recording | failed"
}
```
# <a name="c"></a>[<span data-ttu-id="cbbf0-150">C#</span><span class="sxs-lookup"><span data-stu-id="cbbf0-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updaterecordingstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cbbf0-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cbbf0-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updaterecordingstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cbbf0-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cbbf0-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updaterecordingstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cbbf0-153">Java</span><span class="sxs-lookup"><span data-stu-id="cbbf0-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-updaterecordingstatus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="cbbf0-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbbf0-154">Response</span></span>

> <span data-ttu-id="cbbf0-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cbbf0-155">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "name": "call-updateRecordingStatus",
  "truncated": true,
  "@odata.type": "microsoft.graph.updateRecordingStatusOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.updateRecordingStatusOperation",
  "clientContext": "clientContext-value",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "resultInfo": null,
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: updateRecordingStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
