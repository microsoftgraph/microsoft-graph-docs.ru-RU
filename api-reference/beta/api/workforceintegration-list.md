---
title: Список рабочей силыИнтеграции
description: Извлечение списка объектов workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e28e40ec75833cde86d80cca26ea4d0a423ff018
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054702"
---
# <a name="list-workforceintegrations"></a><span data-ttu-id="f71c0-103">Список рабочей силыИнтеграции</span><span class="sxs-lookup"><span data-stu-id="f71c0-103">List workforceIntegrations</span></span>

<span data-ttu-id="f71c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f71c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f71c0-105">Извлечение списка [объектов workforceIntegration.](../resources/workforceintegration.md)</span><span class="sxs-lookup"><span data-stu-id="f71c0-105">Retrieve a list of [workforceIntegration](../resources/workforceintegration.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f71c0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f71c0-106">Permissions</span></span>

<span data-ttu-id="f71c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f71c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f71c0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f71c0-109">Permission type</span></span>                        | <span data-ttu-id="f71c0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f71c0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f71c0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f71c0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f71c0-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f71c0-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="f71c0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f71c0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f71c0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f71c0-114">Not supported.</span></span> |
| <span data-ttu-id="f71c0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f71c0-115">Application</span></span>                            | <span data-ttu-id="f71c0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f71c0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f71c0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f71c0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f71c0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f71c0-118">Optional query parameters</span></span>

<span data-ttu-id="f71c0-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f71c0-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f71c0-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f71c0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f71c0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f71c0-121">Request headers</span></span>

| <span data-ttu-id="f71c0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f71c0-122">Name</span></span>      |<span data-ttu-id="f71c0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f71c0-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f71c0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f71c0-124">Authorization</span></span> | <span data-ttu-id="f71c0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f71c0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f71c0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f71c0-127">Request body</span></span>

<span data-ttu-id="f71c0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f71c0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f71c0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f71c0-129">Response</span></span>

<span data-ttu-id="f71c0-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [workforceIntegration](../resources/workforceintegration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f71c0-130">If successful, this method returns a `200 OK` response code and a collection of [workforceIntegration](../resources/workforceintegration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f71c0-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="f71c0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f71c0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f71c0-132">Request</span></span>

<span data-ttu-id="f71c0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f71c0-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f71c0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f71c0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workforceintegrations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teamwork/workforceIntegrations
```
# <a name="c"></a>[<span data-ttu-id="f71c0-135">C#</span><span class="sxs-lookup"><span data-stu-id="f71c0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workforceintegrations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f71c0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f71c0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workforceintegrations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f71c0-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f71c0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workforceintegrations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f71c0-138">Java</span><span class="sxs-lookup"><span data-stu-id="f71c0-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workforceintegrations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f71c0-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f71c0-139">Response</span></span>

<span data-ttu-id="f71c0-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f71c0-140">The following is an example of the response.</span></span>

> <span data-ttu-id="f71c0-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f71c0-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "supports": "supports-value"
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


