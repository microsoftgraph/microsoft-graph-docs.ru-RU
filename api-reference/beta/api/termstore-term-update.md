---
title: Термин "Обновление"
description: Обновление свойств объекта термина.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 1168407425b0ef8faff213fd807f9499317e0f7b
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874384"
---
# <a name="update-term"></a><span data-ttu-id="64e06-103">Термин "Обновление"</span><span class="sxs-lookup"><span data-stu-id="64e06-103">Update term</span></span>
<span data-ttu-id="64e06-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="64e06-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64e06-105">Обновление свойств объекта [термина.](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="64e06-105">Update the properties of a [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="64e06-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64e06-106">Permissions</span></span>
<span data-ttu-id="64e06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64e06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64e06-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64e06-109">Permission type</span></span>|<span data-ttu-id="64e06-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64e06-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64e06-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64e06-111">Delegated (work or school account)</span></span> | <span data-ttu-id="64e06-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64e06-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="64e06-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64e06-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64e06-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64e06-114">Not supported.</span></span>    |
|<span data-ttu-id="64e06-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64e06-115">Application</span></span> | <span data-ttu-id="64e06-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64e06-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="64e06-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64e06-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}-->

``` http
PATCH /termStore/sets/{setId}/terms/{termId}
```

## <a name="request-headers"></a><span data-ttu-id="64e06-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64e06-118">Request headers</span></span>
|<span data-ttu-id="64e06-119">Имя</span><span class="sxs-lookup"><span data-stu-id="64e06-119">Name</span></span>|<span data-ttu-id="64e06-120">Описание</span><span class="sxs-lookup"><span data-stu-id="64e06-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="64e06-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64e06-121">Authorization</span></span>|<span data-ttu-id="64e06-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64e06-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="64e06-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="64e06-124">Content-Type</span></span>|<span data-ttu-id="64e06-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64e06-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64e06-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="64e06-127">Request body</span></span>
<span data-ttu-id="64e06-128">В теле запроса укажу представление объекта термина в [JSON.](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="64e06-128">In the request body, supply a JSON representation of the [term](../resources/termstore-term.md) object.</span></span>

<span data-ttu-id="64e06-129">В следующей таблице показаны свойства, которые можно обновить для [термина.](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="64e06-129">The following table shows the properties that can be updated for a [term](../resources/termstore-term.md).</span></span>

|<span data-ttu-id="64e06-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="64e06-130">Property</span></span>|<span data-ttu-id="64e06-131">Тип</span><span class="sxs-lookup"><span data-stu-id="64e06-131">Type</span></span>|<span data-ttu-id="64e06-132">Описание</span><span class="sxs-lookup"><span data-stu-id="64e06-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64e06-133">labels</span><span class="sxs-lookup"><span data-stu-id="64e06-133">labels</span></span>|<span data-ttu-id="64e06-134">[Коллекция microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md)</span><span class="sxs-lookup"><span data-stu-id="64e06-134">[microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md) collection</span></span>|<span data-ttu-id="64e06-135">метки термина</span><span class="sxs-lookup"><span data-stu-id="64e06-135">labels of a term</span></span>|
|<span data-ttu-id="64e06-136">descriptions</span><span class="sxs-lookup"><span data-stu-id="64e06-136">descriptions</span></span>|<span data-ttu-id="64e06-137">[Коллекция microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md)</span><span class="sxs-lookup"><span data-stu-id="64e06-137">[microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md) collection</span></span>|<span data-ttu-id="64e06-138">описание термина</span><span class="sxs-lookup"><span data-stu-id="64e06-138">description about the term</span></span>|
|<span data-ttu-id="64e06-139">properties</span><span class="sxs-lookup"><span data-stu-id="64e06-139">properties</span></span>|<span data-ttu-id="64e06-140">[Коллекция microsoft.graph.keyValue](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="64e06-140">[microsoft.graph.keyValue](../resources/keyvalue.md) collection</span></span>|<span data-ttu-id="64e06-141">свойства, связанные с термином</span><span class="sxs-lookup"><span data-stu-id="64e06-141">properties associated with the term</span></span>|



## <a name="response"></a><span data-ttu-id="64e06-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="64e06-142">Response</span></span>

<span data-ttu-id="64e06-143">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` термина в тексте отклика. [](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="64e06-143">If successful, this method returns a `200 OK` response code and an updated [term](../resources/termstore-term.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64e06-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="64e06-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="64e06-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="64e06-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="64e06-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="64e06-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_term"
} -->

``` http
PATCH https://graph.microsoft.com/beta/termStore/sets/{setId}/terms/{termId}
Content-Type: application/json
Content-length: 366

{
  "labels" : [
      {
          "name" : "changedLabel",
          "languageTag" : "en-US",
          "isDefault" : true
      }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="64e06-147">C#</span><span class="sxs-lookup"><span data-stu-id="64e06-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-term-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64e06-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64e06-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-term-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64e06-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64e06-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-term-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64e06-150">Java</span><span class="sxs-lookup"><span data-stu-id="64e06-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-term-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="64e06-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="64e06-151">Response</span></span>
<span data-ttu-id="64e06-152">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="64e06-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.term"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "81be9856-9856-81be-5698-be815698be81",
  "labels" : [
      {
          "name" : "changedLabel",
          "languageTag" : "en-US",
          "isDefault" : true
      }
  ]
}
```

[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Get term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Update term",
  "suppressions": [
  ]
}
-->


