---
author: swapnil1993
title: Список contentTypes в списке
description: Список типов контента в списке
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: ff6ecd580a654c9b9bff6005317b586f9bf105d9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965170"
---
# <a name="list-contenttypes-in-a-list"></a><span data-ttu-id="f3e9b-103">Список contentTypes в списке</span><span class="sxs-lookup"><span data-stu-id="f3e9b-103">List contentTypes in a list</span></span>
<span data-ttu-id="f3e9b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3e9b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="f3e9b-105">Получите коллекцию [ресурсов contentType][contentType] в [списке.][]</span><span class="sxs-lookup"><span data-stu-id="f3e9b-105">Get the collection of [contentType][contentType] resources in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="f3e9b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3e9b-106">Permissions</span></span>

<span data-ttu-id="f3e9b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f3e9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="f3e9b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3e9b-109">Permission type</span></span>      | <span data-ttu-id="f3e9b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3e9b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3e9b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3e9b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f3e9b-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="f3e9b-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="f3e9b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3e9b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3e9b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3e9b-114">Not supported.</span></span>    |
|<span data-ttu-id="f3e9b-115">Application</span><span class="sxs-lookup"><span data-stu-id="f3e9b-115">Application</span></span> | <span data-ttu-id="f3e9b-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="f3e9b-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3e9b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3e9b-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /sites/{site-id}/lists/{list-id}/contentTypes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f3e9b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f3e9b-118">Optional query parameters</span></span>

<span data-ttu-id="f3e9b-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f3e9b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f3e9b-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f3e9b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3e9b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3e9b-121">Request headers</span></span>
|<span data-ttu-id="f3e9b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f3e9b-122">Name</span></span>|<span data-ttu-id="f3e9b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f3e9b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f3e9b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3e9b-124">Authorization</span></span>|<span data-ttu-id="f3e9b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3e9b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3e9b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3e9b-127">Request body</span></span>
<span data-ttu-id="f3e9b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f3e9b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3e9b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3e9b-129">Response</span></span>

<span data-ttu-id="f3e9b-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [contentType](../resources/contenttype.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f3e9b-130">If successful, this method returns a `200 OK` response code and a collection of [contentType](../resources/contenttype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3e9b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f3e9b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3e9b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3e9b-132">Request</span></span>

<!-- { "blockType": "request", "name": "enum_contentTypes"} -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/contentTypes
```

### <a name="response"></a><span data-ttu-id="f3e9b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3e9b-133">Response</span></span>

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
[list]: ../resources/list.md
