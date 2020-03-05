---
title: Удаление типа ресурса claimsMappingPolicy
description: Удаление объекта Клаимсмаппингполици из servicePrincipal.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 077476c07e5df3804b67ff7b8974f79e715551bf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453508"
---
# <a name="remove-claimsmappingpolicy"></a><span data-ttu-id="0ffca-103">Удаление типа ресурса claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="0ffca-103">Remove claimsMappingPolicy</span></span>

<span data-ttu-id="0ffca-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0ffca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ffca-105">Удаление объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) из [servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="0ffca-105">Remove a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) from a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0ffca-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ffca-106">Permissions</span></span>

<span data-ttu-id="0ffca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ffca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ffca-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ffca-109">Permission type</span></span>                        | <span data-ttu-id="0ffca-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ffca-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0ffca-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ffca-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0ffca-112">Policy. Read. ALL и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0ffca-112">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="0ffca-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ffca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ffca-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ffca-114">Not supported.</span></span> |
| <span data-ttu-id="0ffca-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ffca-115">Application</span></span>                            | <span data-ttu-id="0ffca-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0ffca-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ffca-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ffca-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/claimsMappingPolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="0ffca-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ffca-118">Request headers</span></span>

| <span data-ttu-id="0ffca-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0ffca-119">Name</span></span>          | <span data-ttu-id="0ffca-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0ffca-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0ffca-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ffca-121">Authorization</span></span> | <span data-ttu-id="0ffca-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="0ffca-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ffca-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ffca-123">Request body</span></span>

<span data-ttu-id="0ffca-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ffca-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ffca-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ffca-125">Response</span></span>

<span data-ttu-id="0ffca-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0ffca-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0ffca-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="0ffca-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0ffca-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ffca-128">Request</span></span>

<span data-ttu-id="0ffca-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ffca-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy_from_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="0ffca-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ffca-130">Response</span></span>

<span data-ttu-id="0ffca-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0ffca-131">The following is an example of the response.</span></span>

> <span data-ttu-id="0ffca-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ffca-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->