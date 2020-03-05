---
title: 'Call: Упдатерекордингстатус'
description: Обновление состояния записи приложения, связанного с вызовом.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7a86276b42244b6fc1443d07d5170175f7166a92
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440684"
---
# <a name="call-updaterecordingstatus"></a><span data-ttu-id="5b28a-103">Call: Упдатерекордингстатус</span><span class="sxs-lookup"><span data-stu-id="5b28a-103">call: updateRecordingStatus</span></span>

<span data-ttu-id="5b28a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5b28a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b28a-105">Обновление состояния записи приложения, связанного с вызовом.</span><span class="sxs-lookup"><span data-stu-id="5b28a-105">Update the application's recording status associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b28a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b28a-106">Permissions</span></span>
<span data-ttu-id="5b28a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b28a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b28a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b28a-109">Permission type</span></span>                        | <span data-ttu-id="5b28a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b28a-110">Permissions (from least to most privileged)</span></span>      |
|:---------------------------------------|:-------------------------------------------------|
| <span data-ttu-id="5b28a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b28a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b28a-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b28a-112">Not Supported</span></span>                                    |
| <span data-ttu-id="5b28a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b28a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b28a-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5b28a-114">Not Supported</span></span>                                    |
| <span data-ttu-id="5b28a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b28a-115">Application</span></span>                            | <span data-ttu-id="5b28a-116">Calls. Жоинграупкаллс. ALL, Calls. Акцессмедиа. ALL</span><span class="sxs-lookup"><span data-stu-id="5b28a-116">Calls.JoinGroupCalls.All, Calls.AccessMedia.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5b28a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b28a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateRecordingStatus
POST /communications/calls/{id}/updateRecordingStatus
```
> <span data-ttu-id="5b28a-118">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="5b28a-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="5b28a-119">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="5b28a-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b28a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b28a-120">Request headers</span></span>
| <span data-ttu-id="5b28a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5b28a-121">Name</span></span>          | <span data-ttu-id="5b28a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5b28a-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5b28a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b28a-123">Authorization</span></span> | <span data-ttu-id="5b28a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b28a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5b28a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b28a-126">Content-type</span></span> | <span data-ttu-id="5b28a-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b28a-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b28a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b28a-129">Request body</span></span>
<span data-ttu-id="5b28a-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5b28a-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5b28a-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="5b28a-131">Parameter</span></span>       | <span data-ttu-id="5b28a-132">Тип</span><span class="sxs-lookup"><span data-stu-id="5b28a-132">Type</span></span>    | <span data-ttu-id="5b28a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="5b28a-133">Description</span></span>                                                                           |
|:----------------|:--------|:--------------------------------------------------------------------------------------|
| <span data-ttu-id="5b28a-134">Контекст</span><span class="sxs-lookup"><span data-stu-id="5b28a-134">clientContext</span></span>   | <span data-ttu-id="5b28a-135">String</span><span class="sxs-lookup"><span data-stu-id="5b28a-135">String</span></span>  | <span data-ttu-id="5b28a-136">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="5b28a-136">Unique Client Context string.</span></span> <span data-ttu-id="5b28a-137">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="5b28a-137">Max limit is 256 chars.</span></span>                                 |
| <span data-ttu-id="5b28a-138">status</span><span class="sxs-lookup"><span data-stu-id="5b28a-138">status</span></span>          | <span data-ttu-id="5b28a-139">String</span><span class="sxs-lookup"><span data-stu-id="5b28a-139">String</span></span>  | <span data-ttu-id="5b28a-140">Состояние записи.</span><span class="sxs-lookup"><span data-stu-id="5b28a-140">The recording status.</span></span> <span data-ttu-id="5b28a-141">Возможные значения: `notRecording`, `recording`, или. `failed`</span><span class="sxs-lookup"><span data-stu-id="5b28a-141">Possible values are: `notRecording`, `recording`, or `failed`.</span></span>  |

## <a name="response"></a><span data-ttu-id="5b28a-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b28a-142">Response</span></span>
<span data-ttu-id="5b28a-143">Этот метод возвращает код `200 OK` отклика и заголовок Location с URI для объекта [упдатерекордингстатусоператион](../resources/updaterecordingstatusoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="5b28a-143">This method returns a `200 OK` response code and a Location header with a URI to the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="5b28a-144">Пример</span><span class="sxs-lookup"><span data-stu-id="5b28a-144">Example</span></span>
<span data-ttu-id="5b28a-145">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="5b28a-145">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="5b28a-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b28a-146">Request</span></span>
<span data-ttu-id="5b28a-147">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b28a-147">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5b28a-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b28a-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5b28a-149">C#</span><span class="sxs-lookup"><span data-stu-id="5b28a-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updaterecordingstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b28a-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b28a-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updaterecordingstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b28a-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b28a-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updaterecordingstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5b28a-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b28a-152">Response</span></span>

> <span data-ttu-id="5b28a-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b28a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
