---
title: Назначение appliesTo
description: Назначение каталогаОбект для выкатки функций.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8bafd8a2ec3e869ccd20f5aa800be4e63f20ba16
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201338"
---
# <a name="assign-appliesto"></a><span data-ttu-id="7fe87-103">Назначение appliesTo</span><span class="sxs-lookup"><span data-stu-id="7fe87-103">Assign appliesTo</span></span>

<span data-ttu-id="7fe87-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fe87-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7fe87-105">Добавьте appliesTo на [объект featureRolloutPolicy,](../resources/featurerolloutpolicy.md) чтобы указать [directoryObject,](../resources/directoryobject.md) к которому следует применить функциюRolloutPolicy. [](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7fe87-105">Add an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to specify the [directoryObject](../resources/directoryobject.md) to which the [featureRolloutPolicy](../resources/featurerolloutpolicy.md) should be applied.</span></span>

## <a name="permissions"></a><span data-ttu-id="7fe87-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7fe87-106">Permissions</span></span>

<span data-ttu-id="7fe87-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fe87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7fe87-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fe87-109">Permission type</span></span>                        | <span data-ttu-id="7fe87-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fe87-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7fe87-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fe87-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7fe87-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fe87-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="7fe87-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fe87-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fe87-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fe87-114">Not supported.</span></span> |
| <span data-ttu-id="7fe87-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7fe87-115">Application</span></span>                            | <span data-ttu-id="7fe87-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fe87-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fe87-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fe87-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/featureRolloutPolicies/{id}/appliesTo/$ref
```

## <a name="request-headers"></a><span data-ttu-id="7fe87-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7fe87-118">Request headers</span></span>

| <span data-ttu-id="7fe87-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7fe87-119">Name</span></span>          | <span data-ttu-id="7fe87-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7fe87-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7fe87-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7fe87-121">Authorization</span></span> | <span data-ttu-id="7fe87-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="7fe87-122">Bearer {token}.</span></span> <span data-ttu-id="7fe87-123">Обязательна</span><span class="sxs-lookup"><span data-stu-id="7fe87-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="7fe87-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7fe87-124">Request body</span></span>

<span data-ttu-id="7fe87-125">Укажите представление JSON объекта [directoryObject](../resources/directoryobject.md) в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="7fe87-125">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7fe87-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fe87-126">Response</span></span>

<span data-ttu-id="7fe87-127">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7fe87-127">If successful, this method returns a `201 Created` response code and a new [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7fe87-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="7fe87-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7fe87-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fe87-129">Request</span></span>

<span data-ttu-id="7fe87-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7fe87-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7fe87-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fe87-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_featurerolloutpolicy"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/featureRolloutPolicies/{id}/appliesTo/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/2441b489-4f12-4882-b039-8f6006bd66da"
}
```
# <a name="c"></a>[<span data-ttu-id="7fe87-132">C#</span><span class="sxs-lookup"><span data-stu-id="7fe87-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7fe87-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7fe87-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7fe87-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7fe87-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7fe87-135">Java</span><span class="sxs-lookup"><span data-stu-id="7fe87-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7fe87-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fe87-136">Response</span></span>

<span data-ttu-id="7fe87-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7fe87-137">The following is an example of the response.</span></span>

> <span data-ttu-id="7fe87-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7fe87-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


