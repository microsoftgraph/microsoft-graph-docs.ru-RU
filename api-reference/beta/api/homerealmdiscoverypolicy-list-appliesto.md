---
title: Список appliesTo
description: Получение списка объектов directoryObject, к которым был применен объект Хомереалмдисковериполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 369a852668e56794311bafb2c53b0e692ad3efd4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446540"
---
# <a name="list-appliesto"></a><span data-ttu-id="291e0-103">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="291e0-103">List appliesTo</span></span>

<span data-ttu-id="291e0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="291e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="291e0-105">Получение списка объектов [directoryObject](../resources/directoryObject.md) , к которым был применен объект [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="291e0-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object has been applied to.</span></span> <span data-ttu-id="291e0-106">Хомереалмдисковериполици можно применять только к ресурсам [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="291e0-106">The homeRealmDiscoveryPolicy can only be applied to [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="291e0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="291e0-107">Permissions</span></span>

<span data-ttu-id="291e0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="291e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="291e0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="291e0-110">Permission type</span></span>                        | <span data-ttu-id="291e0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="291e0-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="291e0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="291e0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="291e0-113">Policy. Read. ALL и Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="291e0-113">Policy.Read.All and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="291e0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="291e0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="291e0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="291e0-115">Not supported.</span></span> |
| <span data-ttu-id="291e0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="291e0-116">Application</span></span>                            | <span data-ttu-id="291e0-117">Policy. Read. ALL и Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="291e0-117">Policy.Read.All and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="291e0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="291e0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="291e0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="291e0-119">Optional query parameters</span></span>

<span data-ttu-id="291e0-120">Этот метод поддерживает параметры `$select` запросов `$top` OData и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="291e0-120">This method supports the `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="291e0-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="291e0-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="291e0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="291e0-122">Request headers</span></span>

| <span data-ttu-id="291e0-123">Имя</span><span class="sxs-lookup"><span data-stu-id="291e0-123">Name</span></span>      |<span data-ttu-id="291e0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="291e0-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="291e0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="291e0-125">Authorization</span></span> | <span data-ttu-id="291e0-126">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="291e0-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="291e0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="291e0-127">Request body</span></span>

<span data-ttu-id="291e0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="291e0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="291e0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="291e0-129">Response</span></span>

<span data-ttu-id="291e0-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="291e0-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="291e0-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="291e0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="291e0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="291e0-132">Request</span></span>

<span data-ttu-id="291e0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="291e0-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/beta/homeRealmDiscoveryPolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="291e0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="291e0-134">Response</span></span>

<span data-ttu-id="291e0-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="291e0-135">The following is an example of the response.</span></span>

> <span data-ttu-id="291e0-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="291e0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "deletedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->