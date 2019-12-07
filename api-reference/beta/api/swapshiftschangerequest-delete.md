---
title: Удаление Свапшифтсчанжерекуест
description: Удаление объекта Свапшифтсчанжерекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 843226c6cd1109a87919790a004ad52b0351b753
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895820"
---
# <a name="delete-swapshiftschangerequest"></a><span data-ttu-id="c7ca9-103">Удаление Свапшифтсчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="c7ca9-103">Delete swapShiftsChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7ca9-104">Удаление объекта [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="c7ca9-104">Delete a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7ca9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7ca9-105">Permissions</span></span>

<span data-ttu-id="c7ca9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7ca9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c7ca9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7ca9-108">Permission type</span></span>                        | <span data-ttu-id="c7ca9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7ca9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c7ca9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7ca9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7ca9-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7ca9-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="c7ca9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7ca9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7ca9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-113">Not supported.</span></span> |
| <span data-ttu-id="c7ca9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7ca9-114">Application</span></span>                            | <span data-ttu-id="c7ca9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7ca9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7ca9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/swapShiftsChangeRequests
```

## <a name="request-headers"></a><span data-ttu-id="c7ca9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7ca9-117">Request headers</span></span>

| <span data-ttu-id="c7ca9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c7ca9-118">Name</span></span>          | <span data-ttu-id="c7ca9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c7ca9-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c7ca9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7ca9-120">Authorization</span></span> | <span data-ttu-id="c7ca9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7ca9-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7ca9-123">Request body</span></span>

<span data-ttu-id="c7ca9-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7ca9-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7ca9-125">Response</span></span>

<span data-ttu-id="c7ca9-p103">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c7ca9-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="c7ca9-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c7ca9-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7ca9-129">Request</span></span>

<span data-ttu-id="c7ca9-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_swapshiftschangerequest"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/schedule/swapShiftsChangeRequests
```

### <a name="response"></a><span data-ttu-id="c7ca9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7ca9-131">Response</span></span>

<span data-ttu-id="c7ca9-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c7ca9-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete swapShiftsChangeRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
