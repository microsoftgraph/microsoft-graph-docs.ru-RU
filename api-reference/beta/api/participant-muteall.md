---
title: 'участник: Мутеалл'
description: Отключение звука всех участников звонка.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b1e4555c77a843cfccd420ef0c17a09dba20a383
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636829"
---
# <a name="participant-muteall"></a><span data-ttu-id="b1b89-103">участник: Мутеалл</span><span class="sxs-lookup"><span data-stu-id="b1b89-103">participant: muteAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1b89-104">Отключение звука всех участников звонка.</span><span class="sxs-lookup"><span data-stu-id="b1b89-104">Mute all participants in the call.</span></span>

> <span data-ttu-id="b1b89-105">**Примечание:** Этот API является устаревшим и будет удален 15 марта 2020.</span><span class="sxs-lookup"><span data-stu-id="b1b89-105">**Note:** This API is deprecated and will be removed by March 15th, 2020.</span></span> <span data-ttu-id="b1b89-106">Чтобы отключиться от одного участника, ознакомьтесь со статьей [участник: выкл](participant-mute.md).</span><span class="sxs-lookup"><span data-stu-id="b1b89-106">To mute a single participant, see [participant: mute](participant-mute.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="b1b89-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1b89-107">Permissions</span></span>
<span data-ttu-id="b1b89-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1b89-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b1b89-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1b89-110">Permission type</span></span>                        | <span data-ttu-id="b1b89-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1b89-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b1b89-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1b89-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b1b89-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b1b89-113">Not Supported</span></span>                               |
| <span data-ttu-id="b1b89-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1b89-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1b89-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b1b89-115">Not Supported</span></span>                               |
| <span data-ttu-id="b1b89-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="b1b89-116">Application</span></span>                            | <span data-ttu-id="b1b89-117">Нет</span><span class="sxs-lookup"><span data-stu-id="b1b89-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="b1b89-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1b89-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /communications/calls/{id}/participants/muteAll
```
> <span data-ttu-id="b1b89-119">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="b1b89-119">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="b1b89-120">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="b1b89-120">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1b89-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1b89-121">Request headers</span></span>
| <span data-ttu-id="b1b89-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b1b89-122">Name</span></span>          | <span data-ttu-id="b1b89-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b1b89-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b1b89-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1b89-124">Authorization</span></span> | <span data-ttu-id="b1b89-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1b89-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b1b89-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b1b89-127">Content-type</span></span> | <span data-ttu-id="b1b89-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1b89-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1b89-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1b89-130">Request body</span></span>
<span data-ttu-id="b1b89-131">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b1b89-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b1b89-132">Параметр</span><span class="sxs-lookup"><span data-stu-id="b1b89-132">Parameter</span></span>      | <span data-ttu-id="b1b89-133">Тип</span><span class="sxs-lookup"><span data-stu-id="b1b89-133">Type</span></span>    |<span data-ttu-id="b1b89-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b1b89-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1b89-135">participants</span><span class="sxs-lookup"><span data-stu-id="b1b89-135">participants</span></span>|<span data-ttu-id="b1b89-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b1b89-136">String collection</span></span>|<span data-ttu-id="b1b89-137">Участники, которые должны быть отключены.</span><span class="sxs-lookup"><span data-stu-id="b1b89-137">The participants to be muted.</span></span>|
|<span data-ttu-id="b1b89-138">Контекст</span><span class="sxs-lookup"><span data-stu-id="b1b89-138">clientContext</span></span>|<span data-ttu-id="b1b89-139">String</span><span class="sxs-lookup"><span data-stu-id="b1b89-139">String</span></span>|<span data-ttu-id="b1b89-140">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="b1b89-140">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="b1b89-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1b89-141">Response</span></span>
<span data-ttu-id="b1b89-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [коммсоператион](../resources/commsoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1b89-142">If successful, this method returns a `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1b89-143">Пример</span><span class="sxs-lookup"><span data-stu-id="b1b89-143">Example</span></span>
<span data-ttu-id="b1b89-144">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="b1b89-144">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b1b89-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1b89-145">Request</span></span>
<span data-ttu-id="b1b89-146">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1b89-146">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b1b89-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1b89-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-muteAll"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/participants/muteAll
Content-Type: application/json
Content-Length: 81

{
  "participants": [
    ""
  ],
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b1b89-148">C#</span><span class="sxs-lookup"><span data-stu-id="b1b89-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-muteall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1b89-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1b89-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-muteall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b1b89-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b1b89-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-muteall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b1b89-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1b89-151">Response</span></span>

> <span data-ttu-id="b1b89-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1b89-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "participant-muteAll",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.commsOperation",
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
  "description": "participant: muteAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
