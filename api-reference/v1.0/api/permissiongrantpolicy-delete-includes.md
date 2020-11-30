---
title: Удаление Пермиссионгранткондитионсет из коллекции включенных элементов Пермиссионгрантполици
description: Удаляет включенный набор условий из политики предоставления разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: ca7a37c0cbcb67aa2bf8fc961c8f3211a85a4256
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377242"
---
# <a name="delete-permissiongrantconditionset-from-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="9f6f8-103">Удаление Пермиссионгранткондитионсет из коллекции включенных элементов Пермиссионгрантполици</span><span class="sxs-lookup"><span data-stu-id="9f6f8-103">Delete permissionGrantConditionSet from includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="9f6f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f6f8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9f6f8-105">Удаляет объект [пермиссионгранткондитионсет](../resources/permissiongrantconditionset.md) из коллекции **includes** объекта [пермиссионгрантполици](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9f6f8-105">Deletes a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) from the **includes** collection of a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9f6f8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f6f8-106">Permissions</span></span>

<span data-ttu-id="9f6f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f6f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f6f8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f6f8-109">Permission type</span></span>      | <span data-ttu-id="9f6f8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f6f8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="9f6f8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f6f8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9f6f8-112">Пермиссионгрантполици. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9f6f8-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
| <span data-ttu-id="9f6f8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f6f8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f6f8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f6f8-114">Not supported.</span></span>    |
| <span data-ttu-id="9f6f8-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="9f6f8-115">Application</span></span> | <span data-ttu-id="9f6f8-116">Пермиссионгрантполици. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9f6f8-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f6f8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f6f8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{permissiongrantpolicy-id}/includes/{include-id}
```

## <a name="request-headers"></a><span data-ttu-id="9f6f8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f6f8-118">Request headers</span></span>

| <span data-ttu-id="9f6f8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9f6f8-119">Name</span></span>       | <span data-ttu-id="9f6f8-120">Тип</span><span class="sxs-lookup"><span data-stu-id="9f6f8-120">Type</span></span> | <span data-ttu-id="9f6f8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9f6f8-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9f6f8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f6f8-122">Authorization</span></span>  | <span data-ttu-id="9f6f8-123">string</span><span class="sxs-lookup"><span data-stu-id="9f6f8-123">string</span></span>  | <span data-ttu-id="9f6f8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f6f8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f6f8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f6f8-126">Request body</span></span>

<span data-ttu-id="9f6f8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f6f8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f6f8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f6f8-128">Response</span></span>

<span data-ttu-id="9f6f8-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9f6f8-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f6f8-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="9f6f8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9f6f8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f6f8-132">Request</span></span>

<span data-ttu-id="9f6f8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f6f8-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_delete_includes"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/my-custom-consent-policy/includes/198d8d6b-ecf6-47bc-a3dd-eaa2fe0544c5
```

### <a name="response"></a><span data-ttu-id="9f6f8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f6f8-134">Response</span></span>

<span data-ttu-id="9f6f8-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9f6f8-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
