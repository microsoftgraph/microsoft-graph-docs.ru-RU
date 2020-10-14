---
title: Создание Пермиссионгрантполици
description: Создает объект Пермиссионгрантполици, описывающий условия, при которых могут быть предоставлены разрешения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 4e6c268abee94f81db722249ad31fd97d1c62e48
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458661"
---
# <a name="create-permissiongrantpolicy"></a><span data-ttu-id="4d548-103">Создание Пермиссионгрантполици</span><span class="sxs-lookup"><span data-stu-id="4d548-103">Create permissionGrantPolicy</span></span>

<span data-ttu-id="4d548-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d548-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d548-105">Создает объект [пермиссионгрантполици](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4d548-105">Creates a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span> <span data-ttu-id="4d548-106">Политика предоставления разрешений используется для описания условий, при которых могут быть предоставлены разрешения (например, во время согласия приложения).</span><span class="sxs-lookup"><span data-stu-id="4d548-106">A permission grant policy is used to describe the conditions under which permissions can be granted (for example, during application consent).</span></span>

<span data-ttu-id="4d548-107">После создания политики предоставления разрешений можно [добавить наборы условий include](permissiongrantpolicy-post-includes.md) , чтобы добавить правила проверки совпадения, и [добавить наборы условий исключения](permissiongrantpolicy-post-excludes.md) для добавления правил исключения.</span><span class="sxs-lookup"><span data-stu-id="4d548-107">After creating the permission grant policy, you can [add include condition sets](permissiongrantpolicy-post-includes.md) to add matching rules, and [add exclude condition sets](permissiongrantpolicy-post-excludes.md) to add exclusion rules.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d548-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4d548-108">Permissions</span></span>

<span data-ttu-id="4d548-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d548-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d548-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d548-111">Permission type</span></span>      | <span data-ttu-id="4d548-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d548-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d548-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d548-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4d548-114">Пермиссионгрантполици. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4d548-114">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="4d548-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d548-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d548-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d548-116">Not supported.</span></span>    |
|<span data-ttu-id="4d548-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d548-117">Application</span></span> | <span data-ttu-id="4d548-118">Пермиссионгрантполици. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4d548-118">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d548-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d548-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /policies/permissionGrantPolicies
```

## <a name="request-headers"></a><span data-ttu-id="4d548-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d548-120">Request headers</span></span>

| <span data-ttu-id="4d548-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4d548-121">Name</span></span>       | <span data-ttu-id="4d548-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4d548-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="4d548-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d548-123">Authorization</span></span> | <span data-ttu-id="4d548-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d548-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4d548-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4d548-126">Content-type</span></span> | <span data-ttu-id="4d548-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d548-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d548-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d548-129">Request body</span></span>

<span data-ttu-id="4d548-130">В тексте запроса добавьте представление объекта [пермиссионгрантполици](../resources/permissiongrantpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d548-130">In the request body, supply a JSON representation of an [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4d548-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d548-131">Response</span></span>

<span data-ttu-id="4d548-132">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [пермиссионгрантполици](../resources/permissiongrantpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4d548-132">If successful, this method returns a `201 Created` response code and a [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4d548-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="4d548-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4d548-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d548-134">Request</span></span>

<span data-ttu-id="4d548-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d548-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4d548-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d548-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "create_permissiongrantpolicy"
}-->

```http
POST https://graph.microsoft.com/beta/policies/permissionGrantPolicies
Content-Type: application/json

{
  "id": "my-custom-consent-policy",
  "displayName": "Custom application consent policy",
  "description": "A custom permission grant policy to customize conditions for granting consent."
}
```
# <a name="c"></a>[<span data-ttu-id="4d548-137">C#</span><span class="sxs-lookup"><span data-stu-id="4d548-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d548-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d548-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d548-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d548-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4d548-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d548-140">Response</span></span>

<span data-ttu-id="4d548-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4d548-141">The following is an example of the response.</span></span>

> <span data-ttu-id="4d548-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d548-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "my-custom-consent-policy",
  "displayName": "Custom application consent policy",
  "description": "A custom permission grant policy to customize conditions for granting consent."
}
```
