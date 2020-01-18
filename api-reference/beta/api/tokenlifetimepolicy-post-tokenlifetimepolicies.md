---
title: Создание Токенлифетимеполици
description: Создание нового Токенлифетимеполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d40146e205dd250f99df3334b5e0c8d0323564c7
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234502"
---
# <a name="create-tokenlifetimepolicy"></a><span data-ttu-id="44875-103">Создание Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="44875-103">Create tokenLifetimePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44875-104">Создание нового объекта [токенлифетимеполици](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="44875-104">Create a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="44875-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44875-105">Permissions</span></span>

<span data-ttu-id="44875-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44875-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44875-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44875-108">Permission type</span></span>                        | <span data-ttu-id="44875-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44875-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="44875-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44875-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="44875-111">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="44875-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="44875-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44875-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44875-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44875-113">Not supported.</span></span> |
| <span data-ttu-id="44875-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44875-114">Application</span></span>                            | <span data-ttu-id="44875-115">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="44875-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="44875-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44875-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="44875-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44875-117">Request headers</span></span>

| <span data-ttu-id="44875-118">Имя</span><span class="sxs-lookup"><span data-stu-id="44875-118">Name</span></span>          | <span data-ttu-id="44875-119">Описание</span><span class="sxs-lookup"><span data-stu-id="44875-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="44875-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44875-120">Authorization</span></span> | <span data-ttu-id="44875-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="44875-121">Bearer {token}</span></span> |
| <span data-ttu-id="44875-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="44875-122">Content-type</span></span> | <span data-ttu-id="44875-123">application/json</span><span class="sxs-lookup"><span data-stu-id="44875-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="44875-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44875-124">Request body</span></span>

<span data-ttu-id="44875-125">В тексте запроса добавьте представление объекта [токенлифетимеполици](../resources/tokenlifetimepolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44875-125">In the request body, supply a JSON representation of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="44875-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="44875-126">Response</span></span>

<span data-ttu-id="44875-127">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [токенлифетимеполици](../resources/tokenlifetimepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44875-127">If successful, this method returns a `201 Created` response code and a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="44875-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="44875-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="44875-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="44875-129">Request</span></span>

<span data-ttu-id="44875-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44875-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_tokenlifetimepolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/tokenLifetimePolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```

### <a name="response"></a><span data-ttu-id="44875-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="44875-131">Response</span></span>

<span data-ttu-id="44875-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="44875-132">The following is an example of the response.</span></span>

> <span data-ttu-id="44875-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44875-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
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
  "description": "Create tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->