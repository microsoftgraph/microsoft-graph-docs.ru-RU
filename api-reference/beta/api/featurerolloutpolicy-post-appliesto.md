---
title: Назначение appliesTo
description: Назначение каталогаОбект для выкатки функций.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f845aac0abd8fd8d6f23151ffd4fc99e8b6bdcf3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959300"
---
# <a name="assign-appliesto"></a><span data-ttu-id="3d5cb-103">Назначение appliesTo</span><span class="sxs-lookup"><span data-stu-id="3d5cb-103">Assign appliesTo</span></span>

<span data-ttu-id="3d5cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d5cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d5cb-105">Добавьте appliesTo на [объект featureRolloutPolicy,](../resources/featurerolloutpolicy.md) чтобы указать [directoryObject,](../resources/directoryobject.md) к которому следует применить функциюRolloutPolicy. [](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3d5cb-105">Add an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to specify the [directoryObject](../resources/directoryobject.md) to which the [featureRolloutPolicy](../resources/featurerolloutpolicy.md) should be applied.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d5cb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d5cb-106">Permissions</span></span>

<span data-ttu-id="3d5cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d5cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3d5cb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d5cb-109">Permission type</span></span>                        | <span data-ttu-id="3d5cb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d5cb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3d5cb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d5cb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3d5cb-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d5cb-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="3d5cb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d5cb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d5cb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d5cb-114">Not supported.</span></span> |
| <span data-ttu-id="3d5cb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d5cb-115">Application</span></span>                            | <span data-ttu-id="3d5cb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d5cb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d5cb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d5cb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/featureRolloutPolicies/{id}/appliesTo/$ref
```

## <a name="request-headers"></a><span data-ttu-id="3d5cb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d5cb-118">Request headers</span></span>

| <span data-ttu-id="3d5cb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3d5cb-119">Name</span></span>          | <span data-ttu-id="3d5cb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3d5cb-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3d5cb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d5cb-121">Authorization</span></span> | <span data-ttu-id="3d5cb-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="3d5cb-122">Bearer {token}.</span></span> <span data-ttu-id="3d5cb-123">Обязательный</span><span class="sxs-lookup"><span data-stu-id="3d5cb-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d5cb-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d5cb-124">Request body</span></span>

<span data-ttu-id="3d5cb-125">Укажите представление JSON объекта [directoryObject](../resources/directoryobject.md) в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="3d5cb-125">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3d5cb-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d5cb-126">Response</span></span>

<span data-ttu-id="3d5cb-127">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3d5cb-127">If successful, this method returns a `201 Created` response code and a new [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3d5cb-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="3d5cb-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3d5cb-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d5cb-129">Request</span></span>

<span data-ttu-id="3d5cb-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d5cb-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_featurerolloutpolicy_policies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/featureRolloutPolicies/{id}/appliesTo/$ref
Content-type: application/json

{
  "@odata.id": " https://graph.microsoft.com/beta/directoryObjects/2441b489-4f12-4882-b039-8f6006bd66da"
}
```

### <a name="response"></a><span data-ttu-id="3d5cb-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d5cb-131">Response</span></span>

<span data-ttu-id="3d5cb-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3d5cb-132">The following is an example of the response.</span></span>

> <span data-ttu-id="3d5cb-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3d5cb-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


