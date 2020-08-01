---
title: Список дочерних элементов
description: Получение терминов из свойства навигации Children.
author: mohitpcad
ms.prod: Sharepoint
localization_priority: Normal
doc_type: apiPageType
ms.openlocfilehash: b33b2ac40a489909d23183319b6c8f0fe2506c60
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539439"
---
# <a name="list-children"></a><span data-ttu-id="f4497-103">Список дочерних элементов</span><span class="sxs-lookup"><span data-stu-id="f4497-103">List children</span></span>
<span data-ttu-id="f4497-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="f4497-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4497-105">Получение потомков первого уровня ресурса " [набор] " или " [термин] " с помощью свойства навигации Children.</span><span class="sxs-lookup"><span data-stu-id="f4497-105">Get the first level children of a [set] or [term] resource using the children navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4497-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f4497-106">Permissions</span></span>
<span data-ttu-id="f4497-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4497-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4497-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4497-109">Permission type</span></span>|<span data-ttu-id="f4497-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4497-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4497-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4497-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f4497-112">Банк. чтение. ALL, банк. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f4497-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="f4497-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4497-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4497-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4497-114">Not supported.</span></span>    |
|<span data-ttu-id="f4497-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4497-115">Application</span></span> | <span data-ttu-id="f4497-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4497-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4497-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4497-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /termStore/sets/{setId}/children
GET /termStore/sets/{setId}/terms/{termId}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4497-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f4497-118">Optional query parameters</span></span>
<span data-ttu-id="f4497-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f4497-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f4497-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f4497-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4497-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4497-121">Request headers</span></span>
|<span data-ttu-id="f4497-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f4497-122">Name</span></span>|<span data-ttu-id="f4497-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f4497-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f4497-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4497-124">Authorization</span></span>|<span data-ttu-id="f4497-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4497-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4497-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4497-127">Request body</span></span>
<span data-ttu-id="f4497-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f4497-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4497-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4497-129">Response</span></span>

<span data-ttu-id="f4497-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Term](../resources/termstore-term.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f4497-130">If successful, this method returns a `200 OK` response code and a collection of [term](../resources/termstore-term.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f4497-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="f4497-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f4497-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4497-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_term"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/sets/{setId}/children
```


### <a name="response"></a><span data-ttu-id="f4497-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4497-133">Response</span></span>
<span data-ttu-id="f4497-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f4497-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.termStore.term)"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {      
      "id": "81be9856-9856-81be-5698-be815698be81",
      "labels" : [
        {
          "name" : "Car",
          "languageTag" : "en-US",
          "isDefault" : true
        }
      ],
      "lastModifiedDateTime": "2019-06-21T20:01:37Z"
   }  
 ]
}
```

[банком]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md
[set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "Get children of a term or termSet in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get termchildren",
  "suppressions": []
}
-->
