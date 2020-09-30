---
title: 'Call: Упдатерекордингстатус'
description: Обновление состояния записи приложения, связанного с вызовом.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: d92ba7e1774e41110ea8e1120dd616d24098971c
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313298"
---
# <a name="call-updaterecordingstatus"></a><span data-ttu-id="4f21c-103">Call: Упдатерекордингстатус</span><span class="sxs-lookup"><span data-stu-id="4f21c-103">call: updateRecordingStatus</span></span>

<span data-ttu-id="4f21c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f21c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f21c-105">Обновление состояния записи приложения, связанного с вызовом.</span><span class="sxs-lookup"><span data-stu-id="4f21c-105">Update the application's recording status associated with a call.</span></span> <span data-ttu-id="4f21c-106">Для этого необходимо использовать решение для [записи на основе политики Teams](/MicrosoftTeams/teams-recording-policy) .</span><span class="sxs-lookup"><span data-stu-id="4f21c-106">This requires the use of the [Teams policy-based recording](/MicrosoftTeams/teams-recording-policy) solution.</span></span>

> <span data-ttu-id="4f21c-107">**Дополнительное ограничение**: вы не можете использовать API-интерфейс для записи или сохранения мультимедийного контента из вызовов или собраний, к которым обращается приложение, или данных, полученных из этого контента ("запись" или "запись"), без предварительного вызова API **упдатерекордингстатус** для указания того, что запись началась и получает ответ об успешной отправке от этого API.</span><span class="sxs-lookup"><span data-stu-id="4f21c-107">**Additional Restriction**: You may NOT use the Media Access API to record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content ("record" or "recording"), without first calling the **updateRecordingStatus** API to indicate that recording has begun, and receiving a success reply from that API.</span></span> <span data-ttu-id="4f21c-108">Если приложение начинает запись собрания, оно должно закончить запись перед вызовом API **упдатерекордингстатус** , чтобы указать, что запись закончена.</span><span class="sxs-lookup"><span data-stu-id="4f21c-108">If your application begins recording any meeting, it must end the recording prior to calling the **updateRecordingStatus** API to indicate that the recording has ended.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f21c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f21c-109">Permissions</span></span>
<span data-ttu-id="4f21c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f21c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f21c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f21c-112">Permission type</span></span>                        | <span data-ttu-id="4f21c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f21c-113">Permissions (from least to most privileged)</span></span>      |
|:---------------------------------------|:-------------------------------------------------|
| <span data-ttu-id="4f21c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f21c-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f21c-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f21c-115">Not Supported</span></span>                                    |
| <span data-ttu-id="4f21c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f21c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f21c-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f21c-117">Not Supported</span></span>                                    |
| <span data-ttu-id="4f21c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f21c-118">Application</span></span>                            | <span data-ttu-id="4f21c-119">Calls. Жоинграупкаллс. ALL, Calls. Акцессмедиа. ALL</span><span class="sxs-lookup"><span data-stu-id="4f21c-119">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4f21c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f21c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateRecordingStatus
POST /communications/calls/{id}/updateRecordingStatus
```
> <span data-ttu-id="4f21c-121">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="4f21c-121">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="4f21c-122">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="4f21c-122">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f21c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f21c-123">Request headers</span></span>
| <span data-ttu-id="4f21c-124">Имя</span><span class="sxs-lookup"><span data-stu-id="4f21c-124">Name</span></span>          | <span data-ttu-id="4f21c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="4f21c-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4f21c-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f21c-126">Authorization</span></span> | <span data-ttu-id="4f21c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f21c-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4f21c-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4f21c-129">Content-type</span></span> | <span data-ttu-id="4f21c-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f21c-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f21c-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f21c-132">Request body</span></span>
<span data-ttu-id="4f21c-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4f21c-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4f21c-134">Параметр</span><span class="sxs-lookup"><span data-stu-id="4f21c-134">Parameter</span></span>       | <span data-ttu-id="4f21c-135">Тип</span><span class="sxs-lookup"><span data-stu-id="4f21c-135">Type</span></span>    | <span data-ttu-id="4f21c-136">Описание</span><span class="sxs-lookup"><span data-stu-id="4f21c-136">Description</span></span>                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| <span data-ttu-id="4f21c-137">Контекст</span><span class="sxs-lookup"><span data-stu-id="4f21c-137">clientContext</span></span>   | <span data-ttu-id="4f21c-138">String</span><span class="sxs-lookup"><span data-stu-id="4f21c-138">String</span></span>  | <span data-ttu-id="4f21c-139">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="4f21c-139">Unique Client Context string.</span></span> <span data-ttu-id="4f21c-140">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="4f21c-140">Max limit is 256 chars.</span></span>                                 |
| <span data-ttu-id="4f21c-141">status</span><span class="sxs-lookup"><span data-stu-id="4f21c-141">status</span></span>          | <span data-ttu-id="4f21c-142">String</span><span class="sxs-lookup"><span data-stu-id="4f21c-142">String</span></span>  | <span data-ttu-id="4f21c-143">Состояние записи.</span><span class="sxs-lookup"><span data-stu-id="4f21c-143">The recording status.</span></span> <span data-ttu-id="4f21c-144">Возможные значения: `notRecording` , `recording` , или `failed` .</span><span class="sxs-lookup"><span data-stu-id="4f21c-144">Possible values are: `notRecording`, `recording`, or `failed`.</span></span>  |

## <a name="response"></a><span data-ttu-id="4f21c-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f21c-145">Response</span></span>
<span data-ttu-id="4f21c-146">Этот метод возвращает `200 OK` код отклика и заголовок Location с URI для объекта [упдатерекордингстатусоператион](../resources/updaterecordingstatusoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="4f21c-146">This method returns a `200 OK` response code and a Location header with a URI to the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="4f21c-147">Пример</span><span class="sxs-lookup"><span data-stu-id="4f21c-147">Example</span></span>
<span data-ttu-id="4f21c-148">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="4f21c-148">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="4f21c-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f21c-149">Request</span></span>
<span data-ttu-id="4f21c-150">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f21c-150">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4f21c-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f21c-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4f21c-152">C#</span><span class="sxs-lookup"><span data-stu-id="4f21c-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updaterecordingstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f21c-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f21c-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updaterecordingstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f21c-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f21c-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updaterecordingstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4f21c-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f21c-155">Response</span></span>

> <span data-ttu-id="4f21c-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f21c-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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