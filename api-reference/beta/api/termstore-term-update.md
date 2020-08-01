---
title: Обновление термина
description: Обновление свойств объекта Term.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: cce2fadc8dd2990f4b58b74dad554050f8e526d2
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539411"
---
# <a name="update-term"></a><span data-ttu-id="6af63-103">Обновление термина</span><span class="sxs-lookup"><span data-stu-id="6af63-103">Update term</span></span>
<span data-ttu-id="6af63-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="6af63-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6af63-105">Обновление свойств объекта [Term](../resources/termstore-term.md) .</span><span class="sxs-lookup"><span data-stu-id="6af63-105">Update the properties of a [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6af63-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6af63-106">Permissions</span></span>
<span data-ttu-id="6af63-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6af63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6af63-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6af63-109">Permission type</span></span>|<span data-ttu-id="6af63-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6af63-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6af63-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6af63-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6af63-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6af63-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="6af63-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6af63-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6af63-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6af63-114">Not supported.</span></span>    |
|<span data-ttu-id="6af63-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6af63-115">Application</span></span> | <span data-ttu-id="6af63-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6af63-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="6af63-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6af63-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}-->

``` http
PATCH /termStore/sets/{setId}/terms/{termId}
```

## <a name="request-headers"></a><span data-ttu-id="6af63-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6af63-118">Request headers</span></span>
|<span data-ttu-id="6af63-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6af63-119">Name</span></span>|<span data-ttu-id="6af63-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6af63-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6af63-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6af63-121">Authorization</span></span>|<span data-ttu-id="6af63-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6af63-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6af63-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6af63-124">Content-Type</span></span>|<span data-ttu-id="6af63-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6af63-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6af63-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6af63-127">Request body</span></span>
<span data-ttu-id="6af63-128">В тексте запроса добавьте представление объекта [Term](../resources/termstore-term.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6af63-128">In the request body, supply a JSON representation of the [term](../resources/termstore-term.md) object.</span></span>

<span data-ttu-id="6af63-129">В следующей таблице приведены свойства, которые можно обновить для [термина](../resources/termstore-term.md).</span><span class="sxs-lookup"><span data-stu-id="6af63-129">The following table shows the properties that can be updated for a [term](../resources/termstore-term.md).</span></span>

|<span data-ttu-id="6af63-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6af63-130">Property</span></span>|<span data-ttu-id="6af63-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6af63-131">Type</span></span>|<span data-ttu-id="6af63-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6af63-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6af63-133">Метка</span><span class="sxs-lookup"><span data-stu-id="6af63-133">labels</span></span>|<span data-ttu-id="6af63-134">Коллекция [Microsoft. Graph. банка Microsoft. Graph. локализедлабел](../resources/termstore-localizedlabel.md)</span><span class="sxs-lookup"><span data-stu-id="6af63-134">[microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md) collection</span></span>|<span data-ttu-id="6af63-135">Метки термина</span><span class="sxs-lookup"><span data-stu-id="6af63-135">labels of a term</span></span>|
|<span data-ttu-id="6af63-136">состояний</span><span class="sxs-lookup"><span data-stu-id="6af63-136">descriptions</span></span>|<span data-ttu-id="6af63-137">Коллекция [Microsoft. Graph. банка Microsoft. Graph. локализеддескриптион](../resources/termstore-localizeddescription.md)</span><span class="sxs-lookup"><span data-stu-id="6af63-137">[microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md) collection</span></span>|<span data-ttu-id="6af63-138">Описание термина</span><span class="sxs-lookup"><span data-stu-id="6af63-138">description about the term</span></span>|
|<span data-ttu-id="6af63-139">properties</span><span class="sxs-lookup"><span data-stu-id="6af63-139">properties</span></span>|<span data-ttu-id="6af63-140">Коллекция [Microsoft. Graph. ключзначение](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6af63-140">[microsoft.graph.keyValue](../resources/keyvalue.md) collection</span></span>|<span data-ttu-id="6af63-141">свойства, связанные с термином</span><span class="sxs-lookup"><span data-stu-id="6af63-141">properties associated with the term</span></span>|



## <a name="response"></a><span data-ttu-id="6af63-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="6af63-142">Response</span></span>

<span data-ttu-id="6af63-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [Term](../resources/termstore-term.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6af63-143">If successful, this method returns a `200 OK` response code and an updated [term](../resources/termstore-term.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6af63-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="6af63-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6af63-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="6af63-145">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="6af63-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="6af63-146">Response</span></span>
<span data-ttu-id="6af63-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6af63-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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
