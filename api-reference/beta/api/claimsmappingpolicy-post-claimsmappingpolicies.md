---
title: Создание Клаимсмаппингполици
description: Создание нового Клаимсмаппингполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fde1bc6f941009c2b6d8a88e19956229f53cd9e4
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234466"
---
# <a name="create-claimsmappingpolicy"></a><span data-ttu-id="8f961-103">Создание Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="8f961-103">Create claimsMappingPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f961-104">Создание нового объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="8f961-104">Create a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f961-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f961-105">Permissions</span></span>

<span data-ttu-id="8f961-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f961-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f961-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f961-108">Permission type</span></span>                        | <span data-ttu-id="8f961-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f961-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8f961-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f961-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f961-111">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="8f961-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="8f961-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f961-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f961-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f961-113">Not supported.</span></span> |
| <span data-ttu-id="8f961-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f961-114">Application</span></span>                            | <span data-ttu-id="8f961-115">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="8f961-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f961-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f961-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="8f961-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f961-117">Request headers</span></span>

| <span data-ttu-id="8f961-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8f961-118">Name</span></span>          | <span data-ttu-id="8f961-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8f961-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8f961-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f961-120">Authorization</span></span> | <span data-ttu-id="8f961-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="8f961-121">Bearer {token}</span></span> |
| <span data-ttu-id="8f961-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f961-122">Content-type</span></span> | <span data-ttu-id="8f961-123">application/json</span><span class="sxs-lookup"><span data-stu-id="8f961-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f961-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f961-124">Request body</span></span>

<span data-ttu-id="8f961-125">В тексте запроса добавьте представление объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f961-125">In the request body, supply a JSON representation of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8f961-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f961-126">Response</span></span>

<span data-ttu-id="8f961-127">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [клаимсмаппингполици](../resources/claimsmappingpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f961-127">If successful, this method returns a `201 Created` response code and a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f961-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="8f961-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8f961-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f961-129">Request</span></span>

<span data-ttu-id="8f961-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f961-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_claimsmappingpolicy_from_claimsmappingpolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/claimsMappingPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```

### <a name="response"></a><span data-ttu-id="8f961-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f961-131">Response</span></span>

<span data-ttu-id="8f961-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8f961-132">The following is an example of the response.</span></span>

> <span data-ttu-id="8f961-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f961-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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