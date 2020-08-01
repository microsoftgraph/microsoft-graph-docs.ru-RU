---
title: Набор обновлений
description: Обновление свойств объекта Set.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: cf2910e70b9eabf79a925f36be911427b31a8d9e
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539485"
---
# <a name="update-set"></a><span data-ttu-id="d8cc6-103">Набор обновлений</span><span class="sxs-lookup"><span data-stu-id="d8cc6-103">Update set</span></span>
<span data-ttu-id="d8cc6-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="d8cc6-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8cc6-105">Обновление свойств объекта [Set](../resources/termstore-set.md) .</span><span class="sxs-lookup"><span data-stu-id="d8cc6-105">Update the properties of a [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8cc6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8cc6-106">Permissions</span></span>
<span data-ttu-id="d8cc6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8cc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8cc6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8cc6-109">Permission type</span></span>|<span data-ttu-id="d8cc6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8cc6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8cc6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8cc6-111">Delegated (work or school account)</span></span> |<span data-ttu-id="d8cc6-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8cc6-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="d8cc6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8cc6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8cc6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8cc6-114">Not supported.</span></span>    |
|<span data-ttu-id="d8cc6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8cc6-115">Application</span></span> | <span data-ttu-id="d8cc6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8cc6-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="d8cc6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8cc6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /termStore/sets/{setId}
```

## <a name="request-headers"></a><span data-ttu-id="d8cc6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8cc6-118">Request headers</span></span>
|<span data-ttu-id="d8cc6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d8cc6-119">Name</span></span>|<span data-ttu-id="d8cc6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d8cc6-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d8cc6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8cc6-121">Authorization</span></span>|<span data-ttu-id="d8cc6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8cc6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d8cc6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d8cc6-124">Content-Type</span></span>|<span data-ttu-id="d8cc6-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8cc6-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8cc6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8cc6-127">Request body</span></span>
<span data-ttu-id="d8cc6-128">В тексте запроса добавьте представление объекта [Set](../resources/termstore-set.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8cc6-128">In the request body, supply a JSON representation of the [set](../resources/termstore-set.md) object.</span></span>

<span data-ttu-id="d8cc6-129">В следующей таблице приведены свойства, которые можно изменить для [набора](../resources/termstore-set.md).</span><span class="sxs-lookup"><span data-stu-id="d8cc6-129">The following table shows the properties that can be edited for the [set](../resources/termstore-set.md).</span></span>

|<span data-ttu-id="d8cc6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8cc6-130">Property</span></span>|<span data-ttu-id="d8cc6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d8cc6-131">Type</span></span>|<span data-ttu-id="d8cc6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d8cc6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8cc6-133">локализеднамес</span><span class="sxs-lookup"><span data-stu-id="d8cc6-133">localizedNames</span></span>|<span data-ttu-id="d8cc6-134">Коллекция [Microsoft. Graph. банка Microsoft. Graph. локализеднаме](../resources/termstore-localizedname.md)</span><span class="sxs-lookup"><span data-stu-id="d8cc6-134">[microsoft.graph.termStore.localizedName](../resources/termstore-localizedname.md) collection</span></span>|<span data-ttu-id="d8cc6-135">Имя набора</span><span class="sxs-lookup"><span data-stu-id="d8cc6-135">Name of the set</span></span>|
|<span data-ttu-id="d8cc6-136">description</span><span class="sxs-lookup"><span data-stu-id="d8cc6-136">description</span></span>|<span data-ttu-id="d8cc6-137">String</span><span class="sxs-lookup"><span data-stu-id="d8cc6-137">String</span></span>|<span data-ttu-id="d8cc6-138">Описание набора</span><span class="sxs-lookup"><span data-stu-id="d8cc6-138">Description of the set</span></span>|
|<span data-ttu-id="d8cc6-139">properties</span><span class="sxs-lookup"><span data-stu-id="d8cc6-139">properties</span></span>|<span data-ttu-id="d8cc6-140">Коллекция [Microsoft. Graph. ключзначение](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d8cc6-140">[microsoft.graph.keyValue](../resources/keyvalue.md) collection</span></span>|<span data-ttu-id="d8cc6-141">Свойства набора</span><span class="sxs-lookup"><span data-stu-id="d8cc6-141">properties of a set</span></span>|



## <a name="response"></a><span data-ttu-id="d8cc6-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8cc6-142">Response</span></span>

<span data-ttu-id="d8cc6-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [Set](../resources/termstore-set.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d8cc6-143">If successful, this method returns a `200 OK` response code and an updated [set](../resources/termstore-set.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d8cc6-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="d8cc6-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d8cc6-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8cc6-145">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_set"
} -->

``` http
PATCH https://graph.microsoft.com/beta/termStore/sets/{setId}
Content-Type: application/json
Content-length: 288

{
  "description": "mySet"
}
```


### <a name="response"></a><span data-ttu-id="d8cc6-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8cc6-146">Response</span></span>

<span data-ttu-id="d8cc6-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d8cc6-147">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.set"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "3607e9f9-e9f9-3607-f9e9-0736f9e90736",
  "description": "mySet",    
  "localizedNames" : [
    {
      "languageTag" : "en-US",
      "name" : "Department"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Update termSet",
  "suppressions": [
  ]
}
-->
