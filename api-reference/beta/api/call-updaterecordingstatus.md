---
title: 'Call: Упдатерекордингстатус'
description: Обновление состояния записи приложения, связанного с вызовом.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7de436ecdb24a7288cf515c71598b880ec4122dc
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912736"
---
# <a name="call-updaterecordingstatus"></a><span data-ttu-id="3411b-103">Call: Упдатерекордингстатус</span><span class="sxs-lookup"><span data-stu-id="3411b-103">call: updateRecordingStatus</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3411b-104">Обновление состояния записи приложения, связанного с вызовом.</span><span class="sxs-lookup"><span data-stu-id="3411b-104">Update the application's recording status associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="3411b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3411b-105">Permissions</span></span>
<span data-ttu-id="3411b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3411b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3411b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3411b-108">Permission type</span></span>                        | <span data-ttu-id="3411b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3411b-109">Permissions (from least to most privileged)</span></span>      |
|:---------------------------------------|:-------------------------------------------------|
| <span data-ttu-id="3411b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3411b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3411b-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3411b-111">Not Supported</span></span>                                    |
| <span data-ttu-id="3411b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3411b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3411b-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3411b-113">Not Supported</span></span>                                    |
| <span data-ttu-id="3411b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3411b-114">Application</span></span>                            | <span data-ttu-id="3411b-115">Calls. Жоинграупкаллс. ALL, Calls. Акцессмедиа. ALL</span><span class="sxs-lookup"><span data-stu-id="3411b-115">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3411b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3411b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateRecordingStatus
POST /communications/calls/{id}/updateRecordingStatus
```
> <span data-ttu-id="3411b-117">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="3411b-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="3411b-118">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="3411b-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3411b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3411b-119">Request headers</span></span>
| <span data-ttu-id="3411b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3411b-120">Name</span></span>          | <span data-ttu-id="3411b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3411b-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3411b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3411b-122">Authorization</span></span> | <span data-ttu-id="3411b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3411b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3411b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3411b-125">Content-type</span></span> | <span data-ttu-id="3411b-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3411b-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3411b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3411b-128">Request body</span></span>
<span data-ttu-id="3411b-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3411b-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3411b-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="3411b-130">Parameter</span></span>       | <span data-ttu-id="3411b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3411b-131">Type</span></span>    | <span data-ttu-id="3411b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3411b-132">Description</span></span>                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| <span data-ttu-id="3411b-133">Контекст</span><span class="sxs-lookup"><span data-stu-id="3411b-133">clientContext</span></span>   | <span data-ttu-id="3411b-134">String</span><span class="sxs-lookup"><span data-stu-id="3411b-134">String</span></span>  | <span data-ttu-id="3411b-135">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="3411b-135">Unique Client Context string.</span></span> <span data-ttu-id="3411b-136">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="3411b-136">Max limit is 256 chars.</span></span>                                 |
| <span data-ttu-id="3411b-137">status</span><span class="sxs-lookup"><span data-stu-id="3411b-137">status</span></span>          | <span data-ttu-id="3411b-138">String</span><span class="sxs-lookup"><span data-stu-id="3411b-138">String</span></span>  | <span data-ttu-id="3411b-139">Состояние записи.</span><span class="sxs-lookup"><span data-stu-id="3411b-139">The recording status.</span></span> <span data-ttu-id="3411b-140">Возможные значения: `notRecording`, `recording`, или. `failed`</span><span class="sxs-lookup"><span data-stu-id="3411b-140">Possible values are: `notRecording`, `recording`, or `failed`.</span></span>  |

## <a name="response"></a><span data-ttu-id="3411b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3411b-141">Response</span></span>
<span data-ttu-id="3411b-142">Этот метод возвращает код `200 OK` отклика и заголовок Location с URI для объекта [упдатерекордингстатусоператион](../resources/updaterecordingstatusoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="3411b-142">This method returns a `200 OK` response code and a Location header with a URI to the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="3411b-143">Пример</span><span class="sxs-lookup"><span data-stu-id="3411b-143">Example</span></span>
<span data-ttu-id="3411b-144">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="3411b-144">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="3411b-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="3411b-145">Request</span></span>
<span data-ttu-id="3411b-146">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3411b-146">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3411b-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="3411b-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="3411b-148">C#</span><span class="sxs-lookup"><span data-stu-id="3411b-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updaterecordingstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3411b-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3411b-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updaterecordingstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3411b-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3411b-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updaterecordingstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3411b-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="3411b-151">Response</span></span>

> <span data-ttu-id="3411b-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3411b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
