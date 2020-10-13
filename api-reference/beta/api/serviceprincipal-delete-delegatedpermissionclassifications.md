---
title: Удаление Делегатедпермиссионклассификатион
description: Удаление делегированной классификации разрешений из субъекта-службы API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 8a246fbed9b226e36429d82cfb99eee704ca754c
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433616"
---
# <a name="delete-delegatedpermissionclassification"></a><span data-ttu-id="7e901-103">Удаление Делегатедпермиссионклассификатион</span><span class="sxs-lookup"><span data-stu-id="7e901-103">Delete delegatedPermissionClassification</span></span>

<span data-ttu-id="7e901-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e901-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e901-105">Удаляет объект [делегатедпермиссионклассификатион](../resources/delegatedPermissionClassification.md) , который ранее был задан для делегированного разрешения.</span><span class="sxs-lookup"><span data-stu-id="7e901-105">Deletes a [delegatedPermissionClassification](../resources/delegatedPermissionClassification.md) which had previously been set for a delegated permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e901-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e901-106">Permissions</span></span>

<span data-ttu-id="7e901-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e901-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e901-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e901-109">Permission type</span></span>      | <span data-ttu-id="7e901-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e901-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e901-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e901-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7e901-112">Пермиссионгрантполици. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7e901-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="7e901-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e901-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e901-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e901-114">Not supported.</span></span>    |
|<span data-ttu-id="7e901-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="7e901-115">Application</span></span> | <span data-ttu-id="7e901-116">Пермиссионгрантполици. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7e901-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e901-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e901-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/delegatedPermissionClassifications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7e901-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e901-118">Request headers</span></span>

| <span data-ttu-id="7e901-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7e901-119">Name</span></span>       | <span data-ttu-id="7e901-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7e901-120">Type</span></span> | <span data-ttu-id="7e901-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7e901-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7e901-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e901-122">Authorization</span></span>  | <span data-ttu-id="7e901-123">string</span><span class="sxs-lookup"><span data-stu-id="7e901-123">string</span></span>  | <span data-ttu-id="7e901-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e901-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e901-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e901-126">Request body</span></span>

<span data-ttu-id="7e901-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e901-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e901-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e901-128">Response</span></span>

<span data-ttu-id="7e901-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7e901-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7e901-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="7e901-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7e901-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e901-132">Request</span></span>

<span data-ttu-id="7e901-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e901-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_delegatedpermissionclassifications"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/delegatedPermissionClassifications/{id}
```

### <a name="response"></a><span data-ttu-id="7e901-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e901-134">Response</span></span>

<span data-ttu-id="7e901-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7e901-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
