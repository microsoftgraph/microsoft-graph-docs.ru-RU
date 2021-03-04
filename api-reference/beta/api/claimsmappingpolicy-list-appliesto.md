---
title: Список применяетсяTo
description: Получите список объектов directoryObject, к которые был применен объект claimsMappingPolicy.
localization_priority: Normal
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9eb488b931cb5ff89796526f1285fa5454a5bae8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437690"
---
# <a name="list-appliesto"></a><span data-ttu-id="762a4-103">Список применяетсяTo</span><span class="sxs-lookup"><span data-stu-id="762a4-103">List appliesTo</span></span>

<span data-ttu-id="762a4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="762a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="762a4-105">Получите список объектов [directoryObject,](../resources/directoryObject.md) к которые был применен объект [claimsMappingPolicy.](../resources/claimsmappingpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="762a4-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object has been applied to.</span></span> <span data-ttu-id="762a4-106">ТребованияMappingPolicy можно применять только к ресурсам [приложения](../resources/application.md) и [servicePrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="762a4-106">The claimsMappingPolicy can only be applied to [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="762a4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="762a4-107">Permissions</span></span>

<span data-ttu-id="762a4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="762a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="762a4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="762a4-110">Permission type</span></span>                        | <span data-ttu-id="762a4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="762a4-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="762a4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="762a4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="762a4-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="762a4-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="762a4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="762a4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="762a4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="762a4-115">Not supported.</span></span> |
| <span data-ttu-id="762a4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="762a4-116">Application</span></span>                            | <span data-ttu-id="762a4-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="762a4-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="762a4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="762a4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/claimsMappingPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="762a4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="762a4-119">Optional query parameters</span></span>

<span data-ttu-id="762a4-120">Этот метод поддерживает параметры `$expand` `$select` `$top` запроса OData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="762a4-120">This method supports the `$expand`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="762a4-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="762a4-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="762a4-122">При использовании `$expand` убедитесь, что приложение запрашивает разрешения на чтение расширенных объектов.</span><span class="sxs-lookup"><span data-stu-id="762a4-122">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="762a4-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="762a4-123">Request headers</span></span>

| <span data-ttu-id="762a4-124">Имя</span><span class="sxs-lookup"><span data-stu-id="762a4-124">Name</span></span>      |<span data-ttu-id="762a4-125">Описание</span><span class="sxs-lookup"><span data-stu-id="762a4-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="762a4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="762a4-126">Authorization</span></span> | <span data-ttu-id="762a4-127">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="762a4-127">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="762a4-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="762a4-128">Request body</span></span>

<span data-ttu-id="762a4-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="762a4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="762a4-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="762a4-130">Response</span></span>

<span data-ttu-id="762a4-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="762a4-131">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="762a4-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="762a4-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="762a4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="762a4-133">Request</span></span>

<span data-ttu-id="762a4-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="762a4-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/beta/claimsMappingPolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="762a4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="762a4-135">Response</span></span>

<span data-ttu-id="762a4-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="762a4-136">The following is an example of the response.</span></span>

> <span data-ttu-id="762a4-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="762a4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

