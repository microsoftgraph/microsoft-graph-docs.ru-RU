---
title: Список appliesTo
description: Получение списка объектов directoryObject, к которым был применен объект Клаимсмаппингполици.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f749b040da90537ad362fe1d372ae6d090327039
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982530"
---
# <a name="list-appliesto"></a><span data-ttu-id="f329c-103">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="f329c-103">List appliesTo</span></span>

<span data-ttu-id="f329c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f329c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f329c-105">Получение списка объектов [directoryObject](../resources/directoryObject.md) , к которым был применен объект [клаимсмаппингполици](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="f329c-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object has been applied to.</span></span> <span data-ttu-id="f329c-106">Клаимсмаппингполици можно применять только к ресурсам [Application](../resources/application.md) и [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="f329c-106">The claimsMappingPolicy can only be applied to [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="f329c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f329c-107">Permissions</span></span>

<span data-ttu-id="f329c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f329c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f329c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f329c-110">Permission type</span></span>                        | <span data-ttu-id="f329c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f329c-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f329c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f329c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f329c-113">Policy. Read. ALL и Application. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="f329c-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="f329c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f329c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f329c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f329c-115">Not supported.</span></span> |
| <span data-ttu-id="f329c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f329c-116">Application</span></span>                            | <span data-ttu-id="f329c-117">Policy. Read. ALL и Application. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="f329c-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f329c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f329c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/claimsMappingPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f329c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f329c-119">Optional query parameters</span></span>

<span data-ttu-id="f329c-120">Этот метод поддерживает `$expand` `$select` `$top` параметры запросов OData и OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f329c-120">This method supports the `$expand`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="f329c-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f329c-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="f329c-122">При использовании `$expand` Убедитесь, что приложение запрашивает разрешения на чтение развернутых объектов.</span><span class="sxs-lookup"><span data-stu-id="f329c-122">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f329c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f329c-123">Request headers</span></span>

| <span data-ttu-id="f329c-124">Имя</span><span class="sxs-lookup"><span data-stu-id="f329c-124">Name</span></span>      |<span data-ttu-id="f329c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f329c-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f329c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f329c-126">Authorization</span></span> | <span data-ttu-id="f329c-127">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="f329c-127">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f329c-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f329c-128">Request body</span></span>

<span data-ttu-id="f329c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f329c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f329c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f329c-130">Response</span></span>

<span data-ttu-id="f329c-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f329c-131">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f329c-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="f329c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f329c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f329c-133">Request</span></span>

<span data-ttu-id="f329c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f329c-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/beta/claimsMappingPolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="f329c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f329c-135">Response</span></span>

<span data-ttu-id="f329c-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f329c-136">The following is an example of the response.</span></span>

> <span data-ttu-id="f329c-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f329c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

