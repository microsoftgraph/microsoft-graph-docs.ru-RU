---
title: Список назначенных ТокенлифетимеполиЦиес
description: Список ТокенлифетимеполиЦиес, назначенных приложению или servicePrincipal.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1aab750ef0d2121634343ef9c371bae1645744e1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441503"
---
# <a name="list-assigned-tokenlifetimepolicy"></a><span data-ttu-id="37719-103">Список назначенных Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="37719-103">List assigned tokenLifetimePolicy</span></span>

<span data-ttu-id="37719-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="37719-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37719-105">Перечисление объектов [токенлифетимеполици](../resources/tokenlifetimepolicy.md) , назначенных [приложению](../resources/application.md) или [servicePrincipal](../resources/servicePrincipal.md)..</span><span class="sxs-lookup"><span data-stu-id="37719-105">List the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects that are assigned to an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md)..</span></span>

## <a name="permissions"></a><span data-ttu-id="37719-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="37719-106">Permissions</span></span>

<span data-ttu-id="37719-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37719-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="37719-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37719-109">Permission type</span></span>                        | <span data-ttu-id="37719-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37719-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="37719-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37719-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="37719-112">Policy. Read. ALL и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="37719-112">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="37719-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37719-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37719-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37719-114">Not supported.</span></span> |
| <span data-ttu-id="37719-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37719-115">Application</span></span>                            | <span data-ttu-id="37719-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="37719-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37719-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37719-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenLifetimePolicies
GET /servicePrincipals/{id}/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="37719-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37719-118">Request headers</span></span>

| <span data-ttu-id="37719-119">Имя</span><span class="sxs-lookup"><span data-stu-id="37719-119">Name</span></span>          | <span data-ttu-id="37719-120">Описание</span><span class="sxs-lookup"><span data-stu-id="37719-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="37719-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="37719-121">Authorization</span></span> | <span data-ttu-id="37719-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="37719-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="37719-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37719-123">Request body</span></span>

<span data-ttu-id="37719-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="37719-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37719-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="37719-125">Response</span></span>

<span data-ttu-id="37719-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [токенлифетимеполици](../resources/tokenLifetimePolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="37719-126">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenLifetimePolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37719-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="37719-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="37719-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="37719-128">Request</span></span>

<span data-ttu-id="37719-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37719-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37719-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="37719-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenlifetimepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies
```
# <a name="c"></a>[<span data-ttu-id="37719-131">C#</span><span class="sxs-lookup"><span data-stu-id="37719-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tokenlifetimepolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37719-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37719-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tokenlifetimepolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37719-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37719-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tokenlifetimepolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="37719-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="37719-134">Response</span></span>

<span data-ttu-id="37719-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="37719-135">The following is an example of the response.</span></span>

> <span data-ttu-id="37719-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37719-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
