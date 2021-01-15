---
title: Обновление магазина
description: Обновление свойств объекта store.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 73d1fb22b92c134fc4ebb2b15fe4b9314dce2d5d
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874104"
---
# <a name="update-store"></a><span data-ttu-id="1b91a-103">Обновление магазина</span><span class="sxs-lookup"><span data-stu-id="1b91a-103">Update store</span></span>
<span data-ttu-id="1b91a-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="1b91a-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b91a-105">Обновление свойств объекта [store.](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="1b91a-105">Update the properties of a [store](../resources/termstore-store.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b91a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b91a-106">Permissions</span></span>
<span data-ttu-id="1b91a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b91a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b91a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b91a-109">Permission type</span></span>|<span data-ttu-id="1b91a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b91a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b91a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b91a-111">Delegated (work or school account)</span></span> |<span data-ttu-id="1b91a-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b91a-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="1b91a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b91a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b91a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b91a-114">Not supported.</span></span>    |
|<span data-ttu-id="1b91a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b91a-115">Application</span></span> | <span data-ttu-id="1b91a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b91a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b91a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b91a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}-->

``` http
PATCH /termStore
```

## <a name="request-headers"></a><span data-ttu-id="1b91a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b91a-118">Request headers</span></span>
|<span data-ttu-id="1b91a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1b91a-119">Name</span></span>|<span data-ttu-id="1b91a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1b91a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1b91a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b91a-121">Authorization</span></span>|<span data-ttu-id="1b91a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b91a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1b91a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1b91a-124">Content-Type</span></span>|<span data-ttu-id="1b91a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b91a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b91a-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b91a-127">Request body</span></span>
<span data-ttu-id="1b91a-128">В теле запроса укажу представление объекта [store](../resources/termstore-store.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="1b91a-128">In the request body, supply a JSON representation of the [store](../resources/termstore-store.md) object.</span></span>

<span data-ttu-id="1b91a-129">В следующей таблице показаны свойства, которые можно изменить для [магазина.](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="1b91a-129">The following table shows the properties that can be edited for the [store](../resources/termstore-store.md).</span></span>

|<span data-ttu-id="1b91a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b91a-130">Property</span></span>|<span data-ttu-id="1b91a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1b91a-131">Type</span></span>|<span data-ttu-id="1b91a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1b91a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b91a-133">defaultLanguageTag</span><span class="sxs-lookup"><span data-stu-id="1b91a-133">defaultLanguageTag</span></span>|<span data-ttu-id="1b91a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1b91a-134">String</span></span>|<span data-ttu-id="1b91a-135">Язык по умолчанию [для microsoft.graph.termstore.store](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="1b91a-135">Default language of the [microsoft.graph.termstore.store](../resources/termstore-store.md)</span></span>|
|<span data-ttu-id="1b91a-136">languageTags</span><span class="sxs-lookup"><span data-stu-id="1b91a-136">languageTags</span></span>|<span data-ttu-id="1b91a-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1b91a-137">String collection</span></span>|<span data-ttu-id="1b91a-138">Доступные языки [в microsoft.graph.termstore.store](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="1b91a-138">Available languages in the [microsoft.graph.termstore.store](../resources/termstore-store.md)</span></span>|



## <a name="response"></a><span data-ttu-id="1b91a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b91a-139">Response</span></span>

<span data-ttu-id="1b91a-140">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [store](../resources/termstore-store.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b91a-140">If successful, this method returns a `200 OK` response code and an updated [store](../resources/termstore-store.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b91a-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="1b91a-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1b91a-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b91a-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1b91a-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b91a-143">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="1b91a-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b91a-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-store-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b91a-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b91a-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-store-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="1b91a-146">C#</span><span class="sxs-lookup"><span data-stu-id="1b91a-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-store-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b91a-147">Java</span><span class="sxs-lookup"><span data-stu-id="1b91a-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-store-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="1b91a-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b91a-148">Response</span></span>
<span data-ttu-id="1b91a-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1b91a-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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



