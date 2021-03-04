---
title: Список применяетсяTo
description: Получите список объектов directoryObject, к которые был применен объект tokenIssuancePolicy.
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 95e31f704a41250c73f5dc13b5a0e06abc6c47f9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443442"
---
# <a name="list-appliesto"></a><span data-ttu-id="ae244-103">Список применяетсяTo</span><span class="sxs-lookup"><span data-stu-id="ae244-103">List appliesTo</span></span>

<span data-ttu-id="ae244-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae244-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae244-105">Получите список объектов [directoryObject,](../resources/directoryObject.md) к которые был применен [объект tokenIssuancePolicy.](../resources/tokenissuancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="ae244-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object has been applied to.</span></span> <span data-ttu-id="ae244-106">TokenIssuancePolicy может применяться только к ресурсам [приложения](../resources/application.md) и [servicePrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="ae244-106">The tokenIssuancePolicy can only be applied to [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae244-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae244-107">Permissions</span></span>

<span data-ttu-id="ae244-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae244-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ae244-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae244-110">Permission type</span></span>                        | <span data-ttu-id="ae244-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae244-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ae244-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae244-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ae244-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae244-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="ae244-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae244-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae244-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae244-115">Not supported.</span></span> |
| <span data-ttu-id="ae244-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ae244-116">Application</span></span>                            | <span data-ttu-id="ae244-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae244-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae244-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae244-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenIssuancePolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae244-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ae244-119">Optional query parameters</span></span>

<span data-ttu-id="ae244-120">Этот метод поддерживает параметры `$expand` `$select` запроса OData и OData для настройки `$top` ответа.</span><span class="sxs-lookup"><span data-stu-id="ae244-120">This method supports the `$expand`, `$select`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="ae244-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ae244-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="ae244-122">При использовании убедитесь, что ваше приложение запрашивает `$expand` разрешения на чтение расширенных объектов.</span><span class="sxs-lookup"><span data-stu-id="ae244-122">When using `$expand`, make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae244-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae244-123">Request headers</span></span>

| <span data-ttu-id="ae244-124">Имя</span><span class="sxs-lookup"><span data-stu-id="ae244-124">Name</span></span>      |<span data-ttu-id="ae244-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ae244-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ae244-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae244-126">Authorization</span></span> | <span data-ttu-id="ae244-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae244-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae244-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ae244-129">Request body</span></span>

<span data-ttu-id="ae244-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ae244-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae244-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae244-131">Response</span></span>

<span data-ttu-id="ae244-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ae244-132">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ae244-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="ae244-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ae244-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae244-134">Request</span></span>

<span data-ttu-id="ae244-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae244-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/beta/tokenIssuancePolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="ae244-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae244-136">Response</span></span>

<span data-ttu-id="ae244-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ae244-137">The following is an example of the response.</span></span>

> <span data-ttu-id="ae244-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae244-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


