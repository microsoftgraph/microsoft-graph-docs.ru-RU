---
title: Удаление Феатурероллаутполици
description: Удаление объекта Феатурероллаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 72163a15beb9b6b82c4ad60640add3849d60a8b1
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062168"
---
# <a name="delete-featurerolloutpolicy"></a><span data-ttu-id="fdc92-103">Удаление Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="fdc92-103">Delete featureRolloutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdc92-104">Удаление объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="fdc92-104">Delete a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fdc92-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fdc92-105">Permissions</span></span>

<span data-ttu-id="fdc92-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdc92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fdc92-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fdc92-108">Permission type</span></span>                        | <span data-ttu-id="fdc92-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fdc92-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fdc92-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fdc92-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fdc92-111">Policy. ReadWrite. Феатурероллаут</span><span class="sxs-lookup"><span data-stu-id="fdc92-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="fdc92-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fdc92-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdc92-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdc92-113">Not supported.</span></span> |
| <span data-ttu-id="fdc92-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fdc92-114">Application</span></span>                            | <span data-ttu-id="fdc92-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdc92-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdc92-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fdc92-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fdc92-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fdc92-117">Request headers</span></span>

| <span data-ttu-id="fdc92-118">Имя</span><span class="sxs-lookup"><span data-stu-id="fdc92-118">Name</span></span>          | <span data-ttu-id="fdc92-119">Описание</span><span class="sxs-lookup"><span data-stu-id="fdc92-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fdc92-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fdc92-120">Authorization</span></span> | <span data-ttu-id="fdc92-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="fdc92-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="fdc92-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fdc92-122">Request body</span></span>

<span data-ttu-id="fdc92-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fdc92-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdc92-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="fdc92-124">Response</span></span>

<span data-ttu-id="fdc92-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fdc92-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fdc92-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="fdc92-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fdc92-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdc92-128">Request</span></span>

<span data-ttu-id="fdc92-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fdc92-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```

### <a name="response"></a><span data-ttu-id="fdc92-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdc92-130">Response</span></span>

<span data-ttu-id="fdc92-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fdc92-131">The following is an example of the response.</span></span>

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