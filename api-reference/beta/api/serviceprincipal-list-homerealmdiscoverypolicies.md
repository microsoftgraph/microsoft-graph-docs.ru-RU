---
title: Список назначенных ХомереалмдисковериполиЦиес
description: Список ХомереалмдисковериполиЦиес, назначенных для servicePrincipal.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ce4d82ae36a7451c44e266f02953b7e7b7705090
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234490"
---
# <a name="list-assigned-homerealmdiscoverypolicy"></a><span data-ttu-id="69168-103">Список назначенных Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="69168-103">List assigned homeRealmDiscoveryPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69168-104">Перечисление объектов [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) , назначенных для [servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="69168-104">List the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects that are assigned to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="69168-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69168-105">Permissions</span></span>

<span data-ttu-id="69168-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69168-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="69168-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69168-108">Permission type</span></span>                        | <span data-ttu-id="69168-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69168-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="69168-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69168-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="69168-111">Policy. Read. ALL и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="69168-111">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="69168-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69168-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69168-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69168-113">Not supported.</span></span> |
| <span data-ttu-id="69168-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69168-114">Application</span></span>                            | <span data-ttu-id="69168-115">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="69168-115">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69168-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69168-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="69168-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69168-117">Request headers</span></span>

| <span data-ttu-id="69168-118">Имя</span><span class="sxs-lookup"><span data-stu-id="69168-118">Name</span></span>          | <span data-ttu-id="69168-119">Описание</span><span class="sxs-lookup"><span data-stu-id="69168-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="69168-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69168-120">Authorization</span></span> | <span data-ttu-id="69168-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="69168-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="69168-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69168-122">Request body</span></span>

<span data-ttu-id="69168-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="69168-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69168-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="69168-124">Response</span></span>

<span data-ttu-id="69168-125">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [хомереалмдисковериполици](../resources/homeRealmDiscoveryPolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="69168-125">If successful, this method returns a `200 OK` response code and a collection of [homeRealmDiscoveryPolicy](../resources/homeRealmDiscoveryPolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69168-126">Пример</span><span class="sxs-lookup"><span data-stu-id="69168-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="69168-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="69168-127">Request</span></span>

<span data-ttu-id="69168-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69168-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_homerealmdiscoverypolicies_on_serviceprincipal"
}-->

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/homeRealmDiscoveryPolicies
```

### <a name="response"></a><span data-ttu-id="69168-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="69168-129">Response</span></span>

<span data-ttu-id="69168-130">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="69168-130">The following is an example of the response.</span></span>

> <span data-ttu-id="69168-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69168-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
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
  "description": "List assigned homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->