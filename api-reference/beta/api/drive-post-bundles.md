---
author: JeremyKelley
ms.author: jeremyke
title: Создание пакета
description: Создание пакета элементов driveitem
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: a43c04aa0710007afdab9788c41df98903011532
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321094"
---
# <a name="create-bundle"></a><span data-ttu-id="6efd6-103">Создание пакета</span><span class="sxs-lookup"><span data-stu-id="6efd6-103">Create bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6efd6-104">Добавление нового [пакета][] на диск пользователя.</span><span class="sxs-lookup"><span data-stu-id="6efd6-104">Add a new [bundle][] to the user's drive.</span></span>

[bundle]: ../resources/bundle.md

## <a name="permissions"></a><span data-ttu-id="6efd6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6efd6-106">Permissions</span></span>

<span data-ttu-id="6efd6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6efd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6efd6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6efd6-109">Permission type</span></span>      | <span data-ttu-id="6efd6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6efd6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6efd6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6efd6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6efd6-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6efd6-112">Not supported.</span></span>                             |
|<span data-ttu-id="6efd6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6efd6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6efd6-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6efd6-114">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="6efd6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6efd6-115">Application</span></span>          | <span data-ttu-id="6efd6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6efd6-116">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="6efd6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6efd6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drive/bundles
```

## <a name="request-headers"></a><span data-ttu-id="6efd6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6efd6-118">Request headers</span></span>

| <span data-ttu-id="6efd6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6efd6-119">Name</span></span>          | <span data-ttu-id="6efd6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6efd6-120">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="6efd6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6efd6-121">Authorization</span></span> | <span data-ttu-id="6efd6-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="6efd6-122">Bearer \{token\}.</span></span> <span data-ttu-id="6efd6-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="6efd6-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6efd6-124">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="6efd6-124">Request body</span></span>

<span data-ttu-id="6efd6-125">В тексте запроса добавьте представление создаваемого набора в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6efd6-125">In the request body, supply a JSON representation of the bundle to be created.</span></span>

## <a name="response"></a><span data-ttu-id="6efd6-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="6efd6-126">Response</span></span>

<span data-ttu-id="6efd6-127">Если запрос выполнен успешно, будет возвращен [driveItem](../resources/driveitem.md) , представляющий созданный пакет.</span><span class="sxs-lookup"><span data-stu-id="6efd6-127">If the request is successful, the [driveItem](../resources/driveitem.md) representing the newly created bundle will be returned.</span></span>

<span data-ttu-id="6efd6-128">Ознакомьтесь с разделом [ответы об ошибках][error-response] для получения дополнительных сведений об возвращении ошибок.</span><span class="sxs-lookup"><span data-stu-id="6efd6-128">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="6efd6-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="6efd6-129">Examples</span></span>

### <a name="example-1-create-a-bundle"></a><span data-ttu-id="6efd6-130">Пример 1: создание пакета</span><span class="sxs-lookup"><span data-stu-id="6efd6-130">Example 1: Create a bundle</span></span>

<span data-ttu-id="6efd6-131">В приведенном ниже примере показано, как создать базовый пакет.</span><span class="sxs-lookup"><span data-stu-id="6efd6-131">The following example shows how to create a basic new bundle.</span></span>
<span data-ttu-id="6efd6-132">Этот запрос создаст новый пакет с именем `Just some files` и добавит в пакет два существующих элемента.</span><span class="sxs-lookup"><span data-stu-id="6efd6-132">This request will create a new bundle named `Just some files` and add two existing items to the bundle.</span></span>
<span data-ttu-id="6efd6-133">Этот пакет можно использовать для совместного использования коллекции файлов с другими пользователями без предоставления общего доступа к папке, в которой хранятся эти элементы.</span><span class="sxs-lookup"><span data-stu-id="6efd6-133">This bundle can be used to share a collection of files with other users without sharing the folder those items are stored in.</span></span>

#### <a name="request"></a><span data-ttu-id="6efd6-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6efd6-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6efd6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6efd6-135">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-bundle" } -->

```json
POST https://graph.microsoft.com/beta/drive/bundles
Content-Type: application/json

{
  "name": "Just some files",
  "@name.conflictBehavior" : "rename",
  "bundle": { },
  "children": [
    { "id": "1234asdf" },
    { "id": "1234qwerty" }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6efd6-136">C#</span><span class="sxs-lookup"><span data-stu-id="6efd6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6efd6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6efd6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6efd6-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6efd6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6efd6-139">Java</span><span class="sxs-lookup"><span data-stu-id="6efd6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6efd6-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6efd6-140">Response</span></span>

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

<span data-ttu-id="6efd6-141">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6efd6-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6efd6-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6efd6-142">All the properties will be returned from an actual call.</span></span>

### <a name="example-2-create-an-album"></a><span data-ttu-id="6efd6-143">Пример 2: Создание альбома</span><span class="sxs-lookup"><span data-stu-id="6efd6-143">Example 2: Create an album</span></span>

<span data-ttu-id="6efd6-144">Запрос на создание нового фотоальбома похож на то, что в аспекте пакета свойство альбома устанавливается в значение, отличное от NULL.</span><span class="sxs-lookup"><span data-stu-id="6efd6-144">The request to create a new photo album is similar, although inside the bundle facet, the album property is set to a non-null value.</span></span>

#### <a name="request"></a><span data-ttu-id="6efd6-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="6efd6-145">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6efd6-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="6efd6-146">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-album" } -->

```json
POST https://graph.microsoft.com/beta/drive/bundles
Content-Type: application/json

{
  "name": "My Day at the Beach",
  "@name.conflictBehavior" : "rename",
  "bundle": { "album": {} },
  "children": [
    { "id": "1234asdf" }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6efd6-147">C#</span><span class="sxs-lookup"><span data-stu-id="6efd6-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-album-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6efd6-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6efd6-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-album-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6efd6-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6efd6-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-album-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6efd6-150">Java</span><span class="sxs-lookup"><span data-stu-id="6efd6-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-album-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6efd6-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="6efd6-151">Response</span></span>

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

<span data-ttu-id="6efd6-152">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6efd6-152">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6efd6-153">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6efd6-153">All the properties will be returned from an actual call.</span></span>

<span data-ttu-id="6efd6-154">Если для _@microsoft. Graph. conflictBehavior_ задано \*\*\*\* переименование, а пакет с таким именем уже существует, то новое имя пакета будет обновляться как уникальное.</span><span class="sxs-lookup"><span data-stu-id="6efd6-154">If _@microsoft.graph.conflictBehavior_ is set to **rename** and a bundle with the same name already exists, the new bundle name will be updated to be unique.</span></span>
<span data-ttu-id="6efd6-155">OneDrive добавит номер в конец имени пакета.</span><span class="sxs-lookup"><span data-stu-id="6efd6-155">OneDrive will append a number to the end of the bundle name.</span></span>

<span data-ttu-id="6efd6-156">Например, `My Day at the Beach` будет переименован `My Day at the Beach 1`.</span><span class="sxs-lookup"><span data-stu-id="6efd6-156">For example, `My Day at the Beach` would be renamed `My Day at the Beach 1`.</span></span>
<span data-ttu-id="6efd6-157">Если `My Day at the Beach 1` используется, то номер будет увеличен повторно до тех пор, пока не будет обнаружено уникальное имя пакета.</span><span class="sxs-lookup"><span data-stu-id="6efd6-157">If `My Day at the Beach 1` is taken, then the number would be incremented again until a unique bundle name is discovered.</span></span>


[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Create a new bundle or photo album.",
  "keywords": "create,bundle",
  "section": "documentation",
  "tocPath": "Bundles/Create"
} -->
