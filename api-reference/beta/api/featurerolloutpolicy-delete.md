---
title: Удаление Феатурероллаутполици
description: Удаление объекта Феатурероллаутполици.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a23101dc958fddf2d527bc4b7e90bf27bc0067d3
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181114"
---
# <a name="delete-featurerolloutpolicy"></a><span data-ttu-id="8fe50-103">Удаление Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="8fe50-103">Delete featureRolloutPolicy</span></span>

<span data-ttu-id="8fe50-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fe50-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fe50-105">Удаление объекта [феатурероллаутполици](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="8fe50-105">Delete a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8fe50-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8fe50-106">Permissions</span></span>

<span data-ttu-id="8fe50-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fe50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8fe50-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8fe50-109">Permission type</span></span>                        | <span data-ttu-id="8fe50-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8fe50-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8fe50-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8fe50-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8fe50-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="8fe50-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="8fe50-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8fe50-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fe50-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fe50-114">Not supported.</span></span> |
| <span data-ttu-id="8fe50-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8fe50-115">Application</span></span>                            | <span data-ttu-id="8fe50-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fe50-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8fe50-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8fe50-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8fe50-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8fe50-118">Request headers</span></span>

| <span data-ttu-id="8fe50-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8fe50-119">Name</span></span>          | <span data-ttu-id="8fe50-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8fe50-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8fe50-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8fe50-121">Authorization</span></span> | <span data-ttu-id="8fe50-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8fe50-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8fe50-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8fe50-123">Request body</span></span>

<span data-ttu-id="8fe50-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8fe50-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fe50-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fe50-125">Response</span></span>

<span data-ttu-id="8fe50-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8fe50-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8fe50-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="8fe50-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8fe50-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8fe50-129">Request</span></span>

<span data-ttu-id="8fe50-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8fe50-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```

### <a name="response"></a><span data-ttu-id="8fe50-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fe50-131">Response</span></span>

<span data-ttu-id="8fe50-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8fe50-132">The following is an example of the response.</span></span>

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
