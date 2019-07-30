---
author: JeremyKelley
ms.author: jeremyke
title: Обновление пакета
description: Обновление пакета элементов driveitem
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bbeb9f62a0053a4735358097e2441bac08078ef7
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932886"
---
# <a name="update-bundle"></a><span data-ttu-id="195d4-103">Пакет обновления</span><span class="sxs-lookup"><span data-stu-id="195d4-103">Update bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="195d4-104">Обновление метаданных для [пакета][] [элементов DRIVEITEM][driveItem] по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="195d4-104">Update the metadata for a [bundle][] of [driveItems][driveItem] by ID.</span></span>
<span data-ttu-id="195d4-105">Вы можете обновлять только следующие метаданные:</span><span class="sxs-lookup"><span data-stu-id="195d4-105">You can only update the following metadata:</span></span>

* <span data-ttu-id="195d4-106">Имя пакета</span><span class="sxs-lookup"><span data-stu-id="195d4-106">Bundle name</span></span>
* <span data-ttu-id="195d4-107">Альбом `coverImageItemId` (если требуется)</span><span class="sxs-lookup"><span data-stu-id="195d4-107">Album `coverImageItemId` (if applicable)</span></span>

<span data-ttu-id="195d4-108">Любые другие запросы на изменение будут игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="195d4-108">Any other change requests will be ignored.</span></span>

## <a name="permissions"></a><span data-ttu-id="195d4-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="195d4-109">Permissions</span></span>

<span data-ttu-id="195d4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="195d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="195d4-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="195d4-112">Permission type</span></span>      | <span data-ttu-id="195d4-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="195d4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="195d4-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="195d4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="195d4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="195d4-115">Not supported.</span></span>                             |
|<span data-ttu-id="195d4-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="195d4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="195d4-117">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="195d4-117">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="195d4-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="195d4-118">Application</span></span>          | <span data-ttu-id="195d4-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="195d4-119">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="195d4-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="195d4-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drive/items/{bundle-id}
```

## <a name="request-headers"></a><span data-ttu-id="195d4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="195d4-121">Request headers</span></span>

| <span data-ttu-id="195d4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="195d4-122">Name</span></span>          | <span data-ttu-id="195d4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="195d4-123">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="195d4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="195d4-124">Authorization</span></span> | <span data-ttu-id="195d4-125">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="195d4-125">Bearer \{token\}.</span></span> <span data-ttu-id="195d4-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="195d4-126">Required.</span></span> |
| <span data-ttu-id="195d4-127">if-match</span><span class="sxs-lookup"><span data-stu-id="195d4-127">if-match</span></span>      | <span data-ttu-id="195d4-128">тегом.</span><span class="sxs-lookup"><span data-stu-id="195d4-128">eTag.</span></span> <span data-ttu-id="195d4-129">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="195d4-129">Optional.</span></span> <span data-ttu-id="195d4-130">Если указан заголовок запроса, а предоставленное значение eTag не совпадают с текущим тегом eTag в бункле, возвращается `412 Precondition Failed` ответ.</span><span class="sxs-lookup"><span data-stu-id="195d4-130">If this request header is included and the eTag provided does not match the current eTag on the buncle, a `412 Precondition Failed` response is returned.</span></span>

## <a name="request-body"></a><span data-ttu-id="195d4-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="195d4-131">Request body</span></span>

<span data-ttu-id="195d4-132">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="195d4-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="195d4-133">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="195d4-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="195d4-134">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="195d4-134">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="195d4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="195d4-135">Response</span></span>

<span data-ttu-id="195d4-136">В случае успешного выполнения этот метод возвращает ресурс [driveItem][] , представляющий обновленный пакет, в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="195d4-136">If successful, this method returns a [driveItem][] resource that represents the updated bundle in the response body.</span></span>

<span data-ttu-id="195d4-137">Ознакомьтесь с разделом [ответы об ошибках][error-response] для получения дополнительных сведений об возвращении ошибок.</span><span class="sxs-lookup"><span data-stu-id="195d4-137">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="195d4-138">Пример</span><span class="sxs-lookup"><span data-stu-id="195d4-138">Example</span></span>

<span data-ttu-id="195d4-139">В этом примере переименовывается пакет.</span><span class="sxs-lookup"><span data-stu-id="195d4-139">This example renames a bundle.</span></span>

### <a name="request"></a><span data-ttu-id="195d4-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="195d4-140">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="195d4-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="195d4-141">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "rename-bundle" } -->

```json
PATCH https://graph.microsoft.com/beta/drive/items/{bundle-id}
Content-Type: application/json

{
  "name": "Shared legal agreements"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="195d4-142">C#</span><span class="sxs-lookup"><span data-stu-id="195d4-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rename-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="195d4-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="195d4-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rename-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="195d4-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="195d4-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rename-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="195d4-145">Java</span><span class="sxs-lookup"><span data-stu-id="195d4-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rename-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="195d4-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="195d4-146">Response</span></span>

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

<span data-ttu-id="195d4-147">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="195d4-147">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="195d4-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="195d4-148">All the properties will be returned from an actual call.</span></span>


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
