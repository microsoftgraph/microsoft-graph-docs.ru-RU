---
author: JeremyKelley
title: Создание пакета
description: Создание пакета driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 21312f78257fbd3c7c371e3c22e1ee03905402c1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046274"
---
# <a name="create-bundle"></a><span data-ttu-id="461f0-103">Создание пакета</span><span class="sxs-lookup"><span data-stu-id="461f0-103">Create bundle</span></span>

<span data-ttu-id="461f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="461f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="461f0-105">Добавьте новый [пакет][] в диск пользователя.</span><span class="sxs-lookup"><span data-stu-id="461f0-105">Add a new [bundle][] to the user's drive.</span></span>

[bundle]: ../resources/bundle.md

## <a name="permissions"></a><span data-ttu-id="461f0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="461f0-107">Permissions</span></span>

<span data-ttu-id="461f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="461f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="461f0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="461f0-110">Permission type</span></span>      | <span data-ttu-id="461f0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="461f0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="461f0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="461f0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="461f0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="461f0-113">Not supported.</span></span>                             |
|<span data-ttu-id="461f0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="461f0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="461f0-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="461f0-115">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="461f0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="461f0-116">Application</span></span>          | <span data-ttu-id="461f0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="461f0-117">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="461f0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="461f0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drive/bundles
```

## <a name="request-headers"></a><span data-ttu-id="461f0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="461f0-119">Request headers</span></span>

| <span data-ttu-id="461f0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="461f0-120">Name</span></span>          | <span data-ttu-id="461f0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="461f0-121">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="461f0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="461f0-122">Authorization</span></span> | <span data-ttu-id="461f0-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="461f0-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="461f0-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="461f0-125">Request body</span></span>

<span data-ttu-id="461f0-126">В корпусе запроса поставляем представление JSON созданного пакета.</span><span class="sxs-lookup"><span data-stu-id="461f0-126">In the request body, supply a JSON representation of the bundle to be created.</span></span>

## <a name="response"></a><span data-ttu-id="461f0-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="461f0-127">Response</span></span>

<span data-ttu-id="461f0-128">Если запрос будет успешным, будет возвращен [driveItem,](../resources/driveitem.md) представляющий только что созданный пакет.</span><span class="sxs-lookup"><span data-stu-id="461f0-128">If the request is successful, the [driveItem](../resources/driveitem.md) representing the newly created bundle will be returned.</span></span>

<span data-ttu-id="461f0-129">Дополнительные сведения о возвращении ошибок см. в статье [Отклики с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="461f0-129">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="461f0-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="461f0-130">Examples</span></span>

### <a name="example-1-create-a-bundle"></a><span data-ttu-id="461f0-131">Пример 1. Создание пакета</span><span class="sxs-lookup"><span data-stu-id="461f0-131">Example 1: Create a bundle</span></span>

<span data-ttu-id="461f0-132">В следующем примере показано, как создать базовый новый пакет.</span><span class="sxs-lookup"><span data-stu-id="461f0-132">The following example shows how to create a basic new bundle.</span></span>
<span data-ttu-id="461f0-133">Этот запрос создаст новый пакет с именем и добавит в пакет два `Just some files` существующих элементов.</span><span class="sxs-lookup"><span data-stu-id="461f0-133">This request will create a new bundle named `Just some files` and add two existing items to the bundle.</span></span>
<span data-ttu-id="461f0-134">Этот пакет можно использовать для обмена файлами с другими пользователями, не делясь папкой, в которая хранятся эти элементы.</span><span class="sxs-lookup"><span data-stu-id="461f0-134">This bundle can be used to share a collection of files with other users without sharing the folder those items are stored in.</span></span>

#### <a name="request"></a><span data-ttu-id="461f0-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="461f0-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="461f0-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="461f0-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-bundle" } -->

```http
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
# <a name="c"></a>[<span data-ttu-id="461f0-137">C#</span><span class="sxs-lookup"><span data-stu-id="461f0-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="461f0-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="461f0-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="461f0-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="461f0-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="461f0-140">Java</span><span class="sxs-lookup"><span data-stu-id="461f0-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="461f0-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="461f0-141">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
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

<span data-ttu-id="461f0-142">Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="461f0-142">The response object shown here might be shortened for readability.</span></span>

### <a name="example-2-create-an-album"></a><span data-ttu-id="461f0-143">Пример 2. Создание альбома</span><span class="sxs-lookup"><span data-stu-id="461f0-143">Example 2: Create an album</span></span>

<span data-ttu-id="461f0-144">Запрос на создание нового фотоальбома схож, хотя в аспекте пакета свойство альбомов занигается до значения non-null.</span><span class="sxs-lookup"><span data-stu-id="461f0-144">The request to create a new photo album is similar, although inside the bundle facet, the album property is set to a non-null value.</span></span>

#### <a name="request"></a><span data-ttu-id="461f0-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="461f0-145">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="461f0-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="461f0-146">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-album" } -->

```http
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
# <a name="c"></a>[<span data-ttu-id="461f0-147">C#</span><span class="sxs-lookup"><span data-stu-id="461f0-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-album-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="461f0-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="461f0-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-album-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="461f0-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="461f0-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-album-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="461f0-150">Java</span><span class="sxs-lookup"><span data-stu-id="461f0-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-album-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="461f0-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="461f0-151">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
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

<span data-ttu-id="461f0-152">Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="461f0-152">The response object shown here might be shortened for readability.</span></span>

<span data-ttu-id="461f0-153">Если _@microsoft.graph.conflictBehavior_ будет переименован  и пакет с тем же именем уже существует, новое имя пакета будет обновлено, чтобы быть уникальным.</span><span class="sxs-lookup"><span data-stu-id="461f0-153">If _@microsoft.graph.conflictBehavior_ is set to **rename** and a bundle with the same name already exists, the new bundle name will be updated to be unique.</span></span>
<span data-ttu-id="461f0-154">OneDrive будет придать номер к концу имени пакета.</span><span class="sxs-lookup"><span data-stu-id="461f0-154">OneDrive will append a number to the end of the bundle name.</span></span>

<span data-ttu-id="461f0-155">Например, `My Day at the Beach` будет `My Day at the Beach 1` переименовано .</span><span class="sxs-lookup"><span data-stu-id="461f0-155">For example, `My Day at the Beach` would be renamed `My Day at the Beach 1`.</span></span>
<span data-ttu-id="461f0-156">Если будет принято, то номер будет приращен еще раз, пока не будет обнаружено уникальное `My Day at the Beach 1` имя пакета.</span><span class="sxs-lookup"><span data-stu-id="461f0-156">If `My Day at the Beach 1` is taken, then the number would be incremented again until a unique bundle name is discovered.</span></span>


[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Create a new bundle or photo album.",
  "keywords": "create,bundle",
  "section": "documentation",
  "tocPath&quot;: &quot;Bundles/Create"
} -->


