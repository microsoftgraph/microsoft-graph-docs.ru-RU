---
title: Назначение типа ресурса tokenLifetimePolicy
description: Назначьте Токенлифетимеполици приложению.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3f10ee2a69d2546f8320277d58025b99c2c8a3c5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968320"
---
# <a name="assign-tokenlifetimepolicy"></a><span data-ttu-id="d2224-103">Назначение типа ресурса tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="d2224-103">Assign tokenLifetimePolicy</span></span>

<span data-ttu-id="d2224-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2224-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="d2224-105">Назначьте [токенлифетимеполици](../resources/tokenlifetimepolicy.md) [приложению](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="d2224-105">Assign a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d2224-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2224-106">Permissions</span></span>

<span data-ttu-id="d2224-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2224-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2224-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2224-109">Permission type</span></span>                        | <span data-ttu-id="d2224-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2224-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d2224-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2224-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2224-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d2224-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="d2224-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2224-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2224-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2224-114">Not supported.</span></span> |
| <span data-ttu-id="d2224-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2224-115">Application</span></span>                            | <span data-ttu-id="d2224-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d2224-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2224-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2224-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/tokenLifetimePolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="d2224-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2224-118">Request headers</span></span>

| <span data-ttu-id="d2224-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d2224-119">Name</span></span>          | <span data-ttu-id="d2224-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d2224-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d2224-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2224-121">Authorization</span></span> | <span data-ttu-id="d2224-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2224-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2224-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2224-124">Content-Type</span></span> | <span data-ttu-id="d2224-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2224-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2224-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2224-127">Request body</span></span>

<span data-ttu-id="d2224-128">В тексте запроса укажите идентификатор объекта [токенлифетимеполици](../resources/tokenlifetimepolicy.md) (с помощью `@odata.id` Свойства), который должен быть назначен для приложения или участника-службы.</span><span class="sxs-lookup"><span data-stu-id="d2224-128">In the request body, supply the identifier of the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object (using an `@odata.id` property) that should be assigned to the application or service principal.</span></span>

## <a name="response"></a><span data-ttu-id="d2224-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2224-129">Response</span></span>

<span data-ttu-id="d2224-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d2224-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d2224-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="d2224-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d2224-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2224-133">Request</span></span>

<span data-ttu-id="d2224-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2224-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d2224-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2224-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_application"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/tokenLifetimePolicies/$ref
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="c"></a>[<span data-ttu-id="d2224-136">C#</span><span class="sxs-lookup"><span data-stu-id="d2224-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenlifetimepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2224-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2224-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenlifetimepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2224-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2224-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenlifetimepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2224-139">Java</span><span class="sxs-lookup"><span data-stu-id="d2224-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tokenlifetimepolicy-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d2224-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2224-140">Response</span></span>

<span data-ttu-id="d2224-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d2224-141">The following is an example of the response.</span></span>

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
  "description": "Assign tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

