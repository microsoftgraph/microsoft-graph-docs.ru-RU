---
title: Удаление Активитибаседтимеаутполици
description: Удаление Активитибаседтимеаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 29b5e61e9401cd0ed0ee63c82f72042b668cafc1
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234454"
---
# <a name="delete-activitybasedtimeoutpolicy"></a><span data-ttu-id="4a7c1-103">Удаление Активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="4a7c1-103">Delete activityBasedTimeoutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a7c1-104">Удаление объекта [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="4a7c1-104">Delete an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a7c1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a7c1-105">Permissions</span></span>

<span data-ttu-id="4a7c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a7c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a7c1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a7c1-108">Permission type</span></span>                        | <span data-ttu-id="4a7c1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a7c1-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4a7c1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a7c1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a7c1-111">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4a7c1-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="4a7c1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a7c1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a7c1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a7c1-113">Not supported.</span></span> |
| <span data-ttu-id="4a7c1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a7c1-114">Application</span></span>                            | <span data-ttu-id="4a7c1-115">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4a7c1-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a7c1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a7c1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4a7c1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a7c1-117">Request headers</span></span>

| <span data-ttu-id="4a7c1-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4a7c1-118">Name</span></span>          | <span data-ttu-id="4a7c1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4a7c1-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4a7c1-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a7c1-120">Authorization</span></span> | <span data-ttu-id="4a7c1-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="4a7c1-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a7c1-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a7c1-122">Request body</span></span>

<span data-ttu-id="4a7c1-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a7c1-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a7c1-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a7c1-124">Response</span></span>

<span data-ttu-id="4a7c1-125">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4a7c1-125">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4a7c1-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="4a7c1-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4a7c1-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a7c1-127">Request</span></span>

<span data-ttu-id="4a7c1-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a7c1-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_activitybasedtimeoutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="4a7c1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a7c1-129">Response</span></span>

<span data-ttu-id="4a7c1-130">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4a7c1-130">The following is an example of the response.</span></span>

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
  "description": "Delete activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->