---
title: 'Call: Упдатерекордингстатус'
description: Обновление состояния записи приложения, связанного с вызовом.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 9601c3a4589ba899d76b4ce55c1b0fdf8b3da355
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062583"
---
# <a name="call-updaterecordingstatus"></a><span data-ttu-id="4d1cb-103">Call: Упдатерекордингстатус</span><span class="sxs-lookup"><span data-stu-id="4d1cb-103">call: updateRecordingStatus</span></span>

<span data-ttu-id="4d1cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d1cb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4d1cb-105">Обновление состояния записи приложения, связанного с вызовом.</span><span class="sxs-lookup"><span data-stu-id="4d1cb-105">Update the application's recording status associated with a call.</span></span>

> <span data-ttu-id="4d1cb-106">**Дополнительное ограничение**: вы не можете использовать API-интерфейс для записи или сохранения мультимедийного контента из вызовов или собраний, к которым обращается приложение, или данных, полученных из этого контента ("запись" или "запись"), без предварительного вызова API **упдатерекордингстатус** для указания того, что запись началась и получает ответ об успешной отправке от этого API.</span><span class="sxs-lookup"><span data-stu-id="4d1cb-106">**Additional Restriction**: You may NOT use the Media Access API to record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content ("record" or "recording"), without first calling the **updateRecordingStatus** API to indicate that recording has begun, and receiving a success reply from that API.</span></span> <span data-ttu-id="4d1cb-107">Если приложение начинает запись собрания, оно должно закончить запись перед вызовом API **упдатерекордингстатус** , чтобы указать, что запись закончена.</span><span class="sxs-lookup"><span data-stu-id="4d1cb-107">If your application begins recording any meeting, it must end the recording prior to calling the **updateRecordingStatus** API to indicate that the recording has ended.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d1cb-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d1cb-108">Permissions</span></span>
<span data-ttu-id="4d1cb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d1cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4d1cb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d1cb-111">Permission type</span></span>                        | <span data-ttu-id="4d1cb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d1cb-112">Permissions (from least to most privileged)</span></span>      |
|:---------------------------------------|:-------------------------------------------------|
| <span data-ttu-id="4d1cb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d1cb-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d1cb-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4d1cb-114">Not Supported</span></span>                                    |
| <span data-ttu-id="4d1cb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d1cb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d1cb-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4d1cb-116">Not Supported</span></span>                                    |
| <span data-ttu-id="4d1cb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4d1cb-117">Application</span></span>                            | <span data-ttu-id="4d1cb-118">Calls. Жоинграупкаллс. ALL, Calls. Акцессмедиа. ALL</span><span class="sxs-lookup"><span data-stu-id="4d1cb-118">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4d1cb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d1cb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/updateRecordingStatus
```

## <a name="request-headers"></a><span data-ttu-id="4d1cb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d1cb-120">Request headers</span></span>
| <span data-ttu-id="4d1cb-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4d1cb-121">Name</span></span>          | <span data-ttu-id="4d1cb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4d1cb-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4d1cb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d1cb-123">Authorization</span></span> | <span data-ttu-id="4d1cb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d1cb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4d1cb-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4d1cb-126">Content-type</span></span> | <span data-ttu-id="4d1cb-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d1cb-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d1cb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d1cb-129">Request body</span></span>
<span data-ttu-id="4d1cb-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4d1cb-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4d1cb-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="4d1cb-131">Parameter</span></span>       | <span data-ttu-id="4d1cb-132">Тип</span><span class="sxs-lookup"><span data-stu-id="4d1cb-132">Type</span></span>    | <span data-ttu-id="4d1cb-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4d1cb-133">Description</span></span>                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| <span data-ttu-id="4d1cb-134">Контекст</span><span class="sxs-lookup"><span data-stu-id="4d1cb-134">clientContext</span></span>   | <span data-ttu-id="4d1cb-135">String</span><span class="sxs-lookup"><span data-stu-id="4d1cb-135">String</span></span>  | <span data-ttu-id="4d1cb-136">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="4d1cb-136">Unique client context string.</span></span> <span data-ttu-id="4d1cb-137">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="4d1cb-137">Max limit is 256 chars.</span></span>                                 |
| <span data-ttu-id="4d1cb-138">status</span><span class="sxs-lookup"><span data-stu-id="4d1cb-138">status</span></span>          | <span data-ttu-id="4d1cb-139">String</span><span class="sxs-lookup"><span data-stu-id="4d1cb-139">String</span></span>  | <span data-ttu-id="4d1cb-140">Состояние записи.</span><span class="sxs-lookup"><span data-stu-id="4d1cb-140">The recording status.</span></span> <span data-ttu-id="4d1cb-141">Возможные значения: `notRecording`, `recording`, или. `failed`</span><span class="sxs-lookup"><span data-stu-id="4d1cb-141">Possible values are: `notRecording`, `recording`, or `failed`.</span></span>  |

## <a name="response"></a><span data-ttu-id="4d1cb-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d1cb-142">Response</span></span>
<span data-ttu-id="4d1cb-143">Этот метод возвращает код `200 OK` отклика и заголовок Location с URI для объекта [упдатерекордингстатусоператион](../resources/updaterecordingstatusoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="4d1cb-143">This method returns a `200 OK` response code and a Location header with a URI to the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="4d1cb-144">Пример</span><span class="sxs-lookup"><span data-stu-id="4d1cb-144">Example</span></span>
<span data-ttu-id="4d1cb-145">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="4d1cb-145">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="4d1cb-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d1cb-146">Request</span></span>
<span data-ttu-id="4d1cb-147">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d1cb-147">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4d1cb-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d1cb-148">HTTP</span></span>](#tab/http)
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
---

### <a name="response"></a><span data-ttu-id="4d1cb-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d1cb-149">Response</span></span>

> <span data-ttu-id="4d1cb-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d1cb-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
