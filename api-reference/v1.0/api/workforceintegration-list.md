---
title: Список Воркфорцеинтегратионс
description: Получение списка объектов Воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1879feab262460878b2753be8080fbbab66ebfe4
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/04/2020
ms.locfileid: "44217576"
---
# <a name="list-workforceintegrations"></a><span data-ttu-id="d047b-103">Список Воркфорцеинтегратионс</span><span class="sxs-lookup"><span data-stu-id="d047b-103">List workforceIntegrations</span></span>

<span data-ttu-id="d047b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d047b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d047b-105">Получение списка объектов [воркфорцеинтегратион](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="d047b-105">Retrieve a list of [workforceIntegration](../resources/workforceintegration.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d047b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d047b-106">Permissions</span></span>

<span data-ttu-id="d047b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d047b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d047b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d047b-109">Permission type</span></span>                        | <span data-ttu-id="d047b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d047b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d047b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d047b-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="d047b-112">Воркфорцеинтегратион. Read. ALL, Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d047b-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="d047b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d047b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d047b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d047b-114">Not supported.</span></span> |
| <span data-ttu-id="d047b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d047b-115">Application</span></span>                            | <span data-ttu-id="d047b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d047b-116">Not supported.</span></span> |

> <span data-ttu-id="d047b-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="d047b-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d047b-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="d047b-118">Global admins can access groups that they are not a member of.</span></span>


## <a name="http-request"></a><span data-ttu-id="d047b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d047b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d047b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d047b-120">Optional query parameters</span></span>

<span data-ttu-id="d047b-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d047b-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d047b-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d047b-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d047b-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d047b-123">Request headers</span></span>

| <span data-ttu-id="d047b-124">Имя</span><span class="sxs-lookup"><span data-stu-id="d047b-124">Name</span></span>      |<span data-ttu-id="d047b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="d047b-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d047b-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d047b-126">Authorization</span></span> | <span data-ttu-id="d047b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d047b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d047b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d047b-129">Request body</span></span>

<span data-ttu-id="d047b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d047b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d047b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d047b-131">Response</span></span>

<span data-ttu-id="d047b-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркфорцеинтегратион](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d047b-132">If successful, this method returns a `200 OK` response code and a collection of [workforceIntegration](../resources/workforceintegration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d047b-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="d047b-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d047b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d047b-134">Request</span></span>

<span data-ttu-id="d047b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d047b-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d047b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d047b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workforceintegrations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations
```
# <a name="c"></a>[<span data-ttu-id="d047b-137">C#</span><span class="sxs-lookup"><span data-stu-id="d047b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workforceintegrations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d047b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d047b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workforceintegrations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d047b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d047b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workforceintegrations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d047b-140">Java</span><span class="sxs-lookup"><span data-stu-id="d047b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workforceintegrations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="d047b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d047b-141">Response</span></span>

<span data-ttu-id="d047b-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d047b-142">The following is an example of the response.</span></span>

> <span data-ttu-id="d047b-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d047b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName": "displayName-value",
      "apiVersion": 99,
      "encryption": {
        "protocol": "protocol-value",
        "secret": "secret-value"
      },
      "isActive": true,
      "url": "url-value",
      "supportedEntities": "supportedEntities-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List workforceIntegrations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
