---
title: Создание тега
description: Создайте новый объект тегов.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 412a0cd1ae4f8c38466a6526a5c84eea670897bb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773762"
---
# <a name="create-tag"></a><span data-ttu-id="9015b-103">Создание тега</span><span class="sxs-lookup"><span data-stu-id="9015b-103">Create tag</span></span>

<span data-ttu-id="9015b-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="9015b-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9015b-105">Создайте новый тег для указанного случая.</span><span class="sxs-lookup"><span data-stu-id="9015b-105">Create a new tag for the specified case.</span></span>  <span data-ttu-id="9015b-106">Теги используются в наборах обзоров при просмотре контента.</span><span class="sxs-lookup"><span data-stu-id="9015b-106">The tags are used in review sets while reviewing content.</span></span>

## <a name="permissions"></a><span data-ttu-id="9015b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9015b-107">Permissions</span></span>

<span data-ttu-id="9015b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9015b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9015b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9015b-110">Permission type</span></span>|<span data-ttu-id="9015b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9015b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9015b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9015b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9015b-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9015b-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="9015b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9015b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9015b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9015b-115">Not supported.</span></span>|
|<span data-ttu-id="9015b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9015b-116">Application</span></span>|<span data-ttu-id="9015b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9015b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9015b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9015b-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/tags
```

## <a name="request-headers"></a><span data-ttu-id="9015b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9015b-119">Request headers</span></span>

|<span data-ttu-id="9015b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9015b-120">Name</span></span>|<span data-ttu-id="9015b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9015b-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9015b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9015b-122">Authorization</span></span>|<span data-ttu-id="9015b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9015b-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9015b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9015b-125">Content-Type</span></span>|<span data-ttu-id="9015b-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9015b-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9015b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9015b-128">Request body</span></span>

<span data-ttu-id="9015b-129">В теле запроса поставляем представление JSON объекта [тегов.](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="9015b-129">In the request body, supply a JSON representation of the [tag](../resources/ediscovery-tag.md) object.</span></span>

<span data-ttu-id="9015b-130">В следующей таблице показаны свойства, необходимые при создании [тега.](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="9015b-130">The following table shows the properties that are required when you create the [tag](../resources/ediscovery-tag.md).</span></span>

|<span data-ttu-id="9015b-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="9015b-131">Property</span></span>|<span data-ttu-id="9015b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="9015b-132">Type</span></span>|<span data-ttu-id="9015b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="9015b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9015b-134">childSelectability</span><span class="sxs-lookup"><span data-stu-id="9015b-134">childSelectability</span></span>|[<span data-ttu-id="9015b-135">microsoft.graph.ediscovery.childSelectability</span><span class="sxs-lookup"><span data-stu-id="9015b-135">microsoft.graph.ediscovery.childSelectability</span></span>](../resources/ediscovery-tag.md#childselectability-values)|<span data-ttu-id="9015b-136">Указывает, можно ли связывать один или несколько детских тегов с документом.</span><span class="sxs-lookup"><span data-stu-id="9015b-136">Indicates whether a single or multiple child tags can be associated with a document.</span></span> <span data-ttu-id="9015b-137">Возможные значения: `One`, `Many`.</span><span class="sxs-lookup"><span data-stu-id="9015b-137">Possible values are: `One`, `Many`.</span></span>  <span data-ttu-id="9015b-138">Это значение контролирует, представляет ли UX теги в качестве почтовых ящиков или группы кнопок радио.</span><span class="sxs-lookup"><span data-stu-id="9015b-138">This value controls whether the UX presents the tags as checkboxes or a radio button group.</span></span> <span data-ttu-id="9015b-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9015b-139">Required.</span></span>|
|<span data-ttu-id="9015b-140">displayName</span><span class="sxs-lookup"><span data-stu-id="9015b-140">displayName</span></span>|<span data-ttu-id="9015b-141">String</span><span class="sxs-lookup"><span data-stu-id="9015b-141">String</span></span>|<span data-ttu-id="9015b-142">Отображение имени тега.</span><span class="sxs-lookup"><span data-stu-id="9015b-142">Display name of the tag.</span></span> <span data-ttu-id="9015b-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9015b-143">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="9015b-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="9015b-144">Response</span></span>

<span data-ttu-id="9015b-145">В случае успешного решения этот метод возвращает код ответа и `201 Created` [объект microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9015b-145">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9015b-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="9015b-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9015b-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="9015b-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9015b-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="9015b-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tag_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags
Content-Type: application/json
Content-length: 235

{
  "displayName":"Privileged",
  "description":"The document is privileged",
  "parent@odata.bind":"https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/98fdad78bbce4519b75474bc150575c3"
}
```
# <a name="c"></a>[<span data-ttu-id="9015b-149">C#</span><span class="sxs-lookup"><span data-stu-id="9015b-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tag-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9015b-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9015b-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tag-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9015b-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9015b-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tag-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9015b-152">Java</span><span class="sxs-lookup"><span data-stu-id="9015b-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tag-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9015b-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="9015b-153">Response</span></span>

<span data-ttu-id="9015b-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9015b-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.tag"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/$entity",
    "displayName": "Privileged",
    "description": "The document is privileged",
    "lastModifiedDateTime": "2021-01-12T01:01:09.0419153Z",
    "childSelectability": "One",
    "id": "0825ef81ade74095a3b3154a3c434c3e",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": null,
            "userPrincipalName": "admin@contoso.com"
        }
    }
}
```
