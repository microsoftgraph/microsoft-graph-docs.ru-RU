---
title: Назначение appliesTo
description: Назначение directoryObject для развертывания компонентов.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cf1f67ff84c6ba5bff7c171a16a73d07febca8d3
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420408"
---
# <a name="assign-appliesto"></a><span data-ttu-id="bb59f-103">Назначение appliesTo</span><span class="sxs-lookup"><span data-stu-id="bb59f-103">Assign appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb59f-104">Добавьте элемент appliesTo в объект [феатурероллаутполици](../resources/featurerolloutpolicy.md) , чтобы указать [directoryObject](../resources/directoryobject.md) , к которому необходимо применить [феатурероллаутполици](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="bb59f-104">Add an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to specify the [directoryObject](../resources/directoryobject.md) to which the [featureRolloutPolicy](../resources/featurerolloutpolicy.md) should be applied to.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb59f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb59f-105">Permissions</span></span>

<span data-ttu-id="bb59f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb59f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bb59f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb59f-108">Permission type</span></span>                        | <span data-ttu-id="bb59f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb59f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bb59f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb59f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb59f-111">Policy. ReadWrite. Феатурероллаут</span><span class="sxs-lookup"><span data-stu-id="bb59f-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="bb59f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb59f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb59f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb59f-113">Not supported.</span></span> |
| <span data-ttu-id="bb59f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb59f-114">Application</span></span>                            | <span data-ttu-id="bb59f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb59f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb59f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb59f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies/{id}/appliesTo/$ref
```

## <a name="request-headers"></a><span data-ttu-id="bb59f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb59f-117">Request headers</span></span>

| <span data-ttu-id="bb59f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bb59f-118">Name</span></span>          | <span data-ttu-id="bb59f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bb59f-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bb59f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb59f-120">Authorization</span></span> | <span data-ttu-id="bb59f-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bb59f-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb59f-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb59f-122">Request body</span></span>

<span data-ttu-id="bb59f-123">В тексте запроса добавьте представление объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb59f-123">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bb59f-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb59f-124">Response</span></span>

<span data-ttu-id="bb59f-125">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb59f-125">If successful, this method returns a `201 Created` response code and a new [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bb59f-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="bb59f-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bb59f-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb59f-127">Request</span></span>

<span data-ttu-id="bb59f-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb59f-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bb59f-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb59f-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_featurerolloutpolicy"
}-->

```http
POST https://graph.microsoft.com/beta/directory/featureRolloutPolicies/{id}/appliesTo/$ref
Content-type: application/json

{
  "@odata.id": " https://graph.microsoft.com/beta/directoryObjects/2441b489-4f12-4882-b039-8f6006bd66da"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bb59f-130">C#</span><span class="sxs-lookup"><span data-stu-id="bb59f-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb59f-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb59f-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bb59f-132">Цель — C</span><span class="sxs-lookup"><span data-stu-id="bb59f-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bb59f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb59f-133">Response</span></span>

<span data-ttu-id="bb59f-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bb59f-134">The following is an example of the response.</span></span>

> <span data-ttu-id="bb59f-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb59f-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "directoryObject": {
    "id": "2441b489-4f12-4882-b039-8f6006bd66da",
    "objectType": "group"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Assign appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
