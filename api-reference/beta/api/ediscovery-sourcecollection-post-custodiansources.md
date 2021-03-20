---
title: Добавление custodianSources
description: Добавьте объекты custodial dataSource в исходный набор.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 5948452d33e84e40e338c12206202376745fffe5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952043"
---
# <a name="add-custodiansources"></a><span data-ttu-id="9ec13-103">Добавление custodianSources</span><span class="sxs-lookup"><span data-stu-id="9ec13-103">Add custodianSources</span></span>

<span data-ttu-id="9ec13-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="9ec13-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ec13-105">Добавьте [объекты dataSource хранителя](../resources/ediscovery-datasource.md) в исходный набор.</span><span class="sxs-lookup"><span data-stu-id="9ec13-105">Add custodian [dataSource](../resources/ediscovery-datasource.md) objects to a source collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ec13-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ec13-106">Permissions</span></span>

<span data-ttu-id="9ec13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ec13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ec13-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ec13-109">Permission type</span></span>|<span data-ttu-id="9ec13-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ec13-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ec13-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ec13-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9ec13-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ec13-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="9ec13-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ec13-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ec13-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ec13-114">Not supported.</span></span>|
|<span data-ttu-id="9ec13-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ec13-115">Application</span></span>|<span data-ttu-id="9ec13-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ec13-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ec13-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ec13-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/custodianSources/$ref
```

## <a name="request-headers"></a><span data-ttu-id="9ec13-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ec13-118">Request headers</span></span>

|<span data-ttu-id="9ec13-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9ec13-119">Name</span></span>|<span data-ttu-id="9ec13-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9ec13-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9ec13-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ec13-121">Authorization</span></span>|<span data-ttu-id="9ec13-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ec13-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9ec13-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9ec13-124">Content-Type</span></span>|<span data-ttu-id="9ec13-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ec13-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ec13-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ec13-127">Request body</span></span>

<span data-ttu-id="9ec13-128">В теле запроса поставляем представление JSON объекта [dataSource.](../resources/ediscovery-datasource.md)</span><span class="sxs-lookup"><span data-stu-id="9ec13-128">In the request body, supply a JSON representation of the [dataSource](../resources/ediscovery-datasource.md) object.</span></span>

<span data-ttu-id="9ec13-129">В следующей таблице показаны свойства, необходимые при создании [dataSource.](../resources/ediscovery-datasource.md)</span><span class="sxs-lookup"><span data-stu-id="9ec13-129">The following table shows the properties that are required when you create the [dataSource](../resources/ediscovery-datasource.md).</span></span>

|<span data-ttu-id="9ec13-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ec13-130">Property</span></span>|<span data-ttu-id="9ec13-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9ec13-131">Type</span></span>|<span data-ttu-id="9ec13-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9ec13-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ec13-133">@odata.id</span><span class="sxs-lookup"><span data-stu-id="9ec13-133">@odata.id</span></span>|<span data-ttu-id="9ec13-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9ec13-134">String</span></span>|<span data-ttu-id="9ec13-135">Строка, определяемая объектом custodial.</span><span class="sxs-lookup"><span data-stu-id="9ec13-135">String that defines the custodial object.</span></span> <span data-ttu-id="9ec13-136">См. пример, который следует.</span><span class="sxs-lookup"><span data-stu-id="9ec13-136">See the example that follows.</span></span>|

## <a name="response"></a><span data-ttu-id="9ec13-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ec13-137">Response</span></span>

<span data-ttu-id="9ec13-138">В случае успешной работы этот метод возвращает код ответа и `204 No Content` [объект microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9ec13-138">If successful, this method returns a `204 No Content` response code and a [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9ec13-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="9ec13-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9ec13-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ec13-140">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9ec13-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ec13-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_datasource_from__2"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections/1a9b4145d8f84e39bc45a7f68c5c5119/custodianSources/$ref
Content-Type: application/json
Content-length: 179

{
  "@odata.id":"https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/ab3a628a383045eba344b3caecba3104/userSources/31423539-3846-4333-4136-353644383531"
}
```
# <a name="c"></a>[<span data-ttu-id="9ec13-142">C#</span><span class="sxs-lookup"><span data-stu-id="9ec13-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-datasource-from--2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ec13-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ec13-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-datasource-from--2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ec13-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ec13-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-datasource-from--2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ec13-145">Java</span><span class="sxs-lookup"><span data-stu-id="9ec13-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-datasource-from--2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9ec13-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ec13-146">Response</span></span>

<span data-ttu-id="9ec13-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9ec13-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.dataSource"
}
-->

``` http
HTTP/1.1 204 No Content
Content-Type: application/json
```
