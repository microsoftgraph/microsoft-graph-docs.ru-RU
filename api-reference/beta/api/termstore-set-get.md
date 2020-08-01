---
title: Получение набора
description: Считывание свойств и связей объекта Set.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 02f61201db78e2c4e2d8a7dbef4bc0776071f1f0
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539407"
---
# <a name="get-set"></a><span data-ttu-id="1d3d5-103">Получение набора</span><span class="sxs-lookup"><span data-stu-id="1d3d5-103">Get set</span></span>
<span data-ttu-id="1d3d5-104">Пространство имен: Microsoft. Graph. банка[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="1d3d5-104">Namespace: microsoft.graph.termStore [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="1d3d5-105">Считывание свойств и связей объекта [Set](../resources/termstore-set.md) .</span><span class="sxs-lookup"><span data-stu-id="1d3d5-105">Read the properties and relationships of a [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d3d5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d3d5-106">Permissions</span></span>
<span data-ttu-id="1d3d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d3d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d3d5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d3d5-109">Permission type</span></span>|<span data-ttu-id="1d3d5-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d3d5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d3d5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d3d5-111">Delegated (work or school account)</span></span> |<span data-ttu-id="1d3d5-112">Банк. чтение. ALL, банк. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1d3d5-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="1d3d5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d3d5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d3d5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d3d5-114">Not supported.</span></span>    |
|<span data-ttu-id="1d3d5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d3d5-115">Application</span></span> | <span data-ttu-id="1d3d5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d3d5-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="1d3d5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d3d5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/sets/{setId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1d3d5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1d3d5-118">Optional query parameters</span></span>
<span data-ttu-id="1d3d5-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1d3d5-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1d3d5-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1d3d5-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d3d5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d3d5-121">Request headers</span></span>
|<span data-ttu-id="1d3d5-122">Имя</span><span class="sxs-lookup"><span data-stu-id="1d3d5-122">Name</span></span>|<span data-ttu-id="1d3d5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1d3d5-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1d3d5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d3d5-124">Authorization</span></span>|<span data-ttu-id="1d3d5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d3d5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d3d5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d3d5-127">Request body</span></span>
<span data-ttu-id="1d3d5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1d3d5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d3d5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d3d5-129">Response</span></span>

<span data-ttu-id="1d3d5-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Set](../resources/termstore-set.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1d3d5-130">If successful, this method returns a `200 OK` response code and a [set](../resources/termstore-set.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1d3d5-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="1d3d5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1d3d5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d3d5-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_set"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/sets/{setId}
```


### <a name="response"></a><span data-ttu-id="1d3d5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d3d5-133">Response</span></span>
<span data-ttu-id="1d3d5-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1d3d5-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.set"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{

  "createdDateTime": "2019-06-21T20:01:37Z",  
  "description": "Starting term Set",
  "id": "8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f",
  "localizedNames" : [
    {
      "languageTag" : "en-US",
      "name" : "Department"
    }
  ]
}
```

[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.store]: ../resources/termstore-store.md

<!--
{
  "type": "#page.annotation",
  "description": "Get termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get termSet",
  "suppressions": [
  ]
}
-->
