---
title: Обновление набора
description: Обновление свойств объекта set.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: fe2b221bc6e6852af5d8aadcf283e851e1c47872
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872060"
---
# <a name="update-set"></a><span data-ttu-id="71ac1-103">Обновление набора</span><span class="sxs-lookup"><span data-stu-id="71ac1-103">Update set</span></span>
<span data-ttu-id="71ac1-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="71ac1-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71ac1-105">Обновление свойств объекта [set.](../resources/termstore-set.md)</span><span class="sxs-lookup"><span data-stu-id="71ac1-105">Update the properties of a [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="71ac1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71ac1-106">Permissions</span></span>
<span data-ttu-id="71ac1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71ac1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71ac1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71ac1-109">Permission type</span></span>|<span data-ttu-id="71ac1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71ac1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71ac1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71ac1-111">Delegated (work or school account)</span></span> |<span data-ttu-id="71ac1-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71ac1-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="71ac1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71ac1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71ac1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71ac1-114">Not supported.</span></span>    |
|<span data-ttu-id="71ac1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71ac1-115">Application</span></span> | <span data-ttu-id="71ac1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71ac1-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="71ac1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71ac1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /termStore/sets/{setId}
```

## <a name="request-headers"></a><span data-ttu-id="71ac1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71ac1-118">Request headers</span></span>
|<span data-ttu-id="71ac1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="71ac1-119">Name</span></span>|<span data-ttu-id="71ac1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="71ac1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="71ac1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71ac1-121">Authorization</span></span>|<span data-ttu-id="71ac1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71ac1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="71ac1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="71ac1-124">Content-Type</span></span>|<span data-ttu-id="71ac1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71ac1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71ac1-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="71ac1-127">Request body</span></span>
<span data-ttu-id="71ac1-128">В теле запроса укажу представление объекта [set](../resources/termstore-set.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="71ac1-128">In the request body, supply a JSON representation of the [set](../resources/termstore-set.md) object.</span></span>

<span data-ttu-id="71ac1-129">В следующей таблице показаны свойства, которые можно изменить для [набора.](../resources/termstore-set.md)</span><span class="sxs-lookup"><span data-stu-id="71ac1-129">The following table shows the properties that can be edited for the [set](../resources/termstore-set.md).</span></span>

|<span data-ttu-id="71ac1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="71ac1-130">Property</span></span>|<span data-ttu-id="71ac1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="71ac1-131">Type</span></span>|<span data-ttu-id="71ac1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="71ac1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71ac1-133">localizedNames</span><span class="sxs-lookup"><span data-stu-id="71ac1-133">localizedNames</span></span>|<span data-ttu-id="71ac1-134">[Коллекция microsoft.graph.termStore.localizedName](../resources/termstore-localizedname.md)</span><span class="sxs-lookup"><span data-stu-id="71ac1-134">[microsoft.graph.termStore.localizedName](../resources/termstore-localizedname.md) collection</span></span>|<span data-ttu-id="71ac1-135">Имя набора</span><span class="sxs-lookup"><span data-stu-id="71ac1-135">Name of the set</span></span>|
|<span data-ttu-id="71ac1-136">description</span><span class="sxs-lookup"><span data-stu-id="71ac1-136">description</span></span>|<span data-ttu-id="71ac1-137">String</span><span class="sxs-lookup"><span data-stu-id="71ac1-137">String</span></span>|<span data-ttu-id="71ac1-138">Описание набора</span><span class="sxs-lookup"><span data-stu-id="71ac1-138">Description of the set</span></span>|
|<span data-ttu-id="71ac1-139">properties</span><span class="sxs-lookup"><span data-stu-id="71ac1-139">properties</span></span>|<span data-ttu-id="71ac1-140">[Коллекция microsoft.graph.keyValue](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="71ac1-140">[microsoft.graph.keyValue](../resources/keyvalue.md) collection</span></span>|<span data-ttu-id="71ac1-141">свойства набора</span><span class="sxs-lookup"><span data-stu-id="71ac1-141">properties of a set</span></span>|



## <a name="response"></a><span data-ttu-id="71ac1-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="71ac1-142">Response</span></span>

<span data-ttu-id="71ac1-143">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` набора в тексте отклика. [](../resources/termstore-set.md)</span><span class="sxs-lookup"><span data-stu-id="71ac1-143">If successful, this method returns a `200 OK` response code and an updated [set](../resources/termstore-set.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="71ac1-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="71ac1-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="71ac1-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="71ac1-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="71ac1-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="71ac1-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="71ac1-147">C#</span><span class="sxs-lookup"><span data-stu-id="71ac1-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-set-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71ac1-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71ac1-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-set-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71ac1-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71ac1-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-set-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71ac1-150">Java</span><span class="sxs-lookup"><span data-stu-id="71ac1-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-set-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="71ac1-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="71ac1-151">Response</span></span>

<span data-ttu-id="71ac1-152">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="71ac1-152">**Note:** The response object shown here might be shortened for readability.</span></span>

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


