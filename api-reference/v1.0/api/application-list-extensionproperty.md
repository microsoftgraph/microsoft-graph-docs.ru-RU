---
title: Список Екстенсионпропертиес
description: Получение списка объектов екстенсионпроперти.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 35548424bfdb402e7a51b34ade43c852ac9efaf2
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939721"
---
# <a name="list-extensionproperties"></a><span data-ttu-id="ea90f-103">Список Екстенсионпропертиес</span><span class="sxs-lookup"><span data-stu-id="ea90f-103">List extensionProperties</span></span>

<span data-ttu-id="ea90f-104">Получение списка объектов [екстенсионпроперти](../resources/extensionproperty.md) в приложении.</span><span class="sxs-lookup"><span data-stu-id="ea90f-104">Retrieve the list of [extensionProperty](../resources/extensionproperty.md) objects on an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea90f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea90f-105">Permissions</span></span>

<span data-ttu-id="ea90f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea90f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea90f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea90f-108">Permission type</span></span>      | <span data-ttu-id="ea90f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea90f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea90f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea90f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ea90f-111">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ea90f-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ea90f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea90f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea90f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea90f-113">Not supported.</span></span>    |
|<span data-ttu-id="ea90f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea90f-114">Application</span></span> | <span data-ttu-id="ea90f-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea90f-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea90f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea90f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/extensionProperties
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ea90f-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ea90f-117">Optional query parameters</span></span>

<span data-ttu-id="ea90f-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ea90f-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ea90f-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ea90f-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea90f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea90f-120">Request headers</span></span>

| <span data-ttu-id="ea90f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ea90f-121">Name</span></span>       | <span data-ttu-id="ea90f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ea90f-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="ea90f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea90f-123">Authorization</span></span>  | <span data-ttu-id="ea90f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea90f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ea90f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ea90f-126">Request body</span></span>

<span data-ttu-id="ea90f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea90f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea90f-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea90f-128">Response</span></span>

<span data-ttu-id="ea90f-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [екстенсионпроперти](../resources/extensionproperty.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea90f-129">If successful, this method returns a `200 OK` response code and a collection of [extensionProperty](../resources/extensionproperty.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ea90f-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="ea90f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ea90f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea90f-131">Request</span></span>

<span data-ttu-id="ea90f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea90f-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_extensionproperties"
}-->

```http
GET https://graph.microsoft.com/v1.0/applications/{id}/extensionProperties
```

### <a name="response"></a><span data-ttu-id="ea90f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea90f-133">Response</span></span>

<span data-ttu-id="ea90f-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ea90f-134">The following is an example of the response.</span></span>

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
