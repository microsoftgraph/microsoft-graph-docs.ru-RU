---
title: Обновление хранилища
description: Обновление свойств объекта Store.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: cf0c8dfb1eb5915e1a5c7b2b2538959b21cbe0d3
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539416"
---
# <a name="update-store"></a><span data-ttu-id="f24b3-103">Обновление хранилища</span><span class="sxs-lookup"><span data-stu-id="f24b3-103">Update store</span></span>
<span data-ttu-id="f24b3-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="f24b3-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f24b3-105">Обновление свойств объекта [Store](../resources/termstore-store.md) .</span><span class="sxs-lookup"><span data-stu-id="f24b3-105">Update the properties of a [store](../resources/termstore-store.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f24b3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f24b3-106">Permissions</span></span>
<span data-ttu-id="f24b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f24b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f24b3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f24b3-109">Permission type</span></span>|<span data-ttu-id="f24b3-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f24b3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f24b3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f24b3-111">Delegated (work or school account)</span></span> |<span data-ttu-id="f24b3-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f24b3-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="f24b3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f24b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f24b3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f24b3-114">Not supported.</span></span>    |
|<span data-ttu-id="f24b3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f24b3-115">Application</span></span> | <span data-ttu-id="f24b3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f24b3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f24b3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f24b3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}-->

``` http
PATCH /termStore
```

## <a name="request-headers"></a><span data-ttu-id="f24b3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f24b3-118">Request headers</span></span>
|<span data-ttu-id="f24b3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f24b3-119">Name</span></span>|<span data-ttu-id="f24b3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f24b3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f24b3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f24b3-121">Authorization</span></span>|<span data-ttu-id="f24b3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f24b3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f24b3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f24b3-124">Content-Type</span></span>|<span data-ttu-id="f24b3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f24b3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f24b3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f24b3-127">Request body</span></span>
<span data-ttu-id="f24b3-128">В тексте запроса добавьте представление объекта [Store](../resources/termstore-store.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f24b3-128">In the request body, supply a JSON representation of the [store](../resources/termstore-store.md) object.</span></span>

<span data-ttu-id="f24b3-129">В следующей таблице приведены свойства, которые можно изменить для [магазина](../resources/termstore-store.md).</span><span class="sxs-lookup"><span data-stu-id="f24b3-129">The following table shows the properties that can be edited for the [store](../resources/termstore-store.md).</span></span>

|<span data-ttu-id="f24b3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f24b3-130">Property</span></span>|<span data-ttu-id="f24b3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f24b3-131">Type</span></span>|<span data-ttu-id="f24b3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f24b3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f24b3-133">дефаултлангуажетаг</span><span class="sxs-lookup"><span data-stu-id="f24b3-133">defaultLanguageTag</span></span>|<span data-ttu-id="f24b3-134">String</span><span class="sxs-lookup"><span data-stu-id="f24b3-134">String</span></span>|<span data-ttu-id="f24b3-135">Язык по умолчанию для [Microsoft. Graph. банка данных Microsoft. Graph.](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="f24b3-135">Default language of the [microsoft.graph.termstore.store](../resources/termstore-store.md)</span></span>|
|<span data-ttu-id="f24b3-136">лангуажетагс</span><span class="sxs-lookup"><span data-stu-id="f24b3-136">languageTags</span></span>|<span data-ttu-id="f24b3-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f24b3-137">String collection</span></span>|<span data-ttu-id="f24b3-138">Доступные языки в [Microsoft. Graph. банке. Store](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="f24b3-138">Available languages in the [microsoft.graph.termstore.store](../resources/termstore-store.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f24b3-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f24b3-139">Response</span></span>

<span data-ttu-id="f24b3-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [Store](../resources/termstore-store.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f24b3-140">If successful, this method returns a `200 OK` response code and an updated [store](../resources/termstore-store.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f24b3-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="f24b3-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f24b3-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="f24b3-142">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="f24b3-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="f24b3-143">Response</span></span>
<span data-ttu-id="f24b3-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f24b3-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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

