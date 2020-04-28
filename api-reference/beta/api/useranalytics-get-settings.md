---
title: Получение параметров для пользователя Analytics
description: Получение свойств объекта Settings для пользователя Analytics.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: be09792d08799d952334c33d52e0985196df7800
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451590"
---
# <a name="get-settings-for-user-analytics"></a><span data-ttu-id="6d38d-103">Получение параметров для пользователя Analytics</span><span class="sxs-lookup"><span data-stu-id="6d38d-103">Get settings for user analytics</span></span>

<span data-ttu-id="6d38d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d38d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d38d-105">Получение свойств объекта [Settings](../resources/settings.md) , который подходит для API аналитики.</span><span class="sxs-lookup"><span data-stu-id="6d38d-105">Retrieve the properties of a [settings](../resources/settings.md) object as applicable for the analytics API.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d38d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d38d-106">Permissions</span></span>

<span data-ttu-id="6d38d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d38d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6d38d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d38d-109">Permission type</span></span>                        | <span data-ttu-id="6d38d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d38d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6d38d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d38d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d38d-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="6d38d-112">User.Read</span></span> |
| <span data-ttu-id="6d38d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d38d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d38d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d38d-114">Not supported.</span></span> |
| <span data-ttu-id="6d38d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d38d-115">Application</span></span>                            | <span data-ttu-id="6d38d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d38d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d38d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d38d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" }-->

```http
GET /me/analytics/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d38d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6d38d-118">Optional query parameters</span></span>

<span data-ttu-id="6d38d-119">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="6d38d-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d38d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d38d-120">Request headers</span></span>

| <span data-ttu-id="6d38d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6d38d-121">Name</span></span>      |<span data-ttu-id="6d38d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6d38d-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6d38d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d38d-123">Authorization</span></span> | <span data-ttu-id="6d38d-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6d38d-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d38d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6d38d-125">Request body</span></span>

<span data-ttu-id="6d38d-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6d38d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d38d-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d38d-127">Response</span></span>

<span data-ttu-id="6d38d-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [Settings](../resources/settings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6d38d-128">If successful, this method returns a `200 OK` response code and the requested [settings](../resources/settings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6d38d-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="6d38d-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6d38d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d38d-130">Request</span></span>

<span data-ttu-id="6d38d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d38d-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6d38d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d38d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/analytics/settings
```
# <a name="c"></a>[<span data-ttu-id="6d38d-133">C#</span><span class="sxs-lookup"><span data-stu-id="6d38d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d38d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d38d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d38d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d38d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6d38d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d38d-136">Response</span></span>

<span data-ttu-id="6d38d-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6d38d-137">The following is an example of the response.</span></span>

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
