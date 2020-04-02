---
author: JeremyKelley
ms.author: jeremyke
title: Создание пакета
description: Создание пакета элементов driveitem
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 58ac2e4d0e6cc4a4f587aec082b59fe4ab633037
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107271"
---
# <a name="create-bundle"></a><span data-ttu-id="a00f3-103">Создание пакета</span><span class="sxs-lookup"><span data-stu-id="a00f3-103">Create bundle</span></span>

<span data-ttu-id="a00f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a00f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a00f3-105">Добавление нового [пакета][] на диск пользователя.</span><span class="sxs-lookup"><span data-stu-id="a00f3-105">Add a new [bundle][] to the user's drive.</span></span>

[bundle]: ../resources/bundle.md

## <a name="permissions"></a><span data-ttu-id="a00f3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a00f3-107">Permissions</span></span>

<span data-ttu-id="a00f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a00f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a00f3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a00f3-110">Permission type</span></span>      | <span data-ttu-id="a00f3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a00f3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a00f3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a00f3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a00f3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a00f3-113">Not supported.</span></span>                             |
|<span data-ttu-id="a00f3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a00f3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a00f3-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a00f3-115">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="a00f3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a00f3-116">Application</span></span>          | <span data-ttu-id="a00f3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a00f3-117">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="a00f3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a00f3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drive/bundles
```

## <a name="request-headers"></a><span data-ttu-id="a00f3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a00f3-119">Request headers</span></span>

| <span data-ttu-id="a00f3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a00f3-120">Name</span></span>          | <span data-ttu-id="a00f3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a00f3-121">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="a00f3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a00f3-122">Authorization</span></span> | <span data-ttu-id="a00f3-123">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="a00f3-123">Bearer \{token\}.</span></span> <span data-ttu-id="a00f3-124">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="a00f3-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a00f3-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a00f3-125">Request body</span></span>

<span data-ttu-id="a00f3-126">В тексте запроса добавьте представление создаваемого набора в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a00f3-126">In the request body, supply a JSON representation of the bundle to be created.</span></span>

## <a name="response"></a><span data-ttu-id="a00f3-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a00f3-127">Response</span></span>

<span data-ttu-id="a00f3-128">Если запрос выполнен успешно, будет возвращен [driveItem](../resources/driveitem.md) , представляющий созданный пакет.</span><span class="sxs-lookup"><span data-stu-id="a00f3-128">If the request is successful, the [driveItem](../resources/driveitem.md) representing the newly created bundle will be returned.</span></span>

<span data-ttu-id="a00f3-129">Ознакомьтесь с разделом [ответы об ошибках][error-response] для получения дополнительных сведений об возвращении ошибок.</span><span class="sxs-lookup"><span data-stu-id="a00f3-129">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="a00f3-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="a00f3-130">Examples</span></span>

### <a name="example-1-create-a-bundle"></a><span data-ttu-id="a00f3-131">Пример 1: создание пакета</span><span class="sxs-lookup"><span data-stu-id="a00f3-131">Example 1: Create a bundle</span></span>

<span data-ttu-id="a00f3-132">В приведенном ниже примере показано, как создать базовый пакет.</span><span class="sxs-lookup"><span data-stu-id="a00f3-132">The following example shows how to create a basic new bundle.</span></span>
<span data-ttu-id="a00f3-133">Этот запрос создаст новый пакет с именем `Just some files` и добавит в пакет два существующих элемента.</span><span class="sxs-lookup"><span data-stu-id="a00f3-133">This request will create a new bundle named `Just some files` and add two existing items to the bundle.</span></span>
<span data-ttu-id="a00f3-134">Этот пакет можно использовать для совместного использования коллекции файлов с другими пользователями без предоставления общего доступа к папке, в которой хранятся эти элементы.</span><span class="sxs-lookup"><span data-stu-id="a00f3-134">This bundle can be used to share a collection of files with other users without sharing the folder those items are stored in.</span></span>

#### <a name="request"></a><span data-ttu-id="a00f3-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="a00f3-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a00f3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="a00f3-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-bundle" } -->

```json
POST https://graph.microsoft.com/beta/drive/bundles
Content-Type: application/json

