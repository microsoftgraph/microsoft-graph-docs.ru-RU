---
title: 'Call: Упдатерекордингстатус'
description: Обновление состояния записи приложения, связанного с вызовом.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 90f550d50361d3e8ad1b0fd590cbad3e291d7b96
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636871"
---
# <a name="call-updaterecordingstatus"></a><span data-ttu-id="c850e-103">Call: Упдатерекордингстатус</span><span class="sxs-lookup"><span data-stu-id="c850e-103">call: updateRecordingStatus</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c850e-104">Обновление состояния записи приложения, связанного с вызовом.</span><span class="sxs-lookup"><span data-stu-id="c850e-104">Update the application's recording status associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="c850e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c850e-105">Permissions</span></span>
<span data-ttu-id="c850e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c850e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c850e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c850e-108">Permission type</span></span>                        | <span data-ttu-id="c850e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c850e-109">Permissions (from least to most privileged)</span></span>      |
|:---------------------------------------|:-------------------------------------------------|
| <span data-ttu-id="c850e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c850e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c850e-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c850e-111">Not Supported</span></span>                                    |
| <span data-ttu-id="c850e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c850e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c850e-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c850e-113">Not Supported</span></span>                                    |
| <span data-ttu-id="c850e-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="c850e-114">Application</span></span>                            | <span data-ttu-id="c850e-115">Calls. Жоинграупкаллс. ALL, Calls. Акцессмедиа. ALL</span><span class="sxs-lookup"><span data-stu-id="c850e-115">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c850e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c850e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateRecordingStatus
POST /communications/calls/{id}/updateRecordingStatus
```
> <span data-ttu-id="c850e-117">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="c850e-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="c850e-118">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="c850e-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c850e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c850e-119">Request headers</span></span>
| <span data-ttu-id="c850e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c850e-120">Name</span></span>          | <span data-ttu-id="c850e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c850e-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c850e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c850e-122">Authorization</span></span> | <span data-ttu-id="c850e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c850e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c850e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c850e-125">Content-type</span></span> | <span data-ttu-id="c850e-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c850e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c850e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c850e-128">Request body</span></span>
<span data-ttu-id="c850e-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c850e-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c850e-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="c850e-130">Parameter</span></span>       | <span data-ttu-id="c850e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c850e-131">Type</span></span>    | <span data-ttu-id="c850e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c850e-132">Description</span></span>                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| <span data-ttu-id="c850e-133">Контекст</span><span class="sxs-lookup"><span data-stu-id="c850e-133">clientContext</span></span>   | <span data-ttu-id="c850e-134">String</span><span class="sxs-lookup"><span data-stu-id="c850e-134">String</span></span>  | <span data-ttu-id="c850e-135">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="c850e-135">Unique Client Context string.</span></span> <span data-ttu-id="c850e-136">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="c850e-136">Max limit is 256 chars.</span></span>                                 |
| <span data-ttu-id="c850e-137">status</span><span class="sxs-lookup"><span data-stu-id="c850e-137">status</span></span>          | <span data-ttu-id="c850e-138">String</span><span class="sxs-lookup"><span data-stu-id="c850e-138">String</span></span>  | <span data-ttu-id="c850e-139">Состояние записи.</span><span class="sxs-lookup"><span data-stu-id="c850e-139">The recording status.</span></span> <span data-ttu-id="c850e-140">Возможные значения: `notRecording`, `recording`, или. `failed`</span><span class="sxs-lookup"><span data-stu-id="c850e-140">Possible values are: `notRecording`, `recording`, or `failed`.</span></span>  |

## <a name="response"></a><span data-ttu-id="c850e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c850e-141">Response</span></span>
<span data-ttu-id="c850e-142">Этот метод возвращает код `200 OK` отклика и заголовок Location с URI для объекта [упдатерекордингстатусоператион](../resources/updaterecordingstatusoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="c850e-142">This method returns a `200 OK` response code and a Location header with a URI to the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="c850e-143">Пример</span><span class="sxs-lookup"><span data-stu-id="c850e-143">Example</span></span>
<span data-ttu-id="c850e-144">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="c850e-144">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c850e-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="c850e-145">Request</span></span>
<span data-ttu-id="c850e-146">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c850e-146">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c850e-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="c850e-147">HTTP</span></span>](#tab/http)
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

---


### <a name="response"></a><span data-ttu-id="c850e-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="c850e-148">Response</span></span>

> <span data-ttu-id="c850e-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c850e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
