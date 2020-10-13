---
title: Удаление Пермиссионгранткондитионсет из коллекции включенных элементов Пермиссионгрантполици
description: Удаляет включенный набор условий из политики предоставления разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 4fb9fb913698bcee6c788c3a6cbbd22eaf7db6c5
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433679"
---
# <a name="delete-permissiongrantconditionset-from-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="e3416-103">Удаление Пермиссионгранткондитионсет из коллекции включенных элементов Пермиссионгрантполици</span><span class="sxs-lookup"><span data-stu-id="e3416-103">Delete permissionGrantConditionSet from includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="e3416-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3416-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3416-105">Удаляет объект [пермиссионгранткондитионсет](../resources/permissiongrantconditionset.md) из коллекции **includes** объекта [пермиссионгрантполици](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="e3416-105">Deletes a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) from the **includes** collection of a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3416-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3416-106">Permissions</span></span>

<span data-ttu-id="e3416-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3416-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3416-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3416-109">Permission type</span></span>      | <span data-ttu-id="e3416-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3416-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="e3416-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3416-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e3416-112">Пермиссионгрантполици. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e3416-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
| <span data-ttu-id="e3416-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3416-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3416-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3416-114">Not supported.</span></span>    |
| <span data-ttu-id="e3416-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="e3416-115">Application</span></span> | <span data-ttu-id="e3416-116">Пермиссионгрантполици. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e3416-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3416-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3416-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{permissiongrantpolicy-id}/includes/{include-id}
```

## <a name="request-headers"></a><span data-ttu-id="e3416-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3416-118">Request headers</span></span>

| <span data-ttu-id="e3416-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e3416-119">Name</span></span>       | <span data-ttu-id="e3416-120">Тип</span><span class="sxs-lookup"><span data-stu-id="e3416-120">Type</span></span> | <span data-ttu-id="e3416-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e3416-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e3416-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3416-122">Authorization</span></span>  | <span data-ttu-id="e3416-123">string</span><span class="sxs-lookup"><span data-stu-id="e3416-123">string</span></span>  | <span data-ttu-id="e3416-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3416-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3416-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3416-126">Request body</span></span>

<span data-ttu-id="e3416-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3416-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3416-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3416-128">Response</span></span>

<span data-ttu-id="e3416-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e3416-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e3416-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="e3416-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e3416-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3416-132">Request</span></span>

<span data-ttu-id="e3416-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3416-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_delete_includes"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/permissionGrantPolicies/my-custom-consent-policy/includes/198d8d6b-ecf6-47bc-a3dd-eaa2fe0544c5
```

### <a name="response"></a><span data-ttu-id="e3416-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3416-134">Response</span></span>

<span data-ttu-id="e3416-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e3416-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
