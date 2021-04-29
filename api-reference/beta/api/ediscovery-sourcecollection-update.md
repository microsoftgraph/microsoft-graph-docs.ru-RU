---
title: Обновление sourceCollection
description: Обновление свойств объекта sourceCollection.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 482d60dcec4e6f169bbf6962b20deebfbc52f5d5
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080259"
---
# <a name="update-sourcecollection"></a><span data-ttu-id="4cbb3-103">Обновление sourceCollection</span><span class="sxs-lookup"><span data-stu-id="4cbb3-103">Update sourceCollection</span></span>

<span data-ttu-id="4cbb3-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="4cbb3-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cbb3-105">Обновление свойств объекта [sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="4cbb3-105">Update the properties of a [sourceCollection](../resources/ediscovery-sourcecollection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4cbb3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4cbb3-106">Permissions</span></span>

<span data-ttu-id="4cbb3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cbb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cbb3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cbb3-109">Permission type</span></span>|<span data-ttu-id="4cbb3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4cbb3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cbb3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cbb3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4cbb3-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cbb3-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="4cbb3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cbb3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cbb3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cbb3-114">Not supported.</span></span>|
|<span data-ttu-id="4cbb3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4cbb3-115">Application</span></span>|<span data-ttu-id="4cbb3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cbb3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cbb3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cbb3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}
```

## <a name="request-headers"></a><span data-ttu-id="4cbb3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4cbb3-118">Request headers</span></span>

|<span data-ttu-id="4cbb3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4cbb3-119">Name</span></span>|<span data-ttu-id="4cbb3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4cbb3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4cbb3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4cbb3-121">Authorization</span></span>|<span data-ttu-id="4cbb3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cbb3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4cbb3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4cbb3-124">Content-Type</span></span>|<span data-ttu-id="4cbb3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cbb3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cbb3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4cbb3-127">Request body</span></span>

<span data-ttu-id="4cbb3-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="4cbb3-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4cbb3-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="4cbb3-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4cbb3-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4cbb3-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="4cbb3-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="4cbb3-131">Property</span></span>|<span data-ttu-id="4cbb3-132">Тип</span><span class="sxs-lookup"><span data-stu-id="4cbb3-132">Type</span></span>|<span data-ttu-id="4cbb3-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4cbb3-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cbb3-134">contentQuery</span><span class="sxs-lookup"><span data-stu-id="4cbb3-134">contentQuery</span></span>|<span data-ttu-id="4cbb3-135">String</span><span class="sxs-lookup"><span data-stu-id="4cbb3-135">String</span></span>|<span data-ttu-id="4cbb3-136">Строка запроса в запросе KQL (Язык запросов ключевых слов).</span><span class="sxs-lookup"><span data-stu-id="4cbb3-136">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="4cbb3-137">Подробные сведения см. в [статье Ключевые запросы и условия поиска для поиска контента и поиска электронных данных.](/microsoft-365/compliance/keyword-queries-and-search-conditions)</span><span class="sxs-lookup"><span data-stu-id="4cbb3-137">For details, see [Keyword queries and search conditions for Content Search and eDiscovery](/microsoft-365/compliance/keyword-queries-and-search-conditions).</span></span>  <span data-ttu-id="4cbb3-138">Поиск можно уточнить с помощью полей в паре со значениями; например, `subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016` .</span><span class="sxs-lookup"><span data-stu-id="4cbb3-138">You can refine searches by using fields paired with values; for example, `subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016`.</span></span>|
|<span data-ttu-id="4cbb3-139">dataSourceScopes</span><span class="sxs-lookup"><span data-stu-id="4cbb3-139">dataSourceScopes</span></span>|<span data-ttu-id="4cbb3-140">microsoft.graph.ediscovery.dataSourceScopes</span><span class="sxs-lookup"><span data-stu-id="4cbb3-140">microsoft.graph.ediscovery.dataSourceScopes</span></span>|<span data-ttu-id="4cbb3-141">При указании коллекция будет охватывать всю службу для всей рабочей нагрузки.</span><span class="sxs-lookup"><span data-stu-id="4cbb3-141">When specified, the collection will span across a service for an entire workload.</span></span> <span data-ttu-id="4cbb3-142">Возможные значения: `none` `allTenantMailboxes` , , , `allTenantSites` `allCaseCustodians` `allCaseNoncustodialDataSources` .</span><span class="sxs-lookup"><span data-stu-id="4cbb3-142">Possible values are: `none`,`allTenantMailboxes`,`allTenantSites`,`allCaseCustodians`,`allCaseNoncustodialDataSources`.</span></span> <span data-ttu-id="4cbb3-143">**Примечание:** При создании коллекции исходных данных требуется один хранитель или указание данныхSourceScope.</span><span class="sxs-lookup"><span data-stu-id="4cbb3-143">**Note:** Either one custodian or specifying dataSourceScope is required when creating a source collection.</span></span>|
|<span data-ttu-id="4cbb3-144">description</span><span class="sxs-lookup"><span data-stu-id="4cbb3-144">description</span></span>|<span data-ttu-id="4cbb3-145">String</span><span class="sxs-lookup"><span data-stu-id="4cbb3-145">String</span></span>|<span data-ttu-id="4cbb3-146">Описание **sourceCollection**.</span><span class="sxs-lookup"><span data-stu-id="4cbb3-146">The description of the **sourceCollection**.</span></span>|
|<span data-ttu-id="4cbb3-147">displayName</span><span class="sxs-lookup"><span data-stu-id="4cbb3-147">displayName</span></span>|<span data-ttu-id="4cbb3-148">String</span><span class="sxs-lookup"><span data-stu-id="4cbb3-148">String</span></span>|<span data-ttu-id="4cbb3-149">Имя отображения **sourceCollection**.</span><span class="sxs-lookup"><span data-stu-id="4cbb3-149">The display name of the **sourceCollection**.</span></span>|

## <a name="response"></a><span data-ttu-id="4cbb3-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="4cbb3-150">Response</span></span>

<span data-ttu-id="4cbb3-151">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4cbb3-151">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4cbb3-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="4cbb3-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4cbb3-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cbb3-153">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4cbb3-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="4cbb3-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_sourcecollection"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/1a9b4145d8f84e39bc45a7f68c5c5119
Content-Type: application/json
Content-length: 247

{
    "displayName": "Quarterly Financials search",
}
```
# <a name="c"></a>[<span data-ttu-id="4cbb3-155">C#</span><span class="sxs-lookup"><span data-stu-id="4cbb3-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-sourcecollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4cbb3-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4cbb3-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-sourcecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4cbb3-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4cbb3-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-sourcecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4cbb3-158">Java</span><span class="sxs-lookup"><span data-stu-id="4cbb3-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-sourcecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4cbb3-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cbb3-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
