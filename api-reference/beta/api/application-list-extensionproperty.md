---
title: Список Екстенсионпропертиес
description: Получение списка объектов екстенсионпроперти.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ff2f9d1c47d00d03ebafb7b777269b30f017f496
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006426"
---
# <a name="list-extensionproperties"></a><span data-ttu-id="cce88-103">Список Екстенсионпропертиес</span><span class="sxs-lookup"><span data-stu-id="cce88-103">List extensionProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cce88-104">Получение списка объектов [екстенсионпроперти](../resources/extensionproperty.md) в приложении.</span><span class="sxs-lookup"><span data-stu-id="cce88-104">Retrieve the list of [extensionProperty](../resources/extensionproperty.md) objects on an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="cce88-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cce88-105">Permissions</span></span>

<span data-ttu-id="cce88-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cce88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cce88-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cce88-108">Permission type</span></span>      | <span data-ttu-id="cce88-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cce88-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cce88-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cce88-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cce88-111">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cce88-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cce88-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cce88-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cce88-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cce88-113">Not supported.</span></span>    |
|<span data-ttu-id="cce88-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cce88-114">Application</span></span> | <span data-ttu-id="cce88-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="cce88-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cce88-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cce88-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/extensionProperties
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cce88-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cce88-117">Optional query parameters</span></span>

<span data-ttu-id="cce88-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cce88-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="cce88-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cce88-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cce88-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cce88-120">Request headers</span></span>

| <span data-ttu-id="cce88-121">Имя</span><span class="sxs-lookup"><span data-stu-id="cce88-121">Name</span></span>       | <span data-ttu-id="cce88-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cce88-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="cce88-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cce88-123">Authorization</span></span>  | <span data-ttu-id="cce88-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cce88-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cce88-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cce88-126">Request body</span></span>

<span data-ttu-id="cce88-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cce88-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cce88-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="cce88-128">Response</span></span>

<span data-ttu-id="cce88-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [екстенсионпроперти](../resources/extensionproperty.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cce88-129">If successful, this method returns a `200 OK` response code and a collection of [extensionProperty](../resources/extensionproperty.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cce88-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="cce88-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cce88-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cce88-131">Request</span></span>

<span data-ttu-id="cce88-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cce88-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cce88-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cce88-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_extensionproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/extensionProperties
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cce88-134">C#</span><span class="sxs-lookup"><span data-stu-id="cce88-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-extensionproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cce88-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cce88-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-extensionproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cce88-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cce88-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-extensionproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cce88-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="cce88-137">Response</span></span>

<span data-ttu-id="cce88-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cce88-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.extensionProperty",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "a2c459db-f5dc-4328-ae9b-118e88d04d19",
            "deletedDateTime": null,
            "appDisplayName": "Display name",
            "name": "extension_b3efaf8f68a44275abcff28ef86b2ee3_extensionName",
            "dataType": "String",
            "isSyncedFromOnPremises": false,
            "targetObjects": [
                "Application"
            ]
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List extensionProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->