---
author: swapnil1993
title: 'сайт: getApplicableContentTypesForList'
description: Получите типы контента сайта, которые можно добавить в список.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 2cda6c5e62fc85db8d512d814064fd977fa36b9e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447658"
---
# <a name="site-getapplicablecontenttypesforlist"></a><span data-ttu-id="3afa9-103">сайт: getApplicableContentTypesForList</span><span class="sxs-lookup"><span data-stu-id="3afa9-103">site: getApplicableContentTypesForList</span></span>
<span data-ttu-id="3afa9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3afa9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3afa9-105">Получите [контент][] [сайтаTypes,][contentType] который можно добавить в список.</span><span class="sxs-lookup"><span data-stu-id="3afa9-105">Get [site][] [contentTypes][contentType] that can be added to a list.</span></span>

## <a name="permissions"></a><span data-ttu-id="3afa9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3afa9-106">Permissions</span></span>

<span data-ttu-id="3afa9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3afa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3afa9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3afa9-109">Permission type</span></span>      | <span data-ttu-id="3afa9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3afa9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3afa9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3afa9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3afa9-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="3afa9-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="3afa9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3afa9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3afa9-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3afa9-114">Not Supported</span></span>    |
|<span data-ttu-id="3afa9-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3afa9-115">Application</span></span> | <span data-ttu-id="3afa9-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="3afa9-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3afa9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3afa9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{siteId}/getApplicableContentTypesForList
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3afa9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3afa9-118">Optional query parameters</span></span>

<span data-ttu-id="3afa9-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3afa9-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3afa9-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3afa9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="3afa9-121">Чтобы перечислить только настраиваемые типы контента, используйте `$filter=isBuiltin eq false` .</span><span class="sxs-lookup"><span data-stu-id="3afa9-121">To list only custom content types, use `$filter=isBuiltin eq false`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3afa9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3afa9-122">Request headers</span></span>
|<span data-ttu-id="3afa9-123">Имя</span><span class="sxs-lookup"><span data-stu-id="3afa9-123">Name</span></span>|<span data-ttu-id="3afa9-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3afa9-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3afa9-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3afa9-125">Authorization</span></span>|<span data-ttu-id="3afa9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3afa9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3afa9-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3afa9-128">Request body</span></span>
<span data-ttu-id="3afa9-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3afa9-129">Do not supply a request body for this method.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="3afa9-130">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="3afa9-130">Function Parameters</span></span>
<span data-ttu-id="3afa9-131">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="3afa9-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="3afa9-132">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="3afa9-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="3afa9-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="3afa9-133">Parameter</span></span>|<span data-ttu-id="3afa9-134">Тип</span><span class="sxs-lookup"><span data-stu-id="3afa9-134">Type</span></span>|<span data-ttu-id="3afa9-135">Описание</span><span class="sxs-lookup"><span data-stu-id="3afa9-135">Description</span></span>|
|-|-|-|-|
|<span data-ttu-id="3afa9-136">listId</span><span class="sxs-lookup"><span data-stu-id="3afa9-136">listId</span></span>| <span data-ttu-id="3afa9-137">String</span><span class="sxs-lookup"><span data-stu-id="3afa9-137">String</span></span> | <span data-ttu-id="3afa9-138">GUID списка, для которого необходимо извлечь соответствующие типы контента.</span><span class="sxs-lookup"><span data-stu-id="3afa9-138">GUID of the list for which the applicable content types need to be fetched.</span></span> <span data-ttu-id="3afa9-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3afa9-139">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3afa9-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3afa9-140">Response</span></span>

<span data-ttu-id="3afa9-141">В случае успешной работы эта функция возвращает код ответа и `200 OK` [коллекцию contentType](../resources/contenttype.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3afa9-141">If successful, this function returns a `200 OK` response code and a [contentType](../resources/contenttype.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3afa9-142">Пример</span><span class="sxs-lookup"><span data-stu-id="3afa9-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="3afa9-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="3afa9-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "site_getapplicablecontenttypesforlist"
}
-->
```http
GET https://graph.microsoft.com/beta/sites/{siteId}/getApplicableContentTypesForList(listId='listId')
```

### <a name="response"></a><span data-ttu-id="3afa9-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="3afa9-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.contentType)"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
        "id":"0x",
        "description":"",
        "group":"_Hidden",
        "hidden":false,
        "name":"System",
        "base": {
            "name": "System",
            "id": "0x"
        }
    },
    {
        "id":"0x00A7470EADF4194E2E9ED1031B61DA0884",
        "name": "docSet",
        "description": "custom docset",
        "hidden":false,
        "base": {
            "name": "Document Set",
            "id": "0x0120D520"
        },
        "group": "Custom Content Types"
    }
  ]
}
```

[contentType]: ../resources/contentType.md
[site]: ../resources/site.md
