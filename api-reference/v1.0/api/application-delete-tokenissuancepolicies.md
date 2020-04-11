---
title: Удаление Токениссуанцеполици
description: Удаление Токениссуанцеполици из приложения.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 670a5cb10c8209ed6e30a5cb8115b752f398487c
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227931"
---
# <a name="remove-tokenissuancepolicy"></a><span data-ttu-id="0365f-103">Удаление Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="0365f-103">Remove tokenIssuancePolicy</span></span>

<span data-ttu-id="0365f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0365f-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="0365f-105">Удаление [токениссуанцеполици](../resources/tokenissuancepolicy.md) из [приложения](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="0365f-105">Remove a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0365f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0365f-106">Permissions</span></span>

<span data-ttu-id="0365f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0365f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0365f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0365f-109">Permission type</span></span>                        | <span data-ttu-id="0365f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0365f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0365f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0365f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0365f-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0365f-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="0365f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0365f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0365f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0365f-114">Not supported.</span></span> |
| <span data-ttu-id="0365f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0365f-115">Application</span></span>                            | <span data-ttu-id="0365f-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0365f-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0365f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0365f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenIssuancePolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0365f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0365f-118">Request headers</span></span>

| <span data-ttu-id="0365f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0365f-119">Name</span></span>          | <span data-ttu-id="0365f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0365f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0365f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0365f-121">Authorization</span></span> | <span data-ttu-id="0365f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0365f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0365f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0365f-124">Request body</span></span>

<span data-ttu-id="0365f-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0365f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0365f-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="0365f-126">Response</span></span>

<span data-ttu-id="0365f-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0365f-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0365f-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="0365f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0365f-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="0365f-129">Request</span></span>

<span data-ttu-id="0365f-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0365f-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_tokenissuancepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/tokenIssuancePolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="0365f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0365f-131">Response</span></span>

<span data-ttu-id="0365f-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0365f-132">The following is an example of the response.</span></span>

> <span data-ttu-id="0365f-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0365f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
