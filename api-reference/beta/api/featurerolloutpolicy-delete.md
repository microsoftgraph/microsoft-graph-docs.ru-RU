---
title: Удаление Феатурероллаутполици
description: Удаление объекта Феатурероллаутполици.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 078af77e9b3cffa63e7a86b22aec49c7d98b3dee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006771"
---
# <a name="delete-featurerolloutpolicy"></a><span data-ttu-id="e4888-103">Удаление Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="e4888-103">Delete featureRolloutPolicy</span></span>

<span data-ttu-id="e4888-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4888-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4888-105">Удаление объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="e4888-105">Delete a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4888-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4888-106">Permissions</span></span>

<span data-ttu-id="e4888-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4888-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e4888-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4888-109">Permission type</span></span>                        | <span data-ttu-id="e4888-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4888-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e4888-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4888-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e4888-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="e4888-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="e4888-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4888-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4888-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4888-114">Not supported.</span></span> |
| <span data-ttu-id="e4888-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4888-115">Application</span></span>                            | <span data-ttu-id="e4888-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4888-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4888-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4888-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e4888-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4888-118">Request headers</span></span>

| <span data-ttu-id="e4888-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e4888-119">Name</span></span>          | <span data-ttu-id="e4888-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e4888-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e4888-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4888-121">Authorization</span></span> | <span data-ttu-id="e4888-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e4888-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4888-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4888-123">Request body</span></span>

<span data-ttu-id="e4888-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4888-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4888-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4888-125">Response</span></span>

<span data-ttu-id="e4888-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e4888-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e4888-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="e4888-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e4888-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4888-129">Request</span></span>

<span data-ttu-id="e4888-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4888-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```

### <a name="response"></a><span data-ttu-id="e4888-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4888-131">Response</span></span>

<span data-ttu-id="e4888-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e4888-132">The following is an example of the response.</span></span>

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
  "description": "Delete featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


