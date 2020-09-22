---
title: Получение параметров для пользователя Analytics
description: Получение свойств объекта Settings для пользователя Analytics.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: eb88e2ca480a448bee5fe0c6ebc9f2cba0ee9d0b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022080"
---
# <a name="get-settings-for-user-analytics"></a><span data-ttu-id="40011-103">Получение параметров для пользователя Analytics</span><span class="sxs-lookup"><span data-stu-id="40011-103">Get settings for user analytics</span></span>

<span data-ttu-id="40011-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40011-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40011-105">Получение свойств объекта [Settings](../resources/settings.md) , который подходит для API аналитики.</span><span class="sxs-lookup"><span data-stu-id="40011-105">Retrieve the properties of a [settings](../resources/settings.md) object as applicable for the analytics API.</span></span>

## <a name="permissions"></a><span data-ttu-id="40011-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40011-106">Permissions</span></span>

<span data-ttu-id="40011-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40011-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="40011-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40011-109">Permission type</span></span>                        | <span data-ttu-id="40011-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40011-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="40011-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40011-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="40011-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="40011-112">User.Read</span></span> |
| <span data-ttu-id="40011-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40011-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40011-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40011-114">Not supported.</span></span> |
| <span data-ttu-id="40011-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40011-115">Application</span></span>                            | <span data-ttu-id="40011-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40011-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40011-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40011-117">HTTP request</span></span>

<!-- { "blockType": "ignored" }-->

```http
GET /me/analytics/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40011-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="40011-118">Optional query parameters</span></span>

<span data-ttu-id="40011-119">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="40011-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40011-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40011-120">Request headers</span></span>

| <span data-ttu-id="40011-121">Имя</span><span class="sxs-lookup"><span data-stu-id="40011-121">Name</span></span>      |<span data-ttu-id="40011-122">Описание</span><span class="sxs-lookup"><span data-stu-id="40011-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="40011-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="40011-123">Authorization</span></span> | <span data-ttu-id="40011-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="40011-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="40011-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40011-125">Request body</span></span>

<span data-ttu-id="40011-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40011-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40011-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="40011-127">Response</span></span>

<span data-ttu-id="40011-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [Settings](../resources/settings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40011-128">If successful, this method returns a `200 OK` response code and the requested [settings](../resources/settings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="40011-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="40011-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="40011-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="40011-130">Request</span></span>

<span data-ttu-id="40011-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40011-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="40011-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="40011-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/analytics/settings
```
# <a name="c"></a>[<span data-ttu-id="40011-133">C#</span><span class="sxs-lookup"><span data-stu-id="40011-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40011-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40011-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40011-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40011-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="40011-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="40011-136">Response</span></span>

<span data-ttu-id="40011-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="40011-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.settings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('12ab2b12-4b1a-43a1-adac-1a123456cd78')/analytics/settings",
    "hasLicense": true,
    "hasOptedOut": false,
    "hasGraphMailbox": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


