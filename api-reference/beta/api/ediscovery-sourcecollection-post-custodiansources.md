---
title: Добавление custodianSources
description: Добавьте объекты custodial dataSource в исходный набор.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: e044843992bff6f68d01c35a549a6a9b57a61417
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786007"
---
# <a name="add-custodiansources"></a><span data-ttu-id="81ae7-103">Добавление custodianSources</span><span class="sxs-lookup"><span data-stu-id="81ae7-103">Add custodianSources</span></span>

<span data-ttu-id="81ae7-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="81ae7-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81ae7-105">Добавьте [объекты dataSource хранителя](../resources/ediscovery-datasource.md) в исходный набор.</span><span class="sxs-lookup"><span data-stu-id="81ae7-105">Add custodian [dataSource](../resources/ediscovery-datasource.md) objects to a source collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="81ae7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81ae7-106">Permissions</span></span>

<span data-ttu-id="81ae7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81ae7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81ae7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81ae7-109">Permission type</span></span>|<span data-ttu-id="81ae7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81ae7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81ae7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81ae7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="81ae7-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81ae7-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="81ae7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81ae7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81ae7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81ae7-114">Not supported.</span></span>|
|<span data-ttu-id="81ae7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81ae7-115">Application</span></span>|<span data-ttu-id="81ae7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81ae7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81ae7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81ae7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/custodianSources/$ref
```

## <a name="request-headers"></a><span data-ttu-id="81ae7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81ae7-118">Request headers</span></span>

|<span data-ttu-id="81ae7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="81ae7-119">Name</span></span>|<span data-ttu-id="81ae7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="81ae7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="81ae7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81ae7-121">Authorization</span></span>|<span data-ttu-id="81ae7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81ae7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="81ae7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="81ae7-124">Content-Type</span></span>|<span data-ttu-id="81ae7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81ae7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81ae7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81ae7-127">Request body</span></span>

<span data-ttu-id="81ae7-128">В теле запроса поставляем представление JSON объекта [dataSource.](../resources/ediscovery-datasource.md)</span><span class="sxs-lookup"><span data-stu-id="81ae7-128">In the request body, supply a JSON representation of the [dataSource](../resources/ediscovery-datasource.md) object.</span></span>

<span data-ttu-id="81ae7-129">В следующей таблице показаны свойства, необходимые при создании [dataSource.](../resources/ediscovery-datasource.md)</span><span class="sxs-lookup"><span data-stu-id="81ae7-129">The following table shows the properties that are required when you create the [dataSource](../resources/ediscovery-datasource.md).</span></span>

|<span data-ttu-id="81ae7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="81ae7-130">Property</span></span>|<span data-ttu-id="81ae7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="81ae7-131">Type</span></span>|<span data-ttu-id="81ae7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="81ae7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81ae7-133">@odata.id</span><span class="sxs-lookup"><span data-stu-id="81ae7-133">@odata.id</span></span>|<span data-ttu-id="81ae7-134">String</span><span class="sxs-lookup"><span data-stu-id="81ae7-134">String</span></span>|<span data-ttu-id="81ae7-135">Строка, определяемая объектом custodial.</span><span class="sxs-lookup"><span data-stu-id="81ae7-135">String that defines the custodial object.</span></span> <span data-ttu-id="81ae7-136">См. пример, который следует.</span><span class="sxs-lookup"><span data-stu-id="81ae7-136">See the example that follows.</span></span>|

## <a name="response"></a><span data-ttu-id="81ae7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="81ae7-137">Response</span></span>

<span data-ttu-id="81ae7-138">В случае успешной работы этот метод возвращает код ответа и `204 No Content` [объект microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="81ae7-138">If successful, this method returns a `204 No Content` response code and a [microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81ae7-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="81ae7-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="81ae7-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="81ae7-140">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="81ae7-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="81ae7-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="81ae7-142">C#</span><span class="sxs-lookup"><span data-stu-id="81ae7-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-datasource-from--2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81ae7-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81ae7-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-datasource-from--2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81ae7-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81ae7-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-datasource-from--2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81ae7-145">Java</span><span class="sxs-lookup"><span data-stu-id="81ae7-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-datasource-from--2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="81ae7-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="81ae7-146">Response</span></span>

> <span data-ttu-id="81ae7-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="81ae7-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
}
-->

``` http
HTTP/1.1 204 No Content
```
