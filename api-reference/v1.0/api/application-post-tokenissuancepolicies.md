---
title: Назначение Токениссуанцеполици
description: Назначьте Токениссуанцеполици приложению.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9fb13280c5998926933efb5cbf6aa265cb17ab4f
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227922"
---
# <a name="assign-tokenissuancepolicy"></a><span data-ttu-id="1a91c-103">Назначение Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="1a91c-103">Assign tokenIssuancePolicy</span></span>

<span data-ttu-id="1a91c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a91c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1a91c-105">Назначьте [токениссуанцеполици](../resources/tokenissuancepolicy.md) [приложению](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="1a91c-105">Assign a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1a91c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a91c-106">Permissions</span></span>

<span data-ttu-id="1a91c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a91c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a91c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a91c-109">Permission type</span></span>                        | <span data-ttu-id="1a91c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a91c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1a91c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a91c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a91c-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1a91c-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="1a91c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a91c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a91c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a91c-114">Not supported.</span></span> |
| <span data-ttu-id="1a91c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="1a91c-115">Application</span></span>                            | <span data-ttu-id="1a91c-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1a91c-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a91c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a91c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/tokenIssuancePolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="1a91c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a91c-118">Request headers</span></span>

| <span data-ttu-id="1a91c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1a91c-119">Name</span></span>          | <span data-ttu-id="1a91c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1a91c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1a91c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a91c-121">Authorization</span></span> | <span data-ttu-id="1a91c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a91c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1a91c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1a91c-124">Content-Type</span></span> | <span data-ttu-id="1a91c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a91c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a91c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1a91c-127">Request body</span></span>

<span data-ttu-id="1a91c-128">В тексте запроса укажите идентификатор объекта [токениссуанцеполици](../resources/tokenissuancepolicy.md) (с помощью `@odata.id` свойства), который должен быть назначен приложению.</span><span class="sxs-lookup"><span data-stu-id="1a91c-128">In the request body, supply the identifier of the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object (using an `@odata.id` property) that should be assigned to the application.</span></span>

## <a name="response"></a><span data-ttu-id="1a91c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a91c-129">Response</span></span>

<span data-ttu-id="1a91c-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1a91c-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1a91c-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="1a91c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1a91c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a91c-133">Request</span></span>

<span data-ttu-id="1a91c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a91c-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_tokenissuancepolicy_from_application"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/tokenIssuancePolicies/$ref
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```

### <a name="response"></a><span data-ttu-id="1a91c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a91c-135">Response</span></span>

<span data-ttu-id="1a91c-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1a91c-136">The following is an example of the response.</span></span>

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
