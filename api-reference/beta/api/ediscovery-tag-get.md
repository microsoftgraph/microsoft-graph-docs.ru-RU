---
title: Получить тег
description: Ознакомьтесь с свойствами и отношениями объекта тегов.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 0ac2c2c1fe3e9a4d8d61980ce09850f24cac782a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446831"
---
# <a name="get-tag"></a><span data-ttu-id="59fa8-103">Получить тег</span><span class="sxs-lookup"><span data-stu-id="59fa8-103">Get tag</span></span>

<span data-ttu-id="59fa8-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="59fa8-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59fa8-105">Ознакомьтесь с свойствами и отношениями объекта [тегов.](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="59fa8-105">Read the properties and relationships of a [tag](../resources/ediscovery-tag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="59fa8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59fa8-106">Permissions</span></span>

<span data-ttu-id="59fa8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59fa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59fa8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59fa8-109">Permission type</span></span>|<span data-ttu-id="59fa8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59fa8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59fa8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59fa8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="59fa8-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59fa8-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="59fa8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59fa8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59fa8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59fa8-114">Not supported.</span></span>|
|<span data-ttu-id="59fa8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59fa8-115">Application</span></span>|<span data-ttu-id="59fa8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59fa8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59fa8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59fa8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/tags/{tagId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="59fa8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="59fa8-118">Optional query parameters</span></span>

<span data-ttu-id="59fa8-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="59fa8-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="59fa8-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="59fa8-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="59fa8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59fa8-121">Request headers</span></span>

|<span data-ttu-id="59fa8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="59fa8-122">Name</span></span>|<span data-ttu-id="59fa8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="59fa8-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="59fa8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59fa8-124">Authorization</span></span>|<span data-ttu-id="59fa8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59fa8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59fa8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="59fa8-127">Request body</span></span>

<span data-ttu-id="59fa8-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="59fa8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59fa8-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="59fa8-129">Response</span></span>

<span data-ttu-id="59fa8-130">В случае успешного решения этот метод возвращает код ответа и `200 OK` [объект microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="59fa8-130">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="59fa8-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="59fa8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="59fa8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="59fa8-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_tag"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/e54b3f535b434a9a8743b84e34c00504
```

### <a name="response"></a><span data-ttu-id="59fa8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="59fa8-133">Response</span></span>

<span data-ttu-id="59fa8-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="59fa8-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.tag"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('47746044-fd0b-4a30-acfc-5272b691ba5b')/tags/$entity",
    "displayName": "Responsiveness",
    "description": "Indicates the responsiveness of the document",
    "lastModifiedDateTime": "2021-01-11T19:32:23.1903658Z",
    "childSelectability": "One",
    "id": "e54b3f535b434a9a8743b84e34c00504",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalName": "admin@contoso.com"
        }
    },
    "childTags": []
}
```
