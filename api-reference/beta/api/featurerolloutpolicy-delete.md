---
title: Удаление featureRolloutPolicy
description: Удаление объекта featureRolloutPolicy.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d7197ffff516b1343b14c6042480fd003a94fac6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436101"
---
# <a name="delete-featurerolloutpolicy"></a><span data-ttu-id="39912-103">Удаление featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="39912-103">Delete featureRolloutPolicy</span></span>

<span data-ttu-id="39912-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39912-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39912-105">Удаление [объекта featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="39912-105">Delete a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="39912-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39912-106">Permissions</span></span>

<span data-ttu-id="39912-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39912-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="39912-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39912-109">Permission type</span></span>                        | <span data-ttu-id="39912-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39912-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="39912-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39912-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="39912-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="39912-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="39912-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39912-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39912-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39912-114">Not supported.</span></span> |
| <span data-ttu-id="39912-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39912-115">Application</span></span>                            | <span data-ttu-id="39912-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39912-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="39912-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39912-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="39912-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39912-118">Request headers</span></span>

| <span data-ttu-id="39912-119">Имя</span><span class="sxs-lookup"><span data-stu-id="39912-119">Name</span></span>          | <span data-ttu-id="39912-120">Описание</span><span class="sxs-lookup"><span data-stu-id="39912-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="39912-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39912-121">Authorization</span></span> | <span data-ttu-id="39912-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="39912-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="39912-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39912-123">Request body</span></span>

<span data-ttu-id="39912-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="39912-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39912-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="39912-125">Response</span></span>

<span data-ttu-id="39912-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="39912-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="39912-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="39912-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="39912-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="39912-129">Request</span></span>

<span data-ttu-id="39912-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39912-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```

### <a name="response"></a><span data-ttu-id="39912-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="39912-131">Response</span></span>

<span data-ttu-id="39912-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="39912-132">The following is an example of the response.</span></span>

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


