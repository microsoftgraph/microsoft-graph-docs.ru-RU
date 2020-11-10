---
title: 'участник: Мутеалл'
description: Отключение звука всех участников звонка.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 945619d406baf5552581559397c79dcf13bc61cf
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968735"
---
# <a name="participant-muteall"></a><span data-ttu-id="8fbb4-103">участник: Мутеалл</span><span class="sxs-lookup"><span data-stu-id="8fbb4-103">participant: muteAll</span></span>

<span data-ttu-id="8fbb4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fbb4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fbb4-105">Отключение звука всех участников звонка.</span><span class="sxs-lookup"><span data-stu-id="8fbb4-105">Mute all participants in the call.</span></span>

> <span data-ttu-id="8fbb4-106">**Примечание:** Этот API является устаревшим и будет удален 15 марта 2020.</span><span class="sxs-lookup"><span data-stu-id="8fbb4-106">**Note:** This API is deprecated and will be removed by March 15th, 2020.</span></span> <span data-ttu-id="8fbb4-107">Чтобы отключиться от одного участника, ознакомьтесь со статьей [участник: выкл](participant-mute.md).</span><span class="sxs-lookup"><span data-stu-id="8fbb4-107">To mute a single participant, see [participant: mute](participant-mute.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="8fbb4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8fbb4-108">Permissions</span></span>
<span data-ttu-id="8fbb4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fbb4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8fbb4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8fbb4-111">Permission type</span></span>                        | <span data-ttu-id="8fbb4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8fbb4-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8fbb4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8fbb4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8fbb4-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8fbb4-114">Not Supported</span></span>                               |
| <span data-ttu-id="8fbb4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8fbb4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fbb4-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8fbb4-116">Not Supported</span></span>                               |
| <span data-ttu-id="8fbb4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8fbb4-117">Application</span></span>                            | <span data-ttu-id="8fbb4-118">Нет</span><span class="sxs-lookup"><span data-stu-id="8fbb4-118">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="8fbb4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8fbb4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /communications/calls/{id}/participants/muteAll
```
> <span data-ttu-id="8fbb4-120">**Примечание.** Путь `/app` является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="8fbb4-120">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="8fbb4-121">В дальнейшем используйте путь `/communications`.</span><span class="sxs-lookup"><span data-stu-id="8fbb4-121">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8fbb4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8fbb4-122">Request headers</span></span>
| <span data-ttu-id="8fbb4-123">Имя</span><span class="sxs-lookup"><span data-stu-id="8fbb4-123">Name</span></span>          | <span data-ttu-id="8fbb4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8fbb4-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8fbb4-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8fbb4-125">Authorization</span></span> | <span data-ttu-id="8fbb4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8fbb4-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8fbb4-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8fbb4-128">Content-type</span></span> | <span data-ttu-id="8fbb4-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8fbb4-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8fbb4-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8fbb4-131">Request body</span></span>
<span data-ttu-id="8fbb4-132">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8fbb4-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8fbb4-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="8fbb4-133">Parameter</span></span>      | <span data-ttu-id="8fbb4-134">Тип</span><span class="sxs-lookup"><span data-stu-id="8fbb4-134">Type</span></span>    |<span data-ttu-id="8fbb4-135">Описание</span><span class="sxs-lookup"><span data-stu-id="8fbb4-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8fbb4-136">participants</span><span class="sxs-lookup"><span data-stu-id="8fbb4-136">participants</span></span>|<span data-ttu-id="8fbb4-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8fbb4-137">String collection</span></span>|<span data-ttu-id="8fbb4-138">Участники, которые должны быть отключены.</span><span class="sxs-lookup"><span data-stu-id="8fbb4-138">The participants to be muted.</span></span>|
|<span data-ttu-id="8fbb4-139">Контекст</span><span class="sxs-lookup"><span data-stu-id="8fbb4-139">clientContext</span></span>|<span data-ttu-id="8fbb4-140">String</span><span class="sxs-lookup"><span data-stu-id="8fbb4-140">String</span></span>|<span data-ttu-id="8fbb4-141">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="8fbb4-141">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="8fbb4-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fbb4-142">Response</span></span>
<span data-ttu-id="8fbb4-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [коммсоператион](../resources/commsoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8fbb4-143">If successful, this method returns a `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fbb4-144">Пример</span><span class="sxs-lookup"><span data-stu-id="8fbb4-144">Example</span></span>
<span data-ttu-id="8fbb4-145">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="8fbb4-145">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8fbb4-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="8fbb4-146">Request</span></span>
<span data-ttu-id="8fbb4-147">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8fbb4-147">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8fbb4-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="8fbb4-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8fbb4-149">C#</span><span class="sxs-lookup"><span data-stu-id="8fbb4-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-muteall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8fbb4-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8fbb4-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-muteall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8fbb4-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8fbb4-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-muteall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8fbb4-152">Java</span><span class="sxs-lookup"><span data-stu-id="8fbb4-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-muteall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8fbb4-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fbb4-153">Response</span></span>

> <span data-ttu-id="8fbb4-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8fbb4-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


