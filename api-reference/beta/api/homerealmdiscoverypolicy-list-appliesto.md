---
title: Список appliesTo
description: Получение списка объектов directoryObject, к которым был применен объект Хомереалмдисковериполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a8166c54c6ad62f2add344e4bd4ffd318b668af4
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234473"
---
# <a name="list-appliesto"></a><span data-ttu-id="eafad-103">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="eafad-103">List appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eafad-104">Получение списка объектов [directoryObject](../resources/directoryObject.md) , к которым был применен объект [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="eafad-104">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object has been applied to.</span></span> <span data-ttu-id="eafad-105">Хомереалмдисковериполици можно применять только к ресурсам [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="eafad-105">The homeRealmDiscoveryPolicy can only be applied to [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="eafad-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eafad-106">Permissions</span></span>

<span data-ttu-id="eafad-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eafad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eafad-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eafad-109">Permission type</span></span>                        | <span data-ttu-id="eafad-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eafad-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="eafad-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eafad-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="eafad-112">Policy. Read. ALL и Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="eafad-112">Policy.Read.All and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="eafad-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eafad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eafad-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eafad-114">Not supported.</span></span> |
| <span data-ttu-id="eafad-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eafad-115">Application</span></span>                            | <span data-ttu-id="eafad-116">Policy. Read. ALL и Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="eafad-116">Policy.Read.All and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eafad-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eafad-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eafad-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eafad-118">Optional query parameters</span></span>

<span data-ttu-id="eafad-119">Этот метод поддерживает параметры `$select` запросов `$top` OData и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="eafad-119">This method supports the `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="eafad-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="eafad-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="eafad-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eafad-121">Request headers</span></span>

| <span data-ttu-id="eafad-122">Имя</span><span class="sxs-lookup"><span data-stu-id="eafad-122">Name</span></span>      |<span data-ttu-id="eafad-123">Описание</span><span class="sxs-lookup"><span data-stu-id="eafad-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eafad-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eafad-124">Authorization</span></span> | <span data-ttu-id="eafad-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="eafad-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="eafad-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eafad-126">Request body</span></span>

<span data-ttu-id="eafad-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eafad-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eafad-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="eafad-128">Response</span></span>

<span data-ttu-id="eafad-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eafad-129">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eafad-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="eafad-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eafad-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="eafad-131">Request</span></span>

<span data-ttu-id="eafad-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eafad-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/beta/homeRealmDiscoveryPolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="eafad-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="eafad-133">Response</span></span>

<span data-ttu-id="eafad-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eafad-134">The following is an example of the response.</span></span>

> <span data-ttu-id="eafad-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eafad-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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