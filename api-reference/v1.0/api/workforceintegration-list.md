---
title: Список рабочей силыИнтеграции
description: Извлечение списка объектов workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d96aa5dcf131724fbd231ed7574606bd1b736d21
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52031490"
---
# <a name="list-workforceintegrations"></a><span data-ttu-id="453d4-103">Список рабочей силыИнтеграции</span><span class="sxs-lookup"><span data-stu-id="453d4-103">List workforceIntegrations</span></span>

<span data-ttu-id="453d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="453d4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="453d4-105">Извлечение списка [объектов workforceIntegration.](../resources/workforceintegration.md)</span><span class="sxs-lookup"><span data-stu-id="453d4-105">Retrieve a list of [workforceIntegration](../resources/workforceintegration.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="453d4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="453d4-106">Permissions</span></span>

<span data-ttu-id="453d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="453d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="453d4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="453d4-109">Permission type</span></span>                        | <span data-ttu-id="453d4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="453d4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="453d4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="453d4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="453d4-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="453d4-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="453d4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="453d4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="453d4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="453d4-114">Not supported.</span></span> |
| <span data-ttu-id="453d4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="453d4-115">Application</span></span>                            | <span data-ttu-id="453d4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="453d4-116">Not supported.</span></span> |

> <span data-ttu-id="453d4-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="453d4-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="453d4-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="453d4-118">Global admins can access groups that they are not a member of.</span></span>


## <a name="http-request"></a><span data-ttu-id="453d4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="453d4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="453d4-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="453d4-120">Optional query parameters</span></span>

<span data-ttu-id="453d4-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="453d4-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="453d4-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="453d4-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="453d4-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="453d4-123">Request headers</span></span>

| <span data-ttu-id="453d4-124">Имя</span><span class="sxs-lookup"><span data-stu-id="453d4-124">Name</span></span>      |<span data-ttu-id="453d4-125">Описание</span><span class="sxs-lookup"><span data-stu-id="453d4-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="453d4-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="453d4-126">Authorization</span></span> | <span data-ttu-id="453d4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="453d4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="453d4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="453d4-129">Request body</span></span>

<span data-ttu-id="453d4-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="453d4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="453d4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="453d4-131">Response</span></span>

<span data-ttu-id="453d4-132">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [workforceIntegration](../resources/workforceintegration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="453d4-132">If successful, this method returns a `200 OK` response code and a collection of [workforceIntegration](../resources/workforceintegration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="453d4-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="453d4-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="453d4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="453d4-134">Request</span></span>

<span data-ttu-id="453d4-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="453d4-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="453d4-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="453d4-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workforceintegrations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations
```
# <a name="c"></a>[<span data-ttu-id="453d4-137">C#</span><span class="sxs-lookup"><span data-stu-id="453d4-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workforceintegrations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="453d4-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="453d4-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workforceintegrations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="453d4-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="453d4-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workforceintegrations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="453d4-140">Java</span><span class="sxs-lookup"><span data-stu-id="453d4-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workforceintegrations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="453d4-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="453d4-141">Response</span></span>

<span data-ttu-id="453d4-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="453d4-142">The following is an example of the response.</span></span>

> <span data-ttu-id="453d4-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="453d4-143">**Note:** The response object shown here might be shortened for readability.</span></span>

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

