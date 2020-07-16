---
title: Назначить tokenIssuancePolicy
description: Назначьте Токениссуанцеполици приложению.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 649cb40d06d5a89cba9a07162410a71ebc54ca2e
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142283"
---
# <a name="assign-tokenissuancepolicy"></a><span data-ttu-id="3ef32-103">Назначить tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="3ef32-103">Assign tokenIssuancePolicy</span></span>

<span data-ttu-id="3ef32-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ef32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ef32-105">Назначьте [токениссуанцеполици](../resources/tokenissuancepolicy.md) [приложению](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="3ef32-105">Assign a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3ef32-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ef32-106">Permissions</span></span>

<span data-ttu-id="3ef32-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ef32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ef32-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ef32-109">Permission type</span></span>                        | <span data-ttu-id="3ef32-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ef32-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3ef32-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ef32-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3ef32-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3ef32-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="3ef32-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ef32-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ef32-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ef32-114">Not supported.</span></span> |
| <span data-ttu-id="3ef32-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3ef32-115">Application</span></span>                            | <span data-ttu-id="3ef32-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3ef32-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ef32-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ef32-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/tokenIssuancePolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="3ef32-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ef32-118">Request headers</span></span>

| <span data-ttu-id="3ef32-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3ef32-119">Name</span></span>          | <span data-ttu-id="3ef32-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3ef32-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3ef32-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ef32-121">Authorization</span></span> | <span data-ttu-id="3ef32-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ef32-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3ef32-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3ef32-124">Content-Type</span></span> | <span data-ttu-id="3ef32-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ef32-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ef32-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ef32-127">Request body</span></span>

<span data-ttu-id="3ef32-128">В тексте запроса укажите идентификатор объекта [токениссуанцеполици](../resources/tokenissuancepolicy.md) (с помощью `@odata.id` Свойства), который должен быть назначен приложению.</span><span class="sxs-lookup"><span data-stu-id="3ef32-128">In the request body, supply the identifier of the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object (using an `@odata.id` property) that should be assigned to the application.</span></span>

## <a name="response"></a><span data-ttu-id="3ef32-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ef32-129">Response</span></span>

<span data-ttu-id="3ef32-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3ef32-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3ef32-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="3ef32-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3ef32-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ef32-133">Request</span></span>

<span data-ttu-id="3ef32-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ef32-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3ef32-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ef32-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenissuancepolicy_from_application"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies/$ref
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="c"></a>[<span data-ttu-id="3ef32-136">C#</span><span class="sxs-lookup"><span data-stu-id="3ef32-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenissuancepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ef32-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ef32-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenissuancepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ef32-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ef32-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenissuancepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3ef32-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ef32-139">Response</span></span>

<span data-ttu-id="3ef32-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3ef32-140">The following is an example of the response.</span></span>

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
  "description": "Assign tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
