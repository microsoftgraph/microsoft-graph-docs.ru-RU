---
title: Создание Клаимсмаппингполици
description: Создание нового Клаимсмаппингполици.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7d4e96ab4f746d24ad436f1c63568533e9c38790
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846329"
---
# <a name="create-claimsmappingpolicy"></a><span data-ttu-id="c936b-103">Создание Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="c936b-103">Create claimsMappingPolicy</span></span>

<span data-ttu-id="c936b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c936b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c936b-105">Создание нового объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="c936b-105">Create a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c936b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c936b-106">Permissions</span></span>

<span data-ttu-id="c936b-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c936b-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c936b-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c936b-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c936b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c936b-109">Permission type</span></span>                        | <span data-ttu-id="c936b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c936b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c936b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c936b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c936b-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="c936b-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="c936b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c936b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c936b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c936b-114">Not supported.</span></span> |
| <span data-ttu-id="c936b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c936b-115">Application</span></span>                            | <span data-ttu-id="c936b-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="c936b-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="c936b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c936b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="c936b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c936b-118">Request headers</span></span>

| <span data-ttu-id="c936b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c936b-119">Name</span></span>          | <span data-ttu-id="c936b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c936b-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c936b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c936b-121">Authorization</span></span> | <span data-ttu-id="c936b-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="c936b-122">Bearer {token}</span></span> |
| <span data-ttu-id="c936b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c936b-123">Content-type</span></span> | <span data-ttu-id="c936b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c936b-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c936b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c936b-125">Request body</span></span>

<span data-ttu-id="c936b-126">В тексте запроса добавьте представление объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c936b-126">In the request body, supply a JSON representation of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c936b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c936b-127">Response</span></span>

<span data-ttu-id="c936b-128">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [клаимсмаппингполици](../resources/claimsmappingpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c936b-128">If successful, this method returns a `201 Created` response code and a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c936b-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="c936b-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c936b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c936b-130">Request</span></span>

<span data-ttu-id="c936b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c936b-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c936b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c936b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_claimsmappingpolicy_from_claimsmappingpolicies"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```

### <a name="response"></a><span data-ttu-id="c936b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c936b-133">Response</span></span>

<span data-ttu-id="c936b-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c936b-134">The following is an example of the response.</span></span>

> <span data-ttu-id="c936b-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="c936b-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c936b-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="c936b-136">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy"
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
  "description": "Create claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
