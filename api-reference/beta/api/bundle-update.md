---
author: JeremyKelley
ms.author: jeremyke
title: Обновление пакета
description: Обновление пакета элементов driveitem
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 18c04ff7760505901ded5adb6e291fadc7481b35
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441020"
---
# <a name="update-bundle"></a><span data-ttu-id="04126-103">Пакет обновления</span><span class="sxs-lookup"><span data-stu-id="04126-103">Update bundle</span></span>

<span data-ttu-id="04126-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="04126-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04126-105">Обновление метаданных для [пакета][] [элементов DRIVEITEM][driveItem] по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="04126-105">Update the metadata for a [bundle][] of [driveItems][driveItem] by ID.</span></span>
<span data-ttu-id="04126-106">Вы можете обновлять только следующие метаданные:</span><span class="sxs-lookup"><span data-stu-id="04126-106">You can only update the following metadata:</span></span>

* <span data-ttu-id="04126-107">Имя пакета</span><span class="sxs-lookup"><span data-stu-id="04126-107">Bundle name</span></span>
* <span data-ttu-id="04126-108">Альбом `coverImageItemId` (если требуется)</span><span class="sxs-lookup"><span data-stu-id="04126-108">Album `coverImageItemId` (if applicable)</span></span>

<span data-ttu-id="04126-109">Любые другие запросы на изменение будут игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="04126-109">Any other change requests will be ignored.</span></span>

## <a name="permissions"></a><span data-ttu-id="04126-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04126-110">Permissions</span></span>

<span data-ttu-id="04126-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04126-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04126-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04126-113">Permission type</span></span>      | <span data-ttu-id="04126-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04126-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04126-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04126-115">Delegated (work or school account)</span></span> | <span data-ttu-id="04126-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04126-116">Not supported.</span></span>                             |
|<span data-ttu-id="04126-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04126-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04126-118">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04126-118">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="04126-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04126-119">Application</span></span>          | <span data-ttu-id="04126-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04126-120">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="04126-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04126-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drive/items/{bundle-id}
```

## <a name="request-headers"></a><span data-ttu-id="04126-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04126-122">Request headers</span></span>

| <span data-ttu-id="04126-123">Имя</span><span class="sxs-lookup"><span data-stu-id="04126-123">Name</span></span>          | <span data-ttu-id="04126-124">Описание</span><span class="sxs-lookup"><span data-stu-id="04126-124">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="04126-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="04126-125">Authorization</span></span> | <span data-ttu-id="04126-126">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="04126-126">Bearer \{token\}.</span></span> <span data-ttu-id="04126-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04126-127">Required.</span></span> |
| <span data-ttu-id="04126-128">if-match</span><span class="sxs-lookup"><span data-stu-id="04126-128">if-match</span></span>      | <span data-ttu-id="04126-129">тегом.</span><span class="sxs-lookup"><span data-stu-id="04126-129">eTag.</span></span> <span data-ttu-id="04126-130">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="04126-130">Optional.</span></span> <span data-ttu-id="04126-131">Если указан заголовок запроса, а предоставленное значение eTag не совпадают с текущим тегом eTag в бункле, возвращается `412 Precondition Failed` ответ.</span><span class="sxs-lookup"><span data-stu-id="04126-131">If this request header is included and the eTag provided does not match the current eTag on the buncle, a `412 Precondition Failed` response is returned.</span></span>

## <a name="request-body"></a><span data-ttu-id="04126-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04126-132">Request body</span></span>

<span data-ttu-id="04126-133">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="04126-133">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="04126-134">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="04126-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="04126-135">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="04126-135">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="04126-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="04126-136">Response</span></span>

<span data-ttu-id="04126-137">В случае успешного выполнения этот метод возвращает ресурс [driveItem][] , представляющий обновленный пакет, в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04126-137">If successful, this method returns a [driveItem][] resource that represents the updated bundle in the response body.</span></span>

<span data-ttu-id="04126-138">Ознакомьтесь с разделом [ответы об ошибках][error-response] для получения дополнительных сведений об возвращении ошибок.</span><span class="sxs-lookup"><span data-stu-id="04126-138">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="04126-139">Пример</span><span class="sxs-lookup"><span data-stu-id="04126-139">Example</span></span>

<span data-ttu-id="04126-140">В этом примере переименовывается пакет.</span><span class="sxs-lookup"><span data-stu-id="04126-140">This example renames a bundle.</span></span>

### <a name="request"></a><span data-ttu-id="04126-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="04126-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="04126-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="04126-142">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "rename-bundle" } -->

```json
PATCH https://graph.microsoft.com/beta/drive/items/{bundle-id}
Content-Type: application/json

{
  "name": "Shared legal agreements"
}
```
# <a name="c"></a>[<span data-ttu-id="04126-143">C#</span><span class="sxs-lookup"><span data-stu-id="04126-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rename-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04126-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04126-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rename-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04126-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04126-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rename-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="04126-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="04126-146">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "Shared legal agreements",
  "bundle": {
    "childCount": 3
  }
}
```

<span data-ttu-id="04126-147">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="04126-147">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="04126-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04126-148">All the properties will be returned from an actual call.</span></span>


[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of a bundle.",
  "keywords": "update,replace,contents,bundle",
  "section": "documentation",
    "tocPath": "Bundles/Update"
} -->