{
  "name": "Just some files",
  "@microsoft.graph.conflictBehavior" : "rename",
  "bundle": { },
  "children": [
    { "id": "1234asdf" },
    { "id": "1234qwerty" }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="a00f3-137">C#</span><span class="sxs-lookup"><span data-stu-id="a00f3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a00f3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a00f3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a00f3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a00f3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a00f3-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a00f3-140">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "1234321!abc",
  "name": "Just some files",
  "bundle": {
    "childCount": 2
  }
}
```

<span data-ttu-id="a00f3-141">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a00f3-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a00f3-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a00f3-142">All the properties will be returned from an actual call.</span></span>

### <a name="example-2-create-an-album"></a><span data-ttu-id="a00f3-143">Пример 2: Создание альбома</span><span class="sxs-lookup"><span data-stu-id="a00f3-143">Example 2: Create an album</span></span>

<span data-ttu-id="a00f3-144">Запрос на создание нового фотоальбома похож на то, что в аспекте пакета свойство альбома устанавливается в значение, отличное от NULL.</span><span class="sxs-lookup"><span data-stu-id="a00f3-144">The request to create a new photo album is similar, although inside the bundle facet, the album property is set to a non-null value.</span></span>

#### <a name="request"></a><span data-ttu-id="a00f3-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="a00f3-145">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a00f3-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="a00f3-146">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-album" } -->

```json
POST https://graph.microsoft.com/beta/drive/bundles
Content-Type: application/json

{
  "name": "My Day at the Beach",
  "@microsoft.graph.conflictBehavior" : "rename",
  "bundle": { "album": {} },
  "children": [
    { "id": "1234asdf" }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="a00f3-147">C#</span><span class="sxs-lookup"><span data-stu-id="a00f3-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-album-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a00f3-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a00f3-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-album-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a00f3-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a00f3-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-album-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a00f3-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="a00f3-150">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "1234321!abc",
  "name": "Just some files",
  "bundle": {
    "childCount": 2,
    "album": { }
 }
}
```

<span data-ttu-id="a00f3-151">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a00f3-151">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a00f3-152">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a00f3-152">All the properties will be returned from an actual call.</span></span>

<span data-ttu-id="a00f3-153">Если для _@microsoft. Graph. conflictBehavior_ задано **Переименование** , а пакет с таким именем уже существует, то новое имя пакета будет обновляться как уникальное.</span><span class="sxs-lookup"><span data-stu-id="a00f3-153">If _@microsoft.graph.conflictBehavior_ is set to **rename** and a bundle with the same name already exists, the new bundle name will be updated to be unique.</span></span>
<span data-ttu-id="a00f3-154">OneDrive добавит номер в конец имени пакета.</span><span class="sxs-lookup"><span data-stu-id="a00f3-154">OneDrive will append a number to the end of the bundle name.</span></span>

<span data-ttu-id="a00f3-155">Например, `My Day at the Beach` будет переименован `My Day at the Beach 1`.</span><span class="sxs-lookup"><span data-stu-id="a00f3-155">For example, `My Day at the Beach` would be renamed `My Day at the Beach 1`.</span></span>
<span data-ttu-id="a00f3-156">Если `My Day at the Beach 1` используется, то номер будет увеличен повторно до тех пор, пока не будет обнаружено уникальное имя пакета.</span><span class="sxs-lookup"><span data-stu-id="a00f3-156">If `My Day at the Beach 1` is taken, then the number would be incremented again until a unique bundle name is discovered.</span></span>


[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Create a new bundle or photo album.",
  "keywords": "create,bundle",
  "section": "documentation",
  "tocPath": "Bundles/Create"
} -->
