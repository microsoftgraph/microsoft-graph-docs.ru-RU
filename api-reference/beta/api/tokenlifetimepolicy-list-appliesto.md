---
title: Список применяетсяTo
description: Получите список объектов directoryObject, к которые был применен объект tokenLifetimePolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ac3df91789bb0be148ace7b5e26d94f8c34fae75
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443344"
---
# <a name="list-appliesto"></a><span data-ttu-id="01850-103">Список применяетсяTo</span><span class="sxs-lookup"><span data-stu-id="01850-103">List appliesTo</span></span>

<span data-ttu-id="01850-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01850-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01850-105">Получите список объектов [directoryObject,](../resources/directoryObject.md) к которые был применен [объект tokenLifetimePolicy.](../resources/tokenlifetimepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="01850-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object has been applied to.</span></span> <span data-ttu-id="01850-106">TokenLifetimePolicy может применяться только к ресурсам [приложения](../resources/application.md) и [servicePrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="01850-106">The tokenLifetimePolicy can only be applied to [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="01850-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01850-107">Permissions</span></span>

<span data-ttu-id="01850-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01850-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01850-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01850-110">Permission type</span></span>                        | <span data-ttu-id="01850-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01850-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="01850-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01850-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="01850-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="01850-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="01850-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01850-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01850-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01850-115">Not supported.</span></span> |
| <span data-ttu-id="01850-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="01850-116">Application</span></span>                            | <span data-ttu-id="01850-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="01850-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01850-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01850-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenLifetimePolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="01850-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="01850-119">Optional query parameters</span></span>

<span data-ttu-id="01850-120">Этот метод поддерживает параметры `$expand` `$select` `$top` запроса OData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="01850-120">This method supports the `$expand`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="01850-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="01850-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="01850-122">При использовании `$expand` убедитесь, что приложение запрашивает разрешения на чтение расширенных объектов.</span><span class="sxs-lookup"><span data-stu-id="01850-122">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01850-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01850-123">Request headers</span></span>

| <span data-ttu-id="01850-124">Имя</span><span class="sxs-lookup"><span data-stu-id="01850-124">Name</span></span>      |<span data-ttu-id="01850-125">Описание</span><span class="sxs-lookup"><span data-stu-id="01850-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="01850-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="01850-126">Authorization</span></span> | <span data-ttu-id="01850-127">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="01850-127">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="01850-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01850-128">Request body</span></span>

<span data-ttu-id="01850-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01850-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01850-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="01850-130">Response</span></span>

<span data-ttu-id="01850-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01850-131">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="01850-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="01850-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="01850-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="01850-133">Request</span></span>

<span data-ttu-id="01850-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01850-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/beta/tokenLifetimePolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="01850-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="01850-135">Response</span></span>

<span data-ttu-id="01850-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="01850-136">The following is an example of the response.</span></span>

> <span data-ttu-id="01850-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01850-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

