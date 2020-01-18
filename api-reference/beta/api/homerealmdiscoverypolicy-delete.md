---
title: Удаление Хомереалмдисковериполици
description: Удаление Хомереалмдисковериполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fc54623f6b30226adc493511c1dc8413b5e96421
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234483"
---
# <a name="delete-homerealmdiscoverypolicy"></a><span data-ttu-id="23f9d-103">Удаление Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="23f9d-103">Delete homeRealmDiscoveryPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23f9d-104">Удаление объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="23f9d-104">Delete a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="23f9d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23f9d-105">Permissions</span></span>

<span data-ttu-id="23f9d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23f9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23f9d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23f9d-108">Permission type</span></span>                        | <span data-ttu-id="23f9d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23f9d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="23f9d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23f9d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="23f9d-111">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="23f9d-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="23f9d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23f9d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23f9d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23f9d-113">Not supported.</span></span> |
| <span data-ttu-id="23f9d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23f9d-114">Application</span></span>                            | <span data-ttu-id="23f9d-115">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="23f9d-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="23f9d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23f9d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="23f9d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23f9d-117">Request headers</span></span>

| <span data-ttu-id="23f9d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="23f9d-118">Name</span></span>          | <span data-ttu-id="23f9d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="23f9d-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="23f9d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23f9d-120">Authorization</span></span> | <span data-ttu-id="23f9d-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="23f9d-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="23f9d-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23f9d-122">Request body</span></span>

<span data-ttu-id="23f9d-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23f9d-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23f9d-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="23f9d-124">Response</span></span>

<span data-ttu-id="23f9d-125">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="23f9d-125">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="23f9d-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="23f9d-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="23f9d-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="23f9d-127">Request</span></span>

<span data-ttu-id="23f9d-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23f9d-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="23f9d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="23f9d-129">Response</span></span>

<span data-ttu-id="23f9d-130">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="23f9d-130">The following is an example of the response.</span></span>

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
  "description": "Delete homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->