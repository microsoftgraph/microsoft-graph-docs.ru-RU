---
title: Получить параметры для аналитики пользователей
description: Извлечение свойств объекта параметров для пользовательской аналитики.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 607ddeea17942211cbd9988f5f3248385a0c7283
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955324"
---
# <a name="get-settings-for-user-analytics"></a><span data-ttu-id="10ccc-103">Получить параметры для аналитики пользователей</span><span class="sxs-lookup"><span data-stu-id="10ccc-103">Get settings for user analytics</span></span>

<span data-ttu-id="10ccc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10ccc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10ccc-105">Извлечение свойств объекта [параметров](../resources/settings.md) в соответствии с API аналитики.</span><span class="sxs-lookup"><span data-stu-id="10ccc-105">Retrieve the properties of a [settings](../resources/settings.md) object as applicable for the analytics API.</span></span>

## <a name="permissions"></a><span data-ttu-id="10ccc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10ccc-106">Permissions</span></span>

<span data-ttu-id="10ccc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10ccc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10ccc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10ccc-109">Permission type</span></span>                        | <span data-ttu-id="10ccc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10ccc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="10ccc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10ccc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="10ccc-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="10ccc-112">User.Read</span></span> |
| <span data-ttu-id="10ccc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10ccc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10ccc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10ccc-114">Not supported.</span></span> |
| <span data-ttu-id="10ccc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10ccc-115">Application</span></span>                            | <span data-ttu-id="10ccc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10ccc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="10ccc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10ccc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" }-->

```http
GET /me/analytics/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10ccc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="10ccc-118">Optional query parameters</span></span>

<span data-ttu-id="10ccc-119">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="10ccc-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10ccc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10ccc-120">Request headers</span></span>

| <span data-ttu-id="10ccc-121">Имя</span><span class="sxs-lookup"><span data-stu-id="10ccc-121">Name</span></span>      |<span data-ttu-id="10ccc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="10ccc-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="10ccc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="10ccc-123">Authorization</span></span> | <span data-ttu-id="10ccc-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="10ccc-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="10ccc-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10ccc-125">Request body</span></span>

<span data-ttu-id="10ccc-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10ccc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10ccc-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="10ccc-127">Response</span></span>

<span data-ttu-id="10ccc-128">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта параметров `200 OK` в тексте [](../resources/settings.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="10ccc-128">If successful, this method returns a `200 OK` response code and the requested [settings](../resources/settings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="10ccc-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="10ccc-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="10ccc-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="10ccc-130">Request</span></span>

<span data-ttu-id="10ccc-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10ccc-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="10ccc-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="10ccc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/analytics/settings
```
# <a name="c"></a>[<span data-ttu-id="10ccc-133">C#</span><span class="sxs-lookup"><span data-stu-id="10ccc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10ccc-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10ccc-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10ccc-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10ccc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10ccc-136">Java</span><span class="sxs-lookup"><span data-stu-id="10ccc-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-settings-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="10ccc-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="10ccc-137">Response</span></span>

<span data-ttu-id="10ccc-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="10ccc-138">The following is an example of the response.</span></span>

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


