---
title: Удаление типа ресурса homeRealmDiscoveryPolicy
description: Удаление объекта Хомереалмдисковериполици из servicePrincipal.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b6e1a0c0568fbb72d26b7e51e731fa66301d6cec
ms.sourcegitcommit: 435d80cfa71574c06d24780c591d4303a5cd9636
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2020
ms.locfileid: "42562733"
---
# <a name="remove-homerealmdiscoverypolicy"></a><span data-ttu-id="8727a-103">Удаление типа ресурса homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="8727a-103">Remove homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="8727a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8727a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8727a-105">Удаление объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) из [servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="8727a-105">Remove a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) from a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8727a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8727a-106">Permissions</span></span>

<span data-ttu-id="8727a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8727a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8727a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8727a-109">Permission type</span></span>                        | <span data-ttu-id="8727a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8727a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8727a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8727a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8727a-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8727a-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="8727a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8727a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8727a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8727a-114">Not supported.</span></span> |
| <span data-ttu-id="8727a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8727a-115">Application</span></span>                            | <span data-ttu-id="8727a-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8727a-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8727a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8727a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="8727a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8727a-118">Request headers</span></span>

| <span data-ttu-id="8727a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8727a-119">Name</span></span>          | <span data-ttu-id="8727a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8727a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8727a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8727a-121">Authorization</span></span> | <span data-ttu-id="8727a-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="8727a-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8727a-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8727a-123">Request body</span></span>

<span data-ttu-id="8727a-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8727a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8727a-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="8727a-125">Response</span></span>

<span data-ttu-id="8727a-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8727a-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8727a-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="8727a-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8727a-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="8727a-128">Request</span></span>

<span data-ttu-id="8727a-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8727a-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy_from_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="8727a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8727a-130">Response</span></span>

<span data-ttu-id="8727a-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8727a-131">The following is an example of the response.</span></span>

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
  "description": "Remove homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->