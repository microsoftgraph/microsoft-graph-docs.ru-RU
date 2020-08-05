---
title: Обновление хранилища
description: Обновление свойств объекта Store.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 50a41ab87d3f105eeec04ced231ca8c3aa7e3bee
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565799"
---
# <a name="update-store"></a><span data-ttu-id="4476b-103">Обновление хранилища</span><span class="sxs-lookup"><span data-stu-id="4476b-103">Update store</span></span>
<span data-ttu-id="4476b-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="4476b-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4476b-105">Обновление свойств объекта [Store](../resources/termstore-store.md) .</span><span class="sxs-lookup"><span data-stu-id="4476b-105">Update the properties of a [store](../resources/termstore-store.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4476b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4476b-106">Permissions</span></span>
<span data-ttu-id="4476b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4476b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4476b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4476b-109">Permission type</span></span>|<span data-ttu-id="4476b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4476b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4476b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4476b-111">Delegated (work or school account)</span></span> |<span data-ttu-id="4476b-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4476b-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="4476b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4476b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4476b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4476b-114">Not supported.</span></span>    |
|<span data-ttu-id="4476b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4476b-115">Application</span></span> | <span data-ttu-id="4476b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4476b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4476b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4476b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}-->

``` http
PATCH /termStore
```

## <a name="request-headers"></a><span data-ttu-id="4476b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4476b-118">Request headers</span></span>
|<span data-ttu-id="4476b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4476b-119">Name</span></span>|<span data-ttu-id="4476b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4476b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4476b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4476b-121">Authorization</span></span>|<span data-ttu-id="4476b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4476b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4476b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4476b-124">Content-Type</span></span>|<span data-ttu-id="4476b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4476b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4476b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4476b-127">Request body</span></span>
<span data-ttu-id="4476b-128">В тексте запроса добавьте представление объекта [Store](../resources/termstore-store.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4476b-128">In the request body, supply a JSON representation of the [store](../resources/termstore-store.md) object.</span></span>

<span data-ttu-id="4476b-129">В следующей таблице приведены свойства, которые можно изменить для [магазина](../resources/termstore-store.md).</span><span class="sxs-lookup"><span data-stu-id="4476b-129">The following table shows the properties that can be edited for the [store](../resources/termstore-store.md).</span></span>

|<span data-ttu-id="4476b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4476b-130">Property</span></span>|<span data-ttu-id="4476b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4476b-131">Type</span></span>|<span data-ttu-id="4476b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4476b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4476b-133">дефаултлангуажетаг</span><span class="sxs-lookup"><span data-stu-id="4476b-133">defaultLanguageTag</span></span>|<span data-ttu-id="4476b-134">String</span><span class="sxs-lookup"><span data-stu-id="4476b-134">String</span></span>|<span data-ttu-id="4476b-135">Язык по умолчанию для [Microsoft. Graph. банка данных Microsoft. Graph.](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="4476b-135">Default language of the [microsoft.graph.termstore.store](../resources/termstore-store.md)</span></span>|
|<span data-ttu-id="4476b-136">лангуажетагс</span><span class="sxs-lookup"><span data-stu-id="4476b-136">languageTags</span></span>|<span data-ttu-id="4476b-137">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="4476b-137">String collection</span></span>|<span data-ttu-id="4476b-138">Доступные языки в [Microsoft. Graph. банке. Store](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="4476b-138">Available languages in the [microsoft.graph.termstore.store](../resources/termstore-store.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4476b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4476b-139">Response</span></span>

<span data-ttu-id="4476b-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [Store](../resources/termstore-store.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4476b-140">If successful, this method returns a `200 OK` response code and an updated [store](../resources/termstore-store.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4476b-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="4476b-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4476b-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="4476b-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4476b-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="4476b-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_store"
} -->

``` http
PATCH https://graph.microsoft.com/beta/termStore
Content-Type: application/json
Content-length: 133

{
  "defaultLanguageTag": "en-US"
}
```
# <a name="javascript"></a>[<span data-ttu-id="4476b-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4476b-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-store-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4476b-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4476b-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-store-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4476b-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="4476b-146">Response</span></span>
<span data-ttu-id="4476b-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4476b-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.store"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "dad13b4b-3b4b-dad1-4b3b-d1da4b3bd1da",
  "defaultLanguageTag": "en-US",
  "languageTags": [
    "en-US", 
    "fr-FR"
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Update termstore",
  "suppressions": [
  ]
}
-->

