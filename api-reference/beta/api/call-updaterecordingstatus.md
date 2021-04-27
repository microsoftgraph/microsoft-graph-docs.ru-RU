---
title: 'вызов: updateRecordingStatus'
description: Обновление состояния записи приложения, связанного с вызовом.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 69893f1ff55a080e94ded88722614856c0dcf8c2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047597"
---
# <a name="call-updaterecordingstatus"></a><span data-ttu-id="240ca-103">вызов: updateRecordingStatus</span><span class="sxs-lookup"><span data-stu-id="240ca-103">call: updateRecordingStatus</span></span>

<span data-ttu-id="240ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="240ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="240ca-105">Обновление состояния записи приложения, связанного с вызовом.</span><span class="sxs-lookup"><span data-stu-id="240ca-105">Update the application's recording status associated with a call.</span></span> <span data-ttu-id="240ca-106">Это требует использования решения записи [Teams на основе политики.](/MicrosoftTeams/teams-recording-policy)</span><span class="sxs-lookup"><span data-stu-id="240ca-106">This requires the use of the [Teams policy-based recording](/MicrosoftTeams/teams-recording-policy) solution.</span></span>

> <span data-ttu-id="240ca-107">Дополнительное **ограничение.** Вы не можете использовать API доступа к мультимедиа для записи или иного сохраняемой медиаконтента из звонков или собраний, к которые ваше приложение получает доступ, или данных, полученных из этого медиаконтента ("запись" или "запись"), без вызова API **updateRecordingStatus,** чтобы указать, что запись началась, и получить ответ на успех от этого API.</span><span class="sxs-lookup"><span data-stu-id="240ca-107">**Additional Restriction**: You may NOT use the Media Access API to record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content ("record" or "recording"), without first calling the **updateRecordingStatus** API to indicate that recording has begun, and receiving a success reply from that API.</span></span> <span data-ttu-id="240ca-108">Если ваше приложение начинает записывать любое собрание, оно должно закончить запись перед вызовом **API updateRecordingStatus,** чтобы указать, что запись завершена.</span><span class="sxs-lookup"><span data-stu-id="240ca-108">If your application begins recording any meeting, it must end the recording prior to calling the **updateRecordingStatus** API to indicate that the recording has ended.</span></span>

## <a name="permissions"></a><span data-ttu-id="240ca-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="240ca-109">Permissions</span></span>
<span data-ttu-id="240ca-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="240ca-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="240ca-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="240ca-112">Permission type</span></span>                        | <span data-ttu-id="240ca-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="240ca-113">Permissions (from least to most privileged)</span></span>      |
|:---------------------------------------|:-------------------------------------------------|
| <span data-ttu-id="240ca-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="240ca-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="240ca-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="240ca-115">Not Supported</span></span>                                    |
| <span data-ttu-id="240ca-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="240ca-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="240ca-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="240ca-117">Not Supported</span></span>                                    |
| <span data-ttu-id="240ca-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="240ca-118">Application</span></span>                            | <span data-ttu-id="240ca-119">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="240ca-119">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="240ca-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="240ca-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateRecordingStatus
POST /communications/calls/{id}/updateRecordingStatus
```
> <span data-ttu-id="240ca-121">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="240ca-121">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="240ca-122">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="240ca-122">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="240ca-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="240ca-123">Request headers</span></span>
| <span data-ttu-id="240ca-124">Имя</span><span class="sxs-lookup"><span data-stu-id="240ca-124">Name</span></span>          | <span data-ttu-id="240ca-125">Описание</span><span class="sxs-lookup"><span data-stu-id="240ca-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="240ca-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="240ca-126">Authorization</span></span> | <span data-ttu-id="240ca-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="240ca-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="240ca-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="240ca-129">Content-type</span></span> | <span data-ttu-id="240ca-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="240ca-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="240ca-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="240ca-132">Request body</span></span>
<span data-ttu-id="240ca-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="240ca-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="240ca-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="240ca-134">Parameter</span></span>       | <span data-ttu-id="240ca-135">Тип</span><span class="sxs-lookup"><span data-stu-id="240ca-135">Type</span></span>    | <span data-ttu-id="240ca-136">Описание</span><span class="sxs-lookup"><span data-stu-id="240ca-136">Description</span></span>                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| <span data-ttu-id="240ca-137">clientContext</span><span class="sxs-lookup"><span data-stu-id="240ca-137">clientContext</span></span>   | <span data-ttu-id="240ca-138">String</span><span class="sxs-lookup"><span data-stu-id="240ca-138">String</span></span>  | <span data-ttu-id="240ca-139">Уникальная строка Client Context.</span><span class="sxs-lookup"><span data-stu-id="240ca-139">Unique Client Context string.</span></span> <span data-ttu-id="240ca-140">Максимальное ограничение — 256 шаров.</span><span class="sxs-lookup"><span data-stu-id="240ca-140">Max limit is 256 chars.</span></span>                                 |
| <span data-ttu-id="240ca-141">status</span><span class="sxs-lookup"><span data-stu-id="240ca-141">status</span></span>          | <span data-ttu-id="240ca-142">String</span><span class="sxs-lookup"><span data-stu-id="240ca-142">String</span></span>  | <span data-ttu-id="240ca-143">Состояние записи.</span><span class="sxs-lookup"><span data-stu-id="240ca-143">The recording status.</span></span> <span data-ttu-id="240ca-144">Возможные значения: `notRecording`, `recording` или `failed`.</span><span class="sxs-lookup"><span data-stu-id="240ca-144">Possible values are: `notRecording`, `recording`, or `failed`.</span></span>  |

## <a name="response"></a><span data-ttu-id="240ca-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="240ca-145">Response</span></span>
<span data-ttu-id="240ca-146">Этот метод возвращает код ответа и загорелый загорелый код расположения с URI к объекту `200 OK` [updateRecordingStatusOperation,](../resources/updaterecordingstatusoperation.md) созданному для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="240ca-146">This method returns a `200 OK` response code and a Location header with a URI to the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="240ca-147">Пример</span><span class="sxs-lookup"><span data-stu-id="240ca-147">Example</span></span>
<span data-ttu-id="240ca-148">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="240ca-148">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="240ca-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="240ca-149">Request</span></span>
<span data-ttu-id="240ca-150">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="240ca-150">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="240ca-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="240ca-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-updateRecordingStatus"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/updateRecordingStatus
Content-Type: application/json
Content-Length: 79

{
  "clientContext": "clientContext-value",
  "status": "notRecording | recording | failed"
}
```
# <a name="c"></a>[<span data-ttu-id="240ca-152">C#</span><span class="sxs-lookup"><span data-stu-id="240ca-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updaterecordingstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="240ca-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="240ca-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updaterecordingstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="240ca-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="240ca-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updaterecordingstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="240ca-155">Java</span><span class="sxs-lookup"><span data-stu-id="240ca-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-updaterecordingstatus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="240ca-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="240ca-156">Response</span></span>

> <span data-ttu-id="240ca-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="240ca-157">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "name": "call-updateRecordingStatus",
  "truncated": true,
  "@odata.type": "microsoft.graph.updateRecordingStatusOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

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
