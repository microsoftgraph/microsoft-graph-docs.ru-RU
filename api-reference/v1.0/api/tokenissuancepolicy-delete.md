---
title: Удаление Токениссуанцеполици
description: Удаление Токениссуанцеполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ed3f02e1ff6cb566922282548e0b9fb252f6784b
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229698"
---
# <a name="delete-tokenissuancepolicy"></a><span data-ttu-id="0ffc9-103">Удаление Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="0ffc9-103">Delete tokenIssuancePolicy</span></span>

<span data-ttu-id="0ffc9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ffc9-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="0ffc9-105">Удаление объекта [токениссуанцеполици](../resources/tokenissuancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="0ffc9-105">Delete a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ffc9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ffc9-106">Permissions</span></span>

<span data-ttu-id="0ffc9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ffc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ffc9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ffc9-109">Permission type</span></span>                        | <span data-ttu-id="0ffc9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ffc9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0ffc9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ffc9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0ffc9-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ffc9-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="0ffc9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ffc9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ffc9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ffc9-114">Not supported.</span></span> |
| <span data-ttu-id="0ffc9-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0ffc9-115">Application</span></span>                            | <span data-ttu-id="0ffc9-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ffc9-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ffc9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ffc9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/tokenIssuancePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0ffc9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ffc9-118">Request headers</span></span>

| <span data-ttu-id="0ffc9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0ffc9-119">Name</span></span>          | <span data-ttu-id="0ffc9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0ffc9-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0ffc9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ffc9-121">Authorization</span></span> | <span data-ttu-id="0ffc9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ffc9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ffc9-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ffc9-124">Request body</span></span>

<span data-ttu-id="0ffc9-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ffc9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ffc9-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ffc9-126">Response</span></span>

<span data-ttu-id="0ffc9-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0ffc9-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0ffc9-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="0ffc9-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0ffc9-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ffc9-129">Request</span></span>

<span data-ttu-id="0ffc9-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ffc9-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_tokenissuancepolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies/{id}
```

### <a name="response"></a><span data-ttu-id="0ffc9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ffc9-131">Response</span></span>

<span data-ttu-id="0ffc9-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0ffc9-132">The following is an example of the response.</span></span>

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
  "description": "Delete tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
