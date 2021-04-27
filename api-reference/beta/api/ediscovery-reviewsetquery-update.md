---
title: Обновление обзораSetQuery
description: Обновление свойств объекта reviewSetQuery.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: d5ce888c2b4a32e175ddc69e2edc6f2df0fc0411
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044552"
---
# <a name="update-reviewsetquery"></a><span data-ttu-id="bd33a-103">Обновление обзораSetQuery</span><span class="sxs-lookup"><span data-stu-id="bd33a-103">Update reviewSetQuery</span></span>

<span data-ttu-id="bd33a-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="bd33a-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd33a-105">Обнови свойства обзора [eDiscoverySetQuery.](../resources/ediscovery-reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="bd33a-105">Update the properties of an eDiscovery [reviewSetQuery](../resources/ediscovery-reviewsetquery.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bd33a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd33a-106">Permissions</span></span>

<span data-ttu-id="bd33a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd33a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd33a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd33a-109">Permission type</span></span>|<span data-ttu-id="bd33a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd33a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd33a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd33a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bd33a-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd33a-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="bd33a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd33a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd33a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd33a-114">Not supported.</span></span>|
|<span data-ttu-id="bd33a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd33a-115">Application</span></span>|<span data-ttu-id="bd33a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd33a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd33a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd33a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bd33a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd33a-118">Request headers</span></span>

| <span data-ttu-id="bd33a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bd33a-119">Name</span></span>       | <span data-ttu-id="bd33a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bd33a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bd33a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd33a-121">Authorization</span></span> | <span data-ttu-id="bd33a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd33a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd33a-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd33a-124">Request body</span></span>

<span data-ttu-id="bd33a-125">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="bd33a-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bd33a-126">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="bd33a-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bd33a-127">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="bd33a-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bd33a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd33a-128">Property</span></span>     | <span data-ttu-id="bd33a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bd33a-129">Type</span></span>        | <span data-ttu-id="bd33a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bd33a-130">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bd33a-131">displayName</span><span class="sxs-lookup"><span data-stu-id="bd33a-131">displayName</span></span> | <span data-ttu-id="bd33a-132">String</span><span class="sxs-lookup"><span data-stu-id="bd33a-132">String</span></span> | <span data-ttu-id="bd33a-133">Отображение имени для проверки набора запроса.</span><span class="sxs-lookup"><span data-stu-id="bd33a-133">Display name for they review set query.</span></span> |
| <span data-ttu-id="bd33a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd33a-134">query</span></span> | <span data-ttu-id="bd33a-135">String</span><span class="sxs-lookup"><span data-stu-id="bd33a-135">String</span></span> | <span data-ttu-id="bd33a-136">Строка запроса в запросе KQL (Язык запросов ключевых слов).</span><span class="sxs-lookup"><span data-stu-id="bd33a-136">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="bd33a-137">Подробные сведения см. [в поле метаданных документа.](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery)</span><span class="sxs-lookup"><span data-stu-id="bd33a-137">For details, see [Document metadata fields](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span></span> |

## <a name="response"></a><span data-ttu-id="bd33a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd33a-138">Response</span></span>

<span data-ttu-id="bd33a-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bd33a-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd33a-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="bd33a-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd33a-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd33a-142">Request</span></span>

<span data-ttu-id="bd33a-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd33a-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bd33a-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd33a-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_reviewsetquery"
}-->

```http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807
Content-type: application/json

{
  "displayName": "My Query 1 - Renamed"
}
```
# <a name="c"></a>[<span data-ttu-id="bd33a-145">C#</span><span class="sxs-lookup"><span data-stu-id="bd33a-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd33a-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd33a-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd33a-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd33a-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bd33a-148">Java</span><span class="sxs-lookup"><span data-stu-id="bd33a-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-reviewsetquery-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bd33a-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd33a-149">Response</span></span>

<span data-ttu-id="bd33a-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bd33a-150">The following is an example of the response.</span></span>

> <span data-ttu-id="bd33a-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bd33a-151">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.reviewSetQuery"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update reviewsetquery",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
