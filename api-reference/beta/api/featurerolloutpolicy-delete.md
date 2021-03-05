---
title: Удаление featureRolloutPolicy
description: Удаление объекта featureRolloutPolicy.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 62395dec00e5a7713ffb959f1a871eedd1da50c5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471189"
---
# <a name="delete-featurerolloutpolicy"></a><span data-ttu-id="6cf61-103">Удаление featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="6cf61-103">Delete featureRolloutPolicy</span></span>

<span data-ttu-id="6cf61-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cf61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cf61-105">Удаление [объекта featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6cf61-105">Delete a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cf61-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6cf61-106">Permissions</span></span>

<span data-ttu-id="6cf61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cf61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6cf61-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6cf61-109">Permission type</span></span>                        | <span data-ttu-id="6cf61-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6cf61-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6cf61-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6cf61-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6cf61-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cf61-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="6cf61-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6cf61-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cf61-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cf61-114">Not supported.</span></span> |
| <span data-ttu-id="6cf61-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6cf61-115">Application</span></span>                            | <span data-ttu-id="6cf61-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cf61-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6cf61-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6cf61-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6cf61-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6cf61-118">Request headers</span></span>

| <span data-ttu-id="6cf61-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6cf61-119">Name</span></span>          | <span data-ttu-id="6cf61-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6cf61-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6cf61-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6cf61-121">Authorization</span></span> | <span data-ttu-id="6cf61-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6cf61-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6cf61-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6cf61-123">Request body</span></span>

<span data-ttu-id="6cf61-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6cf61-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cf61-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cf61-125">Response</span></span>

<span data-ttu-id="6cf61-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6cf61-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6cf61-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="6cf61-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6cf61-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cf61-129">Request</span></span>

<span data-ttu-id="6cf61-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cf61-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```

### <a name="response"></a><span data-ttu-id="6cf61-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cf61-131">Response</span></span>

<span data-ttu-id="6cf61-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6cf61-132">The following is an example of the response.</span></span>

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


