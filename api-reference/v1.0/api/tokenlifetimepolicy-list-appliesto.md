---
title: Список appliesTo
description: Получение списка объектов directoryObject, к которым был применен объект Токенлифетимеполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 65929050debc61bdfed18378c50ffd93b4514624
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229565"
---
# <a name="list-appliesto"></a><span data-ttu-id="4c3f3-103">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="4c3f3-103">List appliesTo</span></span>

<span data-ttu-id="4c3f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c3f3-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="4c3f3-105">Получение списка объектов [directoryObject](../resources/directoryObject.md) , к которым был применен объект [токенлифетимеполици](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="4c3f3-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object has been applied to.</span></span> <span data-ttu-id="4c3f3-106">Токенлифетимеполици можно применить только к [приложению](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="4c3f3-106">The tokenLifetimePolicy can only be applied to [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c3f3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c3f3-107">Permissions</span></span>

<span data-ttu-id="4c3f3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c3f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c3f3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c3f3-110">Permission type</span></span>                        | <span data-ttu-id="4c3f3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c3f3-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4c3f3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c3f3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c3f3-113">Policy. Read. ALL и Application. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="4c3f3-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="4c3f3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c3f3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c3f3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c3f3-115">Not supported.</span></span> |
| <span data-ttu-id="4c3f3-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4c3f3-116">Application</span></span>                            | <span data-ttu-id="4c3f3-117">Policy. Read. ALL и Application. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="4c3f3-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c3f3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c3f3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenLifetimePolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4c3f3-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4c3f3-119">Optional query parameters</span></span>

<span data-ttu-id="4c3f3-120">Этот метод поддерживает `$expand`параметры запросов `$select` OData `$top` и OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4c3f3-120">This method supports the `$expand`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="4c3f3-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4c3f3-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="4c3f3-122">При использовании `$expand` убедитесь, что приложение запрашивает разрешения на чтение развернутых объектов.</span><span class="sxs-lookup"><span data-stu-id="4c3f3-122">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c3f3-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c3f3-123">Request headers</span></span>

| <span data-ttu-id="4c3f3-124">Имя</span><span class="sxs-lookup"><span data-stu-id="4c3f3-124">Name</span></span>      |<span data-ttu-id="4c3f3-125">Описание</span><span class="sxs-lookup"><span data-stu-id="4c3f3-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4c3f3-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c3f3-126">Authorization</span></span> | <span data-ttu-id="4c3f3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c3f3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c3f3-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c3f3-129">Request body</span></span>

<span data-ttu-id="4c3f3-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c3f3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c3f3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c3f3-131">Response</span></span>

<span data-ttu-id="4c3f3-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c3f3-132">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4c3f3-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="4c3f3-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4c3f3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c3f3-134">Request</span></span>

<span data-ttu-id="4c3f3-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c3f3-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="4c3f3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c3f3-136">Response</span></span>

<span data-ttu-id="4c3f3-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4c3f3-137">The following is an example of the response.</span></span>

> <span data-ttu-id="4c3f3-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c3f3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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