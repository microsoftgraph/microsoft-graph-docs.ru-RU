---
title: Удаление типа ресурса homeRealmDiscoveryPolicy
description: Удаление объекта Хомереалмдисковериполици из servicePrincipal.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 98830be617ef35492256bbe6ddc19e7ac1af51d6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453487"
---
# <a name="remove-homerealmdiscoverypolicy"></a><span data-ttu-id="a43c1-103">Удаление типа ресурса homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="a43c1-103">Remove homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="a43c1-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a43c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a43c1-105">Удаление объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) из [servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="a43c1-105">Remove a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) from a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a43c1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a43c1-106">Permissions</span></span>

<span data-ttu-id="a43c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a43c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a43c1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a43c1-109">Permission type</span></span>                        | <span data-ttu-id="a43c1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a43c1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a43c1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a43c1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a43c1-112">Policy. Read. ALL и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a43c1-112">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="a43c1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a43c1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a43c1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a43c1-114">Not supported.</span></span> |
| <span data-ttu-id="a43c1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a43c1-115">Application</span></span>                            | <span data-ttu-id="a43c1-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a43c1-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a43c1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a43c1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="a43c1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a43c1-118">Request headers</span></span>

| <span data-ttu-id="a43c1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a43c1-119">Name</span></span>          | <span data-ttu-id="a43c1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a43c1-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a43c1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a43c1-121">Authorization</span></span> | <span data-ttu-id="a43c1-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="a43c1-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a43c1-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a43c1-123">Request body</span></span>

<span data-ttu-id="a43c1-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a43c1-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a43c1-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="a43c1-125">Response</span></span>

<span data-ttu-id="a43c1-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a43c1-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a43c1-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="a43c1-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a43c1-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="a43c1-128">Request</span></span>

<span data-ttu-id="a43c1-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a43c1-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy_from_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="a43c1-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a43c1-130">Response</span></span>

<span data-ttu-id="a43c1-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a43c1-131">The following is an example of the response.</span></span>

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