---
title: Список Ситесаурцес
description: Получение списка объектов Ситесаурце и их свойств.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 558ae59ccbf008889524d3c3825fb3e8ea8249f0
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597759"
---
# <a name="list-sitesources"></a><span data-ttu-id="ba927-103">Список Ситесаурцес</span><span class="sxs-lookup"><span data-stu-id="ba927-103">List siteSources</span></span>

<span data-ttu-id="ba927-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba927-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba927-105">Получение списка объектов [ситесаурце](../resources/sitesource.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="ba927-105">Get a list of [siteSource](../resources/sitesource.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba927-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba927-106">Permissions</span></span>

<span data-ttu-id="ba927-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba927-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba927-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba927-109">Permission type</span></span>|<span data-ttu-id="ba927-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba927-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba927-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba927-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ba927-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="ba927-112">User.Read</span></span>|
|<span data-ttu-id="ba927-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba927-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba927-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba927-114">Not supported.</span></span>|
|<span data-ttu-id="ba927-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba927-115">Application</span></span>|<span data-ttu-id="ba927-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba927-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba927-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba927-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/siteSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba927-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ba927-118">Optional query parameters</span></span>

<span data-ttu-id="ba927-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ba927-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ba927-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ba927-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba927-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba927-121">Request headers</span></span>

|<span data-ttu-id="ba927-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ba927-122">Name</span></span>|<span data-ttu-id="ba927-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ba927-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ba927-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba927-124">Authorization</span></span>|<span data-ttu-id="ba927-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba927-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba927-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba927-127">Request body</span></span>

<span data-ttu-id="ba927-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba927-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba927-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba927-129">Response</span></span>

<span data-ttu-id="ba927-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [ситесаурце](../resources/sitesource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba927-130">If successful, this method returns a `200 OK` response code and a collection of [siteSource](../resources/sitesource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba927-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="ba927-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba927-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba927-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_sitesource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/siteSources
```

### <a name="response"></a><span data-ttu-id="ba927-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba927-133">Response</span></span>

<span data-ttu-id="ba927-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ba927-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.siteSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/siteSources",
    "value": [
        {
            "displayName": "Microsoft Team Site",
            "createdDateTime": "2020-10-27T15:14:11.0048392Z",
            "id": "38304445-3741-3333-4233-344238454333",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": null
                }
            }
        }
    ]
}
```
