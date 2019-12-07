---
title: Удаление Воркфорцеинтегратион
description: Удаление экземпляра объекта Воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 01e690c517e0f8b84b1f059ba153d4bb9de7026e
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895802"
---
# <a name="delete-workforceintegration"></a><span data-ttu-id="3f1b9-103">Удаление Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="3f1b9-103">Delete workforceIntegration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f1b9-104">Удаление экземпляра объекта [воркфорцеинтегратион](../resources/workforceintegration.md).</span><span class="sxs-lookup"><span data-stu-id="3f1b9-104">Delete an instance of a [workforceIntegration](../resources/workforceintegration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3f1b9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3f1b9-105">Permissions</span></span>

<span data-ttu-id="3f1b9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f1b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3f1b9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f1b9-108">Permission type</span></span>                        | <span data-ttu-id="3f1b9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f1b9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3f1b9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f1b9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3f1b9-111">Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3f1b9-111">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="3f1b9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f1b9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f1b9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-113">Not supported.</span></span> |
| <span data-ttu-id="3f1b9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f1b9-114">Application</span></span>                            | <span data-ttu-id="3f1b9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f1b9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f1b9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="3f1b9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f1b9-117">Request headers</span></span>

| <span data-ttu-id="3f1b9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3f1b9-118">Name</span></span>          | <span data-ttu-id="3f1b9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3f1b9-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3f1b9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f1b9-120">Authorization</span></span> | <span data-ttu-id="3f1b9-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="3f1b9-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f1b9-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f1b9-122">Request body</span></span>

<span data-ttu-id="3f1b9-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f1b9-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="3f1b9-124">Response</span></span>

<span data-ttu-id="3f1b9-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3f1b9-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="3f1b9-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3f1b9-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f1b9-128">Request</span></span>

<span data-ttu-id="3f1b9-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_workforceintegration"
}-->

```http
DELETE https://graph.microsoft.com/beta/teamwork/workforceIntegrations
```

### <a name="response"></a><span data-ttu-id="3f1b9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f1b9-130">Response</span></span>

<span data-ttu-id="3f1b9-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3f1b9-131">The following is an example of the response.</span></span>

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
  "description": "Delete workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->