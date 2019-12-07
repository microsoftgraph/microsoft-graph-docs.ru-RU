---
title: Удаление Тимеоффрекуест
description: Удаление объекта Тимеоффрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 289d438f8bf1685445b1dc2c5c95ff2b7233f4d7
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895799"
---
# <a name="delete-timeoffrequest"></a><span data-ttu-id="bfb3a-103">Удаление Тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="bfb3a-103">Delete timeOffRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfb3a-104">Удаление объекта [тимеоффрекуест](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="bfb3a-104">Delete a [timeOffRequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bfb3a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bfb3a-105">Permissions</span></span>

<span data-ttu-id="bfb3a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfb3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bfb3a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bfb3a-108">Permission type</span></span>                        | <span data-ttu-id="bfb3a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bfb3a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bfb3a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bfb3a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bfb3a-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfb3a-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="bfb3a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bfb3a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfb3a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfb3a-113">Not supported.</span></span> |
| <span data-ttu-id="bfb3a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bfb3a-114">Application</span></span>                            | <span data-ttu-id="bfb3a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfb3a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfb3a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfb3a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{id}/schedule/timeOffRequests
```

## <a name="request-headers"></a><span data-ttu-id="bfb3a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bfb3a-117">Request headers</span></span>

| <span data-ttu-id="bfb3a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bfb3a-118">Name</span></span>          | <span data-ttu-id="bfb3a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bfb3a-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bfb3a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bfb3a-120">Authorization</span></span> | <span data-ttu-id="bfb3a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bfb3a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfb3a-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bfb3a-123">Request body</span></span>

<span data-ttu-id="bfb3a-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bfb3a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfb3a-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfb3a-125">Response</span></span>

<span data-ttu-id="bfb3a-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bfb3a-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bfb3a-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="bfb3a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bfb3a-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="bfb3a-129">Request</span></span>

<span data-ttu-id="bfb3a-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bfb3a-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_timeoffrequest"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{id}/schedule/timeOffRequests
```

### <a name="response"></a><span data-ttu-id="bfb3a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfb3a-131">Response</span></span>

<span data-ttu-id="bfb3a-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bfb3a-132">The following is an example of the response.</span></span>

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
  "description": "Delete timeOffRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
