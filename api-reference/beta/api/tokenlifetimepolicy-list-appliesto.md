---
title: Список appliesTo
description: Получение списка объектов directoryObject, к которым был применен объект Токенлифетимеполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ec486f79c1f9c61c606c5630aa7810480a1d2b81
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234505"
---
# <a name="list-appliesto"></a><span data-ttu-id="ececc-103">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="ececc-103">List appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ececc-104">Получение списка объектов [directoryObject](../resources/directoryObject.md) , к которым был применен объект [токенлифетимеполици](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ececc-104">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object has been applied to.</span></span> <span data-ttu-id="ececc-105">Токенлифетимеполици можно применять только к ресурсам [Application](../resources/application.md) и [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="ececc-105">The tokenLifetimePolicy can only be applied to [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="ececc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ececc-106">Permissions</span></span>

<span data-ttu-id="ececc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ececc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ececc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ececc-109">Permission type</span></span>                        | <span data-ttu-id="ececc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ececc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ececc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ececc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ececc-112">Policy. Read. ALL и Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="ececc-112">Policy.Read.All and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="ececc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ececc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ececc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ececc-114">Not supported.</span></span> |
| <span data-ttu-id="ececc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ececc-115">Application</span></span>                            | <span data-ttu-id="ececc-116">Policy. Read. ALL и Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="ececc-116">Policy.Read.All and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ececc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ececc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenLifetimePolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ececc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ececc-118">Optional query parameters</span></span>

<span data-ttu-id="ececc-119">Этот метод поддерживает `$expand`параметры запросов `$select` OData `$top` и OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ececc-119">This method supports the `$expand`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="ececc-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ececc-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="ececc-121">При использовании `$expand` убедитесь, что приложение запрашивает разрешения на чтение развернутых объектов.</span><span class="sxs-lookup"><span data-stu-id="ececc-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ececc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ececc-122">Request headers</span></span>

| <span data-ttu-id="ececc-123">Имя</span><span class="sxs-lookup"><span data-stu-id="ececc-123">Name</span></span>      |<span data-ttu-id="ececc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ececc-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ececc-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ececc-125">Authorization</span></span> | <span data-ttu-id="ececc-126">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="ececc-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ececc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ececc-127">Request body</span></span>

<span data-ttu-id="ececc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ececc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ececc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ececc-129">Response</span></span>

<span data-ttu-id="ececc-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ececc-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ececc-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="ececc-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ececc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ececc-132">Request</span></span>

<span data-ttu-id="ececc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ececc-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/beta/tokenLifetimePolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="ececc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ececc-134">Response</span></span>

<span data-ttu-id="ececc-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ececc-135">The following is an example of the response.</span></span>

> <span data-ttu-id="ececc-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ececc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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