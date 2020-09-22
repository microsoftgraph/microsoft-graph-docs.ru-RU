---
title: 'участник: Мутеалл'
description: Отключение звука всех участников звонка.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 0842ebbf4710c964a1ee35e3d63b0f8a0311cb90
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040349"
---
# <a name="participant-muteall"></a><span data-ttu-id="780af-103">участник: Мутеалл</span><span class="sxs-lookup"><span data-stu-id="780af-103">participant: muteAll</span></span>

<span data-ttu-id="780af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="780af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="780af-105">Отключение звука всех участников звонка.</span><span class="sxs-lookup"><span data-stu-id="780af-105">Mute all participants in the call.</span></span>

> <span data-ttu-id="780af-106">**Примечание:** Этот API является устаревшим и будет удален 15 марта 2020.</span><span class="sxs-lookup"><span data-stu-id="780af-106">**Note:** This API is deprecated and will be removed by March 15th, 2020.</span></span> <span data-ttu-id="780af-107">Чтобы отключиться от одного участника, ознакомьтесь со статьей [участник: выкл](participant-mute.md).</span><span class="sxs-lookup"><span data-stu-id="780af-107">To mute a single participant, see [participant: mute](participant-mute.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="780af-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="780af-108">Permissions</span></span>
<span data-ttu-id="780af-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="780af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="780af-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="780af-111">Permission type</span></span>                        | <span data-ttu-id="780af-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="780af-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="780af-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="780af-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="780af-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="780af-114">Not Supported</span></span>                               |
| <span data-ttu-id="780af-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="780af-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="780af-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="780af-116">Not Supported</span></span>                               |
| <span data-ttu-id="780af-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="780af-117">Application</span></span>                            | <span data-ttu-id="780af-118">Нет</span><span class="sxs-lookup"><span data-stu-id="780af-118">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="780af-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="780af-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /communications/calls/{id}/participants/muteAll
```
> <span data-ttu-id="780af-120">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="780af-120">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="780af-121">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="780af-121">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="780af-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="780af-122">Request headers</span></span>
| <span data-ttu-id="780af-123">Имя</span><span class="sxs-lookup"><span data-stu-id="780af-123">Name</span></span>          | <span data-ttu-id="780af-124">Описание</span><span class="sxs-lookup"><span data-stu-id="780af-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="780af-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="780af-125">Authorization</span></span> | <span data-ttu-id="780af-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="780af-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="780af-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="780af-128">Content-type</span></span> | <span data-ttu-id="780af-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="780af-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="780af-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="780af-131">Request body</span></span>
<span data-ttu-id="780af-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="780af-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="780af-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="780af-133">Parameter</span></span>      | <span data-ttu-id="780af-134">Тип</span><span class="sxs-lookup"><span data-stu-id="780af-134">Type</span></span>    |<span data-ttu-id="780af-135">Описание</span><span class="sxs-lookup"><span data-stu-id="780af-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="780af-136">participants</span><span class="sxs-lookup"><span data-stu-id="780af-136">participants</span></span>|<span data-ttu-id="780af-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="780af-137">String collection</span></span>|<span data-ttu-id="780af-138">Участники, которые должны быть отключены.</span><span class="sxs-lookup"><span data-stu-id="780af-138">The participants to be muted.</span></span>|
|<span data-ttu-id="780af-139">Контекст</span><span class="sxs-lookup"><span data-stu-id="780af-139">clientContext</span></span>|<span data-ttu-id="780af-140">String</span><span class="sxs-lookup"><span data-stu-id="780af-140">String</span></span>|<span data-ttu-id="780af-141">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="780af-141">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="780af-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="780af-142">Response</span></span>
<span data-ttu-id="780af-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [коммсоператион](../resources/commsoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="780af-143">If successful, this method returns a `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="780af-144">Пример</span><span class="sxs-lookup"><span data-stu-id="780af-144">Example</span></span>
<span data-ttu-id="780af-145">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="780af-145">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="780af-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="780af-146">Request</span></span>
<span data-ttu-id="780af-147">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="780af-147">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="780af-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="780af-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="780af-149">C#</span><span class="sxs-lookup"><span data-stu-id="780af-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-muteall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="780af-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="780af-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-muteall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="780af-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="780af-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-muteall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="780af-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="780af-152">Response</span></span>

> <span data-ttu-id="780af-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="780af-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


