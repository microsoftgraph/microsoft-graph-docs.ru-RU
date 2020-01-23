---
title: Назначение типа ресурса tokenLifetimePolicy
description: Назначьте Токенлифетимеполици для приложения или участника службы.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fca668417d52914194ef087a32b28478101a32d7
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475623"
---
# <a name="assign-tokenlifetimepolicy"></a><span data-ttu-id="c1b60-103">Назначение типа ресурса tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="c1b60-103">Assign tokenLifetimePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1b60-104">Назначьте [токенлифетимеполици](../resources/tokenlifetimepolicy.md) [приложению](../resources/application.md) или [servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="c1b60-104">Assign a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) to an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c1b60-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1b60-105">Permissions</span></span>

<span data-ttu-id="c1b60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1b60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1b60-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1b60-108">Permission type</span></span>                        | <span data-ttu-id="c1b60-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1b60-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c1b60-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1b60-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1b60-111">Policy. Read. ALL и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c1b60-111">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="c1b60-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1b60-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1b60-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1b60-113">Not supported.</span></span> |
| <span data-ttu-id="c1b60-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1b60-114">Application</span></span>                            | <span data-ttu-id="c1b60-115">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c1b60-115">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1b60-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1b60-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/tokenLifetimePolicies/$ref
POST /servicePrincipals/{id}/tokenLifetimePolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="c1b60-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1b60-117">Request headers</span></span>

| <span data-ttu-id="c1b60-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c1b60-118">Name</span></span>          | <span data-ttu-id="c1b60-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c1b60-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c1b60-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1b60-120">Authorization</span></span> | <span data-ttu-id="c1b60-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="c1b60-121">Bearer {token}</span></span> |
| <span data-ttu-id="c1b60-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1b60-122">Content-Type</span></span> | <span data-ttu-id="c1b60-123">application/json</span><span class="sxs-lookup"><span data-stu-id="c1b60-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1b60-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c1b60-124">Request body</span></span>

<span data-ttu-id="c1b60-125">В тексте запроса укажите идентификатор объекта [токенлифетимеполици](../resources/tokenlifetimepolicy.md) (с помощью `@odata.id` свойства), который должен быть назначен для приложения или участника-службы.</span><span class="sxs-lookup"><span data-stu-id="c1b60-125">In the request body, supply the identifier of the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object (using an `@odata.id` property) that should be assigned to the application or service principal.</span></span>

## <a name="response"></a><span data-ttu-id="c1b60-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1b60-126">Response</span></span>

<span data-ttu-id="c1b60-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c1b60-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c1b60-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="c1b60-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c1b60-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1b60-130">Request</span></span>

<span data-ttu-id="c1b60-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1b60-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c1b60-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1b60-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_application"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1b60-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1b60-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenlifetimepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c1b60-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1b60-134">Response</span></span>

<span data-ttu-id="c1b60-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c1b60-135">The following is an example of the response.</span></span>

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
