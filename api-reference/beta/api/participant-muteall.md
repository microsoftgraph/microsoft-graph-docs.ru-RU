---
title: 'участник: Мутеалл'
description: Отключение звука всех участников звонка.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7ae154e0a9e211620d9761c9051e73d5b35ec020
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332771"
---
# <a name="participant-muteall"></a><span data-ttu-id="39662-103">участник: Мутеалл</span><span class="sxs-lookup"><span data-stu-id="39662-103">participant: muteAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39662-104">Отключение звука всех участников звонка.</span><span class="sxs-lookup"><span data-stu-id="39662-104">Mute all participants in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="39662-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39662-105">Permissions</span></span>
<span data-ttu-id="39662-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39662-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="39662-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39662-108">Permission type</span></span>                        | <span data-ttu-id="39662-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39662-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="39662-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39662-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="39662-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="39662-111">Not Supported</span></span>                               |
| <span data-ttu-id="39662-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39662-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39662-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="39662-113">Not Supported</span></span>                               |
| <span data-ttu-id="39662-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39662-114">Application</span></span>                            | <span data-ttu-id="39662-115">Нет</span><span class="sxs-lookup"><span data-stu-id="39662-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="39662-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39662-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /applications/{id}/calls/{id}/participants/muteAll
```

## <a name="request-headers"></a><span data-ttu-id="39662-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39662-117">Request headers</span></span>
| <span data-ttu-id="39662-118">Имя</span><span class="sxs-lookup"><span data-stu-id="39662-118">Name</span></span>          | <span data-ttu-id="39662-119">Описание</span><span class="sxs-lookup"><span data-stu-id="39662-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="39662-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39662-120">Authorization</span></span> | <span data-ttu-id="39662-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39662-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39662-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39662-123">Request body</span></span>
<span data-ttu-id="39662-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="39662-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="39662-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="39662-125">Parameter</span></span>      | <span data-ttu-id="39662-126">Тип</span><span class="sxs-lookup"><span data-stu-id="39662-126">Type</span></span>    |<span data-ttu-id="39662-127">Описание</span><span class="sxs-lookup"><span data-stu-id="39662-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39662-128">participants</span><span class="sxs-lookup"><span data-stu-id="39662-128">participants</span></span>|<span data-ttu-id="39662-129">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="39662-129">String collection</span></span>|<span data-ttu-id="39662-130">Участники, которые должны быть отключены.</span><span class="sxs-lookup"><span data-stu-id="39662-130">The participants to be muted.</span></span>|
|<span data-ttu-id="39662-131">Контекст</span><span class="sxs-lookup"><span data-stu-id="39662-131">clientContext</span></span>|<span data-ttu-id="39662-132">String</span><span class="sxs-lookup"><span data-stu-id="39662-132">String</span></span>|<span data-ttu-id="39662-133">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="39662-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="39662-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="39662-134">Response</span></span>
<span data-ttu-id="39662-135">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и объект [коммсоператион](../resources/commsoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="39662-135">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39662-136">Пример</span><span class="sxs-lookup"><span data-stu-id="39662-136">Example</span></span>
<span data-ttu-id="39662-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="39662-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="39662-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="39662-138">Request</span></span>
<span data-ttu-id="39662-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39662-139">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "participant-muteAll"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/muteAll
Content-Type: application/json
Content-Length: 81

{
  "participants": [
    ""
  ],
  "clientContext": "clientContext-value"
}
```

##### <a name="response"></a><span data-ttu-id="39662-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="39662-140">Response</span></span>

> <span data-ttu-id="39662-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39662-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
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
  "suppressions": []
}
-->
