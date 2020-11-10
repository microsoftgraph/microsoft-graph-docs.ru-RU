---
title: Создание термина
description: Создание нового объекта Term.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: e09f892019ee48aeed61f20234856b8d799cd3ae
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972228"
---
# <a name="create-term"></a><span data-ttu-id="c4668-103">Создание термина</span><span class="sxs-lookup"><span data-stu-id="c4668-103">Create term</span></span>
<span data-ttu-id="c4668-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="c4668-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4668-105">Создание нового объекта [Term](../resources/termstore-term.md) .</span><span class="sxs-lookup"><span data-stu-id="c4668-105">Create a new [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4668-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4668-106">Permissions</span></span>
<span data-ttu-id="c4668-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4668-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4668-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4668-109">Permission type</span></span>|<span data-ttu-id="c4668-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4668-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4668-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4668-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c4668-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4668-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="c4668-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4668-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4668-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4668-114">Not supported.</span></span>    |
|<span data-ttu-id="c4668-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4668-115">Application</span></span> | <span data-ttu-id="c4668-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4668-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="c4668-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4668-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
} -->

``` http
POST /termStore/sets/{setId}/children
POST /termStore/sets/{setId}/terms/{termId}/children
```

## <a name="request-headers"></a><span data-ttu-id="c4668-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4668-118">Request headers</span></span>
|<span data-ttu-id="c4668-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c4668-119">Name</span></span>|<span data-ttu-id="c4668-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c4668-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c4668-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4668-121">Authorization</span></span>|<span data-ttu-id="c4668-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4668-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c4668-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4668-124">Content-Type</span></span>|<span data-ttu-id="c4668-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4668-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4668-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4668-127">Request body</span></span>
<span data-ttu-id="c4668-128">В тексте запроса добавьте представление объекта [Term](../resources/termstore-term.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4668-128">In the request body, supply a JSON representation of the [term](../resources/termstore-term.md) object.</span></span>

<span data-ttu-id="c4668-129">В следующей таблице приведены свойства, необходимые при создании [термина](../resources/termstore-term.md).</span><span class="sxs-lookup"><span data-stu-id="c4668-129">The following table shows the properties that are required when you create the [term](../resources/termstore-term.md).</span></span>

|<span data-ttu-id="c4668-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4668-130">Property</span></span>|<span data-ttu-id="c4668-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c4668-131">Type</span></span>|<span data-ttu-id="c4668-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c4668-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4668-133">Метка</span><span class="sxs-lookup"><span data-stu-id="c4668-133">labels</span></span>|<span data-ttu-id="c4668-134">Коллекция [Microsoft. Graph. банка Microsoft. Graph. локализедлабел](../resources/termstore-localizedlabel.md)</span><span class="sxs-lookup"><span data-stu-id="c4668-134">[microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md) collection</span></span>|<span data-ttu-id="c4668-135">Метка для создаваемого термина</span><span class="sxs-lookup"><span data-stu-id="c4668-135">Label for the term to be created</span></span>|



## <a name="response"></a><span data-ttu-id="c4668-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4668-136">Response</span></span>

<span data-ttu-id="c4668-137">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Term](../resources/termstore-term.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c4668-137">If successful, this method returns a `201 Created` response code and a [term](../resources/termstore-term.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c4668-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="c4668-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c4668-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4668-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c4668-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4668-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c4668-141">C#</span><span class="sxs-lookup"><span data-stu-id="c4668-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-term-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4668-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4668-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-term-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4668-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4668-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-term-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4668-144">Java</span><span class="sxs-lookup"><span data-stu-id="c4668-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-term-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c4668-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4668-145">Response</span></span>
<span data-ttu-id="c4668-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c4668-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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


