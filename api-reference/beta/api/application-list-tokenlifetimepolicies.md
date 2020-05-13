---
title: Список назначенных ТокенлифетимеполиЦиес
description: Список ТокенлифетимеполиЦиес, назначенных приложению или servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7c0523d501dd6b77bc5808b0f936f6692b12951b
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "43107236"
---
# <a name="list-assigned-tokenlifetimepolicy"></a><span data-ttu-id="44e32-103">Список назначенных Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="44e32-103">List assigned tokenLifetimePolicy</span></span>

<span data-ttu-id="44e32-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44e32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44e32-105">Перечисление объектов [токенлифетимеполици](../resources/tokenlifetimepolicy.md) , назначенных [приложению](../resources/application.md) или [servicePrincipal](../resources/servicePrincipal.md)..</span><span class="sxs-lookup"><span data-stu-id="44e32-105">List the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects that are assigned to an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md)..</span></span>

## <a name="permissions"></a><span data-ttu-id="44e32-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44e32-106">Permissions</span></span>

<span data-ttu-id="44e32-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44e32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44e32-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44e32-109">Permission type</span></span>                        | <span data-ttu-id="44e32-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44e32-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="44e32-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44e32-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="44e32-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="44e32-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="44e32-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44e32-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44e32-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44e32-114">Not supported.</span></span> |
| <span data-ttu-id="44e32-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44e32-115">Application</span></span>                            | <span data-ttu-id="44e32-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="44e32-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44e32-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44e32-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenLifetimePolicies
GET /servicePrincipals/{id}/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="44e32-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44e32-118">Request headers</span></span>

| <span data-ttu-id="44e32-119">Имя</span><span class="sxs-lookup"><span data-stu-id="44e32-119">Name</span></span>          | <span data-ttu-id="44e32-120">Описание</span><span class="sxs-lookup"><span data-stu-id="44e32-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="44e32-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="44e32-121">Authorization</span></span> | <span data-ttu-id="44e32-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="44e32-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="44e32-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44e32-123">Request body</span></span>

<span data-ttu-id="44e32-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="44e32-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44e32-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="44e32-125">Response</span></span>

<span data-ttu-id="44e32-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [токенлифетимеполици](../resources/tokenLifetimePolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44e32-126">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenLifetimePolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="44e32-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="44e32-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="44e32-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="44e32-128">Request</span></span>

<span data-ttu-id="44e32-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44e32-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="44e32-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="44e32-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenlifetimepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies
```
# <a name="c"></a>[<span data-ttu-id="44e32-131">C#</span><span class="sxs-lookup"><span data-stu-id="44e32-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tokenlifetimepolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44e32-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44e32-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tokenlifetimepolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44e32-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44e32-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tokenlifetimepolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="44e32-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="44e32-134">Response</span></span>

<span data-ttu-id="44e32-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="44e32-135">The following is an example of the response.</span></span>

> <span data-ttu-id="44e32-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44e32-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List assigned tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
