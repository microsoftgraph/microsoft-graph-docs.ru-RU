---
title: Получение параметров для пользователя Analytics
description: Получение свойств объекта Settings для пользователя Analytics.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: d44203c1d0a2a910182822cfc35565a30e1cd4ae
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724108"
---
# <a name="get-settings-for-user-analytics"></a><span data-ttu-id="5f57e-103">Получение параметров для пользователя Analytics</span><span class="sxs-lookup"><span data-stu-id="5f57e-103">Get settings for user analytics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f57e-104">Получение свойств объекта [Settings](../resources/settings.md) , который подходит для API аналитики.</span><span class="sxs-lookup"><span data-stu-id="5f57e-104">Retrieve the properties of a [settings](../resources/settings.md) object as applicable for the analytics API.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f57e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f57e-105">Permissions</span></span>

<span data-ttu-id="5f57e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f57e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5f57e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f57e-108">Permission type</span></span>                        | <span data-ttu-id="5f57e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f57e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5f57e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f57e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f57e-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="5f57e-111">User.Read</span></span> |
| <span data-ttu-id="5f57e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f57e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f57e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f57e-113">Not supported.</span></span> |
| <span data-ttu-id="5f57e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f57e-114">Application</span></span>                            | <span data-ttu-id="5f57e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f57e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f57e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f57e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" }-->

```http
GET https://graph.microsoft.com/beta/me/analytics/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f57e-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5f57e-117">Optional query parameters</span></span>

<span data-ttu-id="5f57e-118">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5f57e-118">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f57e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f57e-119">Request headers</span></span>

| <span data-ttu-id="5f57e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5f57e-120">Name</span></span>      |<span data-ttu-id="5f57e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5f57e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5f57e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f57e-122">Authorization</span></span> | <span data-ttu-id="5f57e-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="5f57e-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f57e-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5f57e-124">Request body</span></span>

<span data-ttu-id="5f57e-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5f57e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f57e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f57e-126">Response</span></span>

<span data-ttu-id="5f57e-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [Settings](../resources/settings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5f57e-127">If successful, this method returns a `200 OK` response code and the requested [settings](../resources/settings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5f57e-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="5f57e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5f57e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f57e-129">Request</span></span>

<span data-ttu-id="5f57e-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f57e-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5f57e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f57e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/analytics/settings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5f57e-132">C#</span><span class="sxs-lookup"><span data-stu-id="5f57e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5f57e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f57e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5f57e-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="5f57e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5f57e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f57e-135">Response</span></span>

<span data-ttu-id="5f57e-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5f57e-136">The following is an example of the response.</span></span>

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
