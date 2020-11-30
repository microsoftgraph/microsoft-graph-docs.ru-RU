---
title: Удаление Делегатедпермиссионклассификатион
description: Удаление делегированной классификации разрешений из субъекта-службы API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 53e3f249ffe909310b446687ffba720752557b63
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377248"
---
# <a name="delete-delegatedpermissionclassification"></a><span data-ttu-id="e7d7f-103">Удаление Делегатедпермиссионклассификатион</span><span class="sxs-lookup"><span data-stu-id="e7d7f-103">Delete delegatedPermissionClassification</span></span>

<span data-ttu-id="e7d7f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7d7f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e7d7f-105">Удаляет объект [делегатедпермиссионклассификатион](../resources/delegatedPermissionClassification.md) , который ранее был задан для делегированного разрешения.</span><span class="sxs-lookup"><span data-stu-id="e7d7f-105">Deletes a [delegatedPermissionClassification](../resources/delegatedPermissionClassification.md) which had previously been set for a delegated permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7d7f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e7d7f-106">Permissions</span></span>

<span data-ttu-id="e7d7f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7d7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7d7f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7d7f-109">Permission type</span></span>      | <span data-ttu-id="e7d7f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7d7f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7d7f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7d7f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e7d7f-112">Пермиссионгрантполици. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e7d7f-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="e7d7f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7d7f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7d7f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7d7f-114">Not supported.</span></span>    |
|<span data-ttu-id="e7d7f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="e7d7f-115">Application</span></span> | <span data-ttu-id="e7d7f-116">Пермиссионгрантполици. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e7d7f-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7d7f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7d7f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/delegatedPermissionClassifications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e7d7f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7d7f-118">Request headers</span></span>

| <span data-ttu-id="e7d7f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e7d7f-119">Name</span></span>       | <span data-ttu-id="e7d7f-120">Тип</span><span class="sxs-lookup"><span data-stu-id="e7d7f-120">Type</span></span> | <span data-ttu-id="e7d7f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e7d7f-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e7d7f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7d7f-122">Authorization</span></span>  | <span data-ttu-id="e7d7f-123">string</span><span class="sxs-lookup"><span data-stu-id="e7d7f-123">string</span></span>  | <span data-ttu-id="e7d7f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7d7f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7d7f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e7d7f-126">Request body</span></span>

<span data-ttu-id="e7d7f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e7d7f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7d7f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7d7f-128">Response</span></span>

<span data-ttu-id="e7d7f-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e7d7f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e7d7f-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="e7d7f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e7d7f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7d7f-132">Request</span></span>

<span data-ttu-id="e7d7f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7d7f-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_delegatedpermissionclassifications"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/delegatedPermissionClassifications/{id}
```

### <a name="response"></a><span data-ttu-id="e7d7f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7d7f-134">Response</span></span>

<span data-ttu-id="e7d7f-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e7d7f-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
