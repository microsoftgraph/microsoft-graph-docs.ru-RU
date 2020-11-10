---
title: Обновление хранилища
description: Обновление свойств объекта Store.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: e0a4201cda9a6579394eba0872ae93fa9a81bb8e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972320"
---
# <a name="update-store"></a><span data-ttu-id="032a1-103">Обновление хранилища</span><span class="sxs-lookup"><span data-stu-id="032a1-103">Update store</span></span>
<span data-ttu-id="032a1-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="032a1-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="032a1-105">Обновление свойств объекта [Store](../resources/termstore-store.md) .</span><span class="sxs-lookup"><span data-stu-id="032a1-105">Update the properties of a [store](../resources/termstore-store.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="032a1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="032a1-106">Permissions</span></span>
<span data-ttu-id="032a1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="032a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="032a1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="032a1-109">Permission type</span></span>|<span data-ttu-id="032a1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="032a1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="032a1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="032a1-111">Delegated (work or school account)</span></span> |<span data-ttu-id="032a1-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="032a1-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="032a1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="032a1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="032a1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="032a1-114">Not supported.</span></span>    |
|<span data-ttu-id="032a1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="032a1-115">Application</span></span> | <span data-ttu-id="032a1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="032a1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="032a1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="032a1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}-->

``` http
PATCH /termStore
```

## <a name="request-headers"></a><span data-ttu-id="032a1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="032a1-118">Request headers</span></span>
|<span data-ttu-id="032a1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="032a1-119">Name</span></span>|<span data-ttu-id="032a1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="032a1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="032a1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="032a1-121">Authorization</span></span>|<span data-ttu-id="032a1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="032a1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="032a1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="032a1-124">Content-Type</span></span>|<span data-ttu-id="032a1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="032a1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="032a1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="032a1-127">Request body</span></span>
<span data-ttu-id="032a1-128">В тексте запроса добавьте представление объекта [Store](../resources/termstore-store.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="032a1-128">In the request body, supply a JSON representation of the [store](../resources/termstore-store.md) object.</span></span>

<span data-ttu-id="032a1-129">В следующей таблице приведены свойства, которые можно изменить для [магазина](../resources/termstore-store.md).</span><span class="sxs-lookup"><span data-stu-id="032a1-129">The following table shows the properties that can be edited for the [store](../resources/termstore-store.md).</span></span>

|<span data-ttu-id="032a1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="032a1-130">Property</span></span>|<span data-ttu-id="032a1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="032a1-131">Type</span></span>|<span data-ttu-id="032a1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="032a1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="032a1-133">дефаултлангуажетаг</span><span class="sxs-lookup"><span data-stu-id="032a1-133">defaultLanguageTag</span></span>|<span data-ttu-id="032a1-134">String</span><span class="sxs-lookup"><span data-stu-id="032a1-134">String</span></span>|<span data-ttu-id="032a1-135">Язык по умолчанию для [Microsoft. Graph. банка данных Microsoft. Graph.](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="032a1-135">Default language of the [microsoft.graph.termstore.store](../resources/termstore-store.md)</span></span>|
|<span data-ttu-id="032a1-136">лангуажетагс</span><span class="sxs-lookup"><span data-stu-id="032a1-136">languageTags</span></span>|<span data-ttu-id="032a1-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="032a1-137">String collection</span></span>|<span data-ttu-id="032a1-138">Доступные языки в [Microsoft. Graph. банке. Store](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="032a1-138">Available languages in the [microsoft.graph.termstore.store](../resources/termstore-store.md)</span></span>|



## <a name="response"></a><span data-ttu-id="032a1-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="032a1-139">Response</span></span>

<span data-ttu-id="032a1-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [Store](../resources/termstore-store.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="032a1-140">If successful, this method returns a `200 OK` response code and an updated [store](../resources/termstore-store.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="032a1-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="032a1-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="032a1-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="032a1-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="032a1-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="032a1-143">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="032a1-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="032a1-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-store-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="032a1-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="032a1-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-store-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="032a1-146">C#</span><span class="sxs-lookup"><span data-stu-id="032a1-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-store-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="032a1-147">Java</span><span class="sxs-lookup"><span data-stu-id="032a1-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-store-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="032a1-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="032a1-148">Response</span></span>
<span data-ttu-id="032a1-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="032a1-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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



