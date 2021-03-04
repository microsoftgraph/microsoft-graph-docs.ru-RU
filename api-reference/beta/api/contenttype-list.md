---
author: swapnil1993
title: List contentTypes
description: Список типов контента на сайте или в списке
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: ef47931edf4cf59094b4d3eb7659536e3866921e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447239"
---
# <a name="list-contenttypes"></a><span data-ttu-id="79e7c-103">List contentTypes</span><span class="sxs-lookup"><span data-stu-id="79e7c-103">List contentTypes</span></span>
<span data-ttu-id="79e7c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79e7c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="79e7c-105">Получить коллекцию типов [контента][contentType] на [сайте][] или в [списке][]</span><span class="sxs-lookup"><span data-stu-id="79e7c-105">Get the collection of [content types][contentType] in a [site][] or a [list][]</span></span>

## <a name="permissions"></a><span data-ttu-id="79e7c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79e7c-106">Permissions</span></span>

<span data-ttu-id="79e7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="79e7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="79e7c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79e7c-109">Permission type</span></span>      | <span data-ttu-id="79e7c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79e7c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79e7c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79e7c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="79e7c-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="79e7c-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="79e7c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79e7c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79e7c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79e7c-114">Not supported.</span></span>    |
|<span data-ttu-id="79e7c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="79e7c-115">Application</span></span> | <span data-ttu-id="79e7c-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="79e7c-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79e7c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79e7c-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /sites/{site-id}/contentTypes
GET /sites/{site-id}/lists/{list-id}/contentTypes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79e7c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="79e7c-118">Optional query parameters</span></span>

<span data-ttu-id="79e7c-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="79e7c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="79e7c-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="79e7c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="79e7c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79e7c-121">Request headers</span></span>
|<span data-ttu-id="79e7c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="79e7c-122">Name</span></span>|<span data-ttu-id="79e7c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="79e7c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="79e7c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79e7c-124">Authorization</span></span>|<span data-ttu-id="79e7c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79e7c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79e7c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="79e7c-127">Request body</span></span>
<span data-ttu-id="79e7c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="79e7c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79e7c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="79e7c-129">Response</span></span>

<span data-ttu-id="79e7c-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [contentType](../resources/contenttype.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79e7c-130">If successful, this method returns a `200 OK` response code and a collection of [contentType](../resources/contenttype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79e7c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="79e7c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="79e7c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="79e7c-132">Request</span></span>

<!-- { "blockType": "request", "name": "enum_contentTypes"} -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/contentTypes
```

### <a name="response"></a><span data-ttu-id="79e7c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="79e7c-133">Response</span></span>

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
[list]: ../resources/list.md
