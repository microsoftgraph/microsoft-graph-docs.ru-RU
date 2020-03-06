---
title: Список Екстенсионпропертиес
description: Получение списка объектов екстенсионпроперти.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e0c2af0d25b65f2f89e38e66971349248357744d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518912"
---
# <a name="list-extensionproperties"></a><span data-ttu-id="96f69-103">Список Екстенсионпропертиес</span><span class="sxs-lookup"><span data-stu-id="96f69-103">List extensionProperties</span></span>

<span data-ttu-id="96f69-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96f69-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="96f69-105">Получение списка объектов [екстенсионпроперти](../resources/extensionproperty.md) в приложении.</span><span class="sxs-lookup"><span data-stu-id="96f69-105">Retrieve the list of [extensionProperty](../resources/extensionproperty.md) objects on an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="96f69-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96f69-106">Permissions</span></span>

<span data-ttu-id="96f69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96f69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96f69-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96f69-109">Permission type</span></span>      | <span data-ttu-id="96f69-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96f69-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96f69-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96f69-111">Delegated (work or school account)</span></span> | <span data-ttu-id="96f69-112">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="96f69-112">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="96f69-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96f69-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96f69-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96f69-114">Not supported.</span></span>    |
|<span data-ttu-id="96f69-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96f69-115">Application</span></span> | <span data-ttu-id="96f69-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="96f69-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="96f69-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96f69-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/extensionProperties
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96f69-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="96f69-118">Optional query parameters</span></span>

<span data-ttu-id="96f69-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="96f69-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="96f69-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="96f69-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="96f69-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96f69-121">Request headers</span></span>

| <span data-ttu-id="96f69-122">Имя</span><span class="sxs-lookup"><span data-stu-id="96f69-122">Name</span></span>       | <span data-ttu-id="96f69-123">Описание</span><span class="sxs-lookup"><span data-stu-id="96f69-123">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="96f69-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96f69-124">Authorization</span></span>  | <span data-ttu-id="96f69-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96f69-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="96f69-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96f69-127">Request body</span></span>

<span data-ttu-id="96f69-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="96f69-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96f69-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="96f69-129">Response</span></span>

<span data-ttu-id="96f69-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [екстенсионпроперти](../resources/extensionproperty.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="96f69-130">If successful, this method returns a `200 OK` response code and a collection of [extensionProperty](../resources/extensionproperty.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="96f69-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="96f69-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="96f69-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="96f69-132">Request</span></span>

<span data-ttu-id="96f69-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96f69-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="96f69-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="96f69-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_extensionproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/{id}/extensionProperties
```
# <a name="c"></a>[<span data-ttu-id="96f69-135">C#</span><span class="sxs-lookup"><span data-stu-id="96f69-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-extensionproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96f69-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96f69-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-extensionproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96f69-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96f69-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-extensionproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96f69-138">Java</span><span class="sxs-lookup"><span data-stu-id="96f69-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-extensionproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="96f69-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="96f69-139">Response</span></span>

<span data-ttu-id="96f69-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="96f69-140">The following is an example of the response.</span></span>

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
