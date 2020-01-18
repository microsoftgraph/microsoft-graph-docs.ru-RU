---
title: Создание Хомереалмдисковериполици
description: Создание нового Хомереалмдисковериполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 852cfa3a09dbf765e9da67ca01bb94b5661b7a7a
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234471"
---
# <a name="create-homerealmdiscoverypolicy"></a><span data-ttu-id="e7f81-103">Создание Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="e7f81-103">Create homeRealmDiscoveryPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7f81-104">Создание нового объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="e7f81-104">Create a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7f81-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e7f81-105">Permissions</span></span>

<span data-ttu-id="e7f81-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7f81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e7f81-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7f81-108">Permission type</span></span>                        | <span data-ttu-id="e7f81-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7f81-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e7f81-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7f81-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e7f81-111">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e7f81-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="e7f81-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7f81-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7f81-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7f81-113">Not supported.</span></span> |
| <span data-ttu-id="e7f81-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7f81-114">Application</span></span>                            | <span data-ttu-id="e7f81-115">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e7f81-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7f81-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7f81-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="e7f81-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7f81-117">Request headers</span></span>

| <span data-ttu-id="e7f81-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e7f81-118">Name</span></span>          | <span data-ttu-id="e7f81-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e7f81-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e7f81-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e7f81-120">Authorization</span></span> | <span data-ttu-id="e7f81-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="e7f81-121">Bearer {token}</span></span> |
| <span data-ttu-id="e7f81-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e7f81-122">Content-type</span></span> | <span data-ttu-id="e7f81-123">application/json</span><span class="sxs-lookup"><span data-stu-id="e7f81-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7f81-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e7f81-124">Request body</span></span>

<span data-ttu-id="e7f81-125">В тексте запроса добавьте представление объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7f81-125">In the request body, supply a JSON representation of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e7f81-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7f81-126">Response</span></span>

<span data-ttu-id="e7f81-127">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e7f81-127">If successful, this method returns a `201 Created` response code and a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e7f81-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="e7f81-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e7f81-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7f81-129">Request</span></span>

<span data-ttu-id="e7f81-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7f81-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_homerealmdiscoverypolicy_from_homerealmdiscoverypolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```

### <a name="response"></a><span data-ttu-id="e7f81-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7f81-131">Response</span></span>

<span data-ttu-id="e7f81-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e7f81-132">The following is an example of the response.</span></span>

> <span data-ttu-id="e7f81-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e7f81-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->