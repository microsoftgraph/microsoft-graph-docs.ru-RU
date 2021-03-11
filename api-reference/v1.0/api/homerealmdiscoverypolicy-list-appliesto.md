---
title: Список применяетсяTo
description: Получите список объектов directoryObject, к которые был применен объект homeRealmDiscoveryPolicy.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 63844b2aacea4d9087500b2d33c797b7500078e5
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625950"
---
# <a name="list-appliesto"></a><span data-ttu-id="90dca-103">Список применяетсяTo</span><span class="sxs-lookup"><span data-stu-id="90dca-103">List appliesTo</span></span>

<span data-ttu-id="90dca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90dca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="90dca-105">Получите список объектов [directoryObject,](../resources/directoryObject.md) к которые был применен [объект homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="90dca-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object has been applied to.</span></span>

## <a name="permissions"></a><span data-ttu-id="90dca-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90dca-106">Permissions</span></span>

<span data-ttu-id="90dca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90dca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90dca-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90dca-109">Permission type</span></span>                        | <span data-ttu-id="90dca-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90dca-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="90dca-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90dca-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="90dca-112">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="90dca-112">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="90dca-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90dca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90dca-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90dca-114">Not supported.</span></span> |
| <span data-ttu-id="90dca-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90dca-115">Application</span></span>                            | <span data-ttu-id="90dca-116">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="90dca-116">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90dca-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90dca-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="90dca-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="90dca-118">Optional query parameters</span></span>

<span data-ttu-id="90dca-119">Этот метод поддерживает параметры `$select` `$top` запроса oData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="90dca-119">This method supports the `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="90dca-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="90dca-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="90dca-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90dca-121">Request headers</span></span>

| <span data-ttu-id="90dca-122">Имя</span><span class="sxs-lookup"><span data-stu-id="90dca-122">Name</span></span>      |<span data-ttu-id="90dca-123">Описание</span><span class="sxs-lookup"><span data-stu-id="90dca-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="90dca-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90dca-124">Authorization</span></span> | <span data-ttu-id="90dca-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90dca-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90dca-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90dca-127">Request body</span></span>

<span data-ttu-id="90dca-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90dca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90dca-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="90dca-129">Response</span></span>

<span data-ttu-id="90dca-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90dca-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="90dca-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="90dca-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="90dca-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="90dca-132">Request</span></span>

<span data-ttu-id="90dca-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90dca-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="90dca-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="90dca-134">Response</span></span>

<span data-ttu-id="90dca-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="90dca-135">The following is an example of the response.</span></span>

> <span data-ttu-id="90dca-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90dca-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
