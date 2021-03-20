---
title: Создание dataSource
description: Добавление дополнительных источников данных в исходный набор.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 3038f657930bcc92360bf5a60b68db4d6a8398a6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952078"
---
# <a name="create-datasource"></a><span data-ttu-id="7622f-103">Создание dataSource</span><span class="sxs-lookup"><span data-stu-id="7622f-103">Create dataSource</span></span>

<span data-ttu-id="7622f-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="7622f-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7622f-105">Добавление дополнительных источников данных в исходный набор.</span><span class="sxs-lookup"><span data-stu-id="7622f-105">Add additional data sources to a source collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="7622f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7622f-106">Permissions</span></span>

<span data-ttu-id="7622f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7622f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7622f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7622f-109">Permission type</span></span>|<span data-ttu-id="7622f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7622f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7622f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7622f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7622f-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7622f-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="7622f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7622f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7622f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7622f-114">Not supported.</span></span>|
|<span data-ttu-id="7622f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7622f-115">Application</span></span>|<span data-ttu-id="7622f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7622f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7622f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7622f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
```

## <a name="request-headers"></a><span data-ttu-id="7622f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7622f-118">Request headers</span></span>

|<span data-ttu-id="7622f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7622f-119">Name</span></span>|<span data-ttu-id="7622f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7622f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7622f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7622f-121">Authorization</span></span>|<span data-ttu-id="7622f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7622f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7622f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7622f-124">Content-Type</span></span>|<span data-ttu-id="7622f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7622f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7622f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7622f-127">Request body</span></span>

<span data-ttu-id="7622f-128">В теле запроса поставляем представление JSON объекта [dataSource.](../resources/ediscovery-datasource.md)</span><span class="sxs-lookup"><span data-stu-id="7622f-128">In the request body, supply a JSON representation of the [dataSource](../resources/ediscovery-datasource.md) object.</span></span>

<span data-ttu-id="7622f-129">В следующей таблице показаны свойства, необходимые при создании [dataSource.](../resources/ediscovery-datasource.md)</span><span class="sxs-lookup"><span data-stu-id="7622f-129">The following table shows the properties that are required when you create the [dataSource](../resources/ediscovery-datasource.md).</span></span>

|<span data-ttu-id="7622f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7622f-130">Property</span></span>|<span data-ttu-id="7622f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7622f-131">Type</span></span>|<span data-ttu-id="7622f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7622f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7622f-133">id</span><span class="sxs-lookup"><span data-stu-id="7622f-133">id</span></span>|<span data-ttu-id="7622f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7622f-134">String</span></span>|<span data-ttu-id="7622f-135">ID для [случая sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="7622f-135">The ID for [sourceCollection](../resources/ediscovery-sourcecollection.md) case.</span></span> <span data-ttu-id="7622f-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7622f-136">Read-only.</span></span> <span data-ttu-id="7622f-137">Унаследованный от [сущности](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="7622f-137">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="7622f-138">displayName</span><span class="sxs-lookup"><span data-stu-id="7622f-138">displayName</span></span>|<span data-ttu-id="7622f-139">Строка</span><span class="sxs-lookup"><span data-stu-id="7622f-139">String</span></span>|<span data-ttu-id="7622f-140">Имя [источникаCollection](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="7622f-140">The name of the [sourceCollection](../resources/ediscovery-sourcecollection.md)</span></span>|
|<span data-ttu-id="7622f-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7622f-141">createdDateTime</span></span>|<span data-ttu-id="7622f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7622f-142">DateTimeOffset</span></span>|<span data-ttu-id="7622f-143">Дата и время создания [sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="7622f-143">The date and time when the [sourceCollection](../resources/ediscovery-sourcecollection.md) was created.</span></span>|
|<span data-ttu-id="7622f-144">createdBy</span><span class="sxs-lookup"><span data-stu-id="7622f-144">createdBy</span></span>|[<span data-ttu-id="7622f-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="7622f-145">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="7622f-146">Пользователь, создавший [sourceCollection.](../resources/ediscovery-sourcecollection.md)</span><span class="sxs-lookup"><span data-stu-id="7622f-146">The user who created the [sourceCollection](../resources/ediscovery-sourcecollection.md).</span></span>|

## <a name="response"></a><span data-ttu-id="7622f-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="7622f-147">Response</span></span>

<span data-ttu-id="7622f-148">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7622f-148">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7622f-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="7622f-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7622f-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="7622f-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7622f-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="7622f-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_datasource_from__1"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources
Content-Type: application/json
Content-length: 179

{
    "@odata.type": "#microsoft.graph.ediscovery.userSource",
    "email": "badguy@contoso.com"
}
```
# <a name="c"></a>[<span data-ttu-id="7622f-152">C#</span><span class="sxs-lookup"><span data-stu-id="7622f-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-datasource-from--1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7622f-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7622f-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-datasource-from--1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7622f-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7622f-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-datasource-from--1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7622f-155">Java</span><span class="sxs-lookup"><span data-stu-id="7622f-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-datasource-from--1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7622f-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="7622f-156">Response</span></span>

<span data-ttu-id="7622f-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7622f-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.dataSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.ediscovery.dataSource",
  "id": "0fb67fc5-7fc5-0fb6-c57f-b60fc57fb60f",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```
