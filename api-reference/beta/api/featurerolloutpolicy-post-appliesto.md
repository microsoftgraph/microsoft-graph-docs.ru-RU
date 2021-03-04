---
title: Назначение appliesTo
description: Назначение каталогаОбект для выкатки функций.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7f8842d554f5cb6f949f0f7f528b3b1f506936f8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436094"
---
# <a name="assign-appliesto"></a><span data-ttu-id="29591-103">Назначение appliesTo</span><span class="sxs-lookup"><span data-stu-id="29591-103">Assign appliesTo</span></span>

<span data-ttu-id="29591-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29591-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29591-105">Добавьте appliesTo на [объект featureRolloutPolicy,](../resources/featurerolloutpolicy.md) чтобы указать [directoryObject,](../resources/directoryobject.md) к которому следует применить функциюRolloutPolicy. [](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="29591-105">Add an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to specify the [directoryObject](../resources/directoryobject.md) to which the [featureRolloutPolicy](../resources/featurerolloutpolicy.md) should be applied to.</span></span>

## <a name="permissions"></a><span data-ttu-id="29591-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29591-106">Permissions</span></span>

<span data-ttu-id="29591-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29591-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="29591-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29591-109">Permission type</span></span>                        | <span data-ttu-id="29591-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29591-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="29591-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29591-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="29591-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="29591-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="29591-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29591-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29591-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29591-114">Not supported.</span></span> |
| <span data-ttu-id="29591-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29591-115">Application</span></span>                            | <span data-ttu-id="29591-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29591-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="29591-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29591-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies/{id}/appliesTo/$ref
```

## <a name="request-headers"></a><span data-ttu-id="29591-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29591-118">Request headers</span></span>

| <span data-ttu-id="29591-119">Имя</span><span class="sxs-lookup"><span data-stu-id="29591-119">Name</span></span>          | <span data-ttu-id="29591-120">Описание</span><span class="sxs-lookup"><span data-stu-id="29591-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="29591-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="29591-121">Authorization</span></span> | <span data-ttu-id="29591-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="29591-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="29591-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29591-123">Request body</span></span>

<span data-ttu-id="29591-124">Укажите представление JSON объекта [directoryObject](../resources/directoryobject.md) в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="29591-124">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="29591-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="29591-125">Response</span></span>

<span data-ttu-id="29591-126">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="29591-126">If successful, this method returns a `201 Created` response code and a new [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="29591-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="29591-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="29591-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="29591-128">Request</span></span>

<span data-ttu-id="29591-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29591-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="29591-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="29591-130">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="29591-131">C#</span><span class="sxs-lookup"><span data-stu-id="29591-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29591-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29591-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29591-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29591-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29591-134">Java</span><span class="sxs-lookup"><span data-stu-id="29591-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="29591-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="29591-135">Response</span></span>

<span data-ttu-id="29591-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="29591-136">The following is an example of the response.</span></span>

> <span data-ttu-id="29591-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="29591-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


