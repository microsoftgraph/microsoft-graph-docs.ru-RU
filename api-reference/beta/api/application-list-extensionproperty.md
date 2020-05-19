---
title: Список Екстенсионпропертиес
description: Получение списка объектов екстенсионпроперти.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4e7a1eed267d98381250fbf3d3bf581e195700b9
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289336"
---
# <a name="list-extensionproperties"></a><span data-ttu-id="e1da6-103">Список Екстенсионпропертиес</span><span class="sxs-lookup"><span data-stu-id="e1da6-103">List extensionProperties</span></span>

<span data-ttu-id="e1da6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1da6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1da6-105">Получение списка объектов [екстенсионпроперти](../resources/extensionproperty.md) в приложении.</span><span class="sxs-lookup"><span data-stu-id="e1da6-105">Retrieve the list of [extensionProperty](../resources/extensionproperty.md) objects on an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1da6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1da6-106">Permissions</span></span>

<span data-ttu-id="e1da6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1da6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1da6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1da6-109">Permission type</span></span>      | <span data-ttu-id="e1da6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1da6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1da6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1da6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e1da6-112">Application. Read. ALL, Directory. Read. ALL, Application. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="e1da6-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e1da6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1da6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1da6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1da6-114">Not supported.</span></span>    |
|<span data-ttu-id="e1da6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1da6-115">Application</span></span> | <span data-ttu-id="e1da6-116">Application. Read. ALL, Application. ReadWrite. Овнедби, Application. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e1da6-116">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1da6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1da6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/extensionProperties
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1da6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e1da6-118">Optional query parameters</span></span>

<span data-ttu-id="e1da6-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e1da6-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e1da6-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e1da6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1da6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1da6-121">Request headers</span></span>

| <span data-ttu-id="e1da6-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e1da6-122">Name</span></span>       | <span data-ttu-id="e1da6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e1da6-123">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="e1da6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1da6-124">Authorization</span></span>  | <span data-ttu-id="e1da6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1da6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e1da6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e1da6-127">Request body</span></span>

<span data-ttu-id="e1da6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e1da6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1da6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1da6-129">Response</span></span>

<span data-ttu-id="e1da6-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [екстенсионпроперти](../resources/extensionproperty.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e1da6-130">If successful, this method returns a `200 OK` response code and a collection of [extensionProperty](../resources/extensionproperty.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e1da6-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="e1da6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e1da6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1da6-132">Request</span></span>

<span data-ttu-id="e1da6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1da6-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e1da6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1da6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_extensionproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/extensionProperties
```
# <a name="c"></a>[<span data-ttu-id="e1da6-135">C#</span><span class="sxs-lookup"><span data-stu-id="e1da6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-extensionproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1da6-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1da6-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-extensionproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1da6-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1da6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-extensionproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e1da6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1da6-138">Response</span></span>

<span data-ttu-id="e1da6-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e1da6-139">The following is an example of the response.</span></span>

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
