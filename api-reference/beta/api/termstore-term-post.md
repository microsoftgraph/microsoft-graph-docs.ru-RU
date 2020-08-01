---
title: Создание термина
description: Создание нового объекта Term.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 2d2c18f802d9dfe68aa17b46c4dc196a31e3f93c
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539415"
---
# <a name="create-term"></a><span data-ttu-id="d3d43-103">Создание термина</span><span class="sxs-lookup"><span data-stu-id="d3d43-103">Create term</span></span>
<span data-ttu-id="d3d43-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="d3d43-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3d43-105">Создание нового объекта [Term](../resources/termstore-term.md) .</span><span class="sxs-lookup"><span data-stu-id="d3d43-105">Create a new [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3d43-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3d43-106">Permissions</span></span>
<span data-ttu-id="d3d43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3d43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3d43-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3d43-109">Permission type</span></span>|<span data-ttu-id="d3d43-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3d43-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3d43-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3d43-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d3d43-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3d43-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="d3d43-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3d43-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3d43-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3d43-114">Not supported.</span></span>    |
|<span data-ttu-id="d3d43-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3d43-115">Application</span></span> | <span data-ttu-id="d3d43-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3d43-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="d3d43-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3d43-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
} -->

``` http
POST /termStore/sets/{setId}/children
POST /termStore/sets/{setId}/terms/{termId}/children
```

## <a name="request-headers"></a><span data-ttu-id="d3d43-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3d43-118">Request headers</span></span>
|<span data-ttu-id="d3d43-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d3d43-119">Name</span></span>|<span data-ttu-id="d3d43-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d3d43-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d3d43-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3d43-121">Authorization</span></span>|<span data-ttu-id="d3d43-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3d43-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d3d43-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d3d43-124">Content-Type</span></span>|<span data-ttu-id="d3d43-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3d43-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3d43-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3d43-127">Request body</span></span>
<span data-ttu-id="d3d43-128">В тексте запроса добавьте представление объекта [Term](../resources/termstore-term.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3d43-128">In the request body, supply a JSON representation of the [term](../resources/termstore-term.md) object.</span></span>

<span data-ttu-id="d3d43-129">В следующей таблице приведены свойства, необходимые при создании [термина](../resources/termstore-term.md).</span><span class="sxs-lookup"><span data-stu-id="d3d43-129">The following table shows the properties that are required when you create the [term](../resources/termstore-term.md).</span></span>

|<span data-ttu-id="d3d43-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3d43-130">Property</span></span>|<span data-ttu-id="d3d43-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d3d43-131">Type</span></span>|<span data-ttu-id="d3d43-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d3d43-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3d43-133">Метка</span><span class="sxs-lookup"><span data-stu-id="d3d43-133">labels</span></span>|<span data-ttu-id="d3d43-134">Коллекция [Microsoft. Graph. банка Microsoft. Graph. локализедлабел](../resources/termstore-localizedlabel.md)</span><span class="sxs-lookup"><span data-stu-id="d3d43-134">[microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md) collection</span></span>|<span data-ttu-id="d3d43-135">Метка для создаваемого термина</span><span class="sxs-lookup"><span data-stu-id="d3d43-135">Label for the term to be created</span></span>|



## <a name="response"></a><span data-ttu-id="d3d43-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3d43-136">Response</span></span>

<span data-ttu-id="d3d43-137">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Term](../resources/termstore-term.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d3d43-137">If successful, this method returns a `201 Created` response code and a [term](../resources/termstore-term.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d3d43-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="d3d43-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d3d43-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3d43-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_term_from_"
} -->

``` http
POST https://graph.microsoft.com/beta/termStore/sets/{setId}/terms
Content-Type: application/json
Content-length: 366

{
  "labels": [
    {
      "languageTag" : "en-US",
      "name" : "Car",
      "isDefault" : true
    }
  ]
}
```


### <a name="response"></a><span data-ttu-id="d3d43-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3d43-140">Response</span></span>
<span data-ttu-id="d3d43-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d3d43-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.term"
}-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "createdDateTime": "2019-06-21T20:01:37Z",
  "id": "8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f",
  "labels" : [
      {
          "name" : "Car",
          "languageTag" : "en-US",
          "isDefault" : true
      }
  ],
  "lastModifiedDateTime": "2019-06-21T20:01:37Z"
}
```

[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Post term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Post term",
  "suppressions": [
  ]
}
-->
