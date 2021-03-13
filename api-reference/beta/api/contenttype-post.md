---
author: swapnil1993
title: Создание contentType
description: Создание типа контента на сайте.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: b9ab72a2d757e2d409f98c2aab4e6f7392769dfc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770474"
---
# <a name="create-contenttype"></a><span data-ttu-id="75cce-103">Создание contentType</span><span class="sxs-lookup"><span data-stu-id="75cce-103">Create contentType</span></span>
<span data-ttu-id="75cce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75cce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75cce-105">Создание нового [contentType][] на [сайте.][]</span><span class="sxs-lookup"><span data-stu-id="75cce-105">Create a new [contentType][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="75cce-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75cce-106">Permissions</span></span>

<span data-ttu-id="75cce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75cce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75cce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75cce-109">Permission type</span></span>      | <span data-ttu-id="75cce-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75cce-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75cce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75cce-111">Delegated (work or school account)</span></span> | <span data-ttu-id="75cce-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="75cce-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="75cce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75cce-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="75cce-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="75cce-114">Not Supported</span></span>    |
|<span data-ttu-id="75cce-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75cce-115">Application</span></span> | <span data-ttu-id="75cce-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="75cce-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="75cce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75cce-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/contentTypes

```

## <a name="request-headers"></a><span data-ttu-id="75cce-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75cce-118">Request headers</span></span>
|<span data-ttu-id="75cce-119">Имя</span><span class="sxs-lookup"><span data-stu-id="75cce-119">Name</span></span>|<span data-ttu-id="75cce-120">Описание</span><span class="sxs-lookup"><span data-stu-id="75cce-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="75cce-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75cce-121">Authorization</span></span>|<span data-ttu-id="75cce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75cce-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="75cce-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="75cce-124">Content-Type</span></span>|<span data-ttu-id="75cce-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75cce-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75cce-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75cce-127">Request body</span></span>

<span data-ttu-id="75cce-128">В теле запроса поставляем представление JSON для создания [ресурса contentType.][]</span><span class="sxs-lookup"><span data-stu-id="75cce-128">In the request body, supply a JSON representation of the [contentType][] resource to create.</span></span>

## <a name="response"></a><span data-ttu-id="75cce-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="75cce-129">Response</span></span>

<span data-ttu-id="75cce-130">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект contentType][] в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="75cce-130">If successful, this method returns a `201 Created` response code and a [contentType][] object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="75cce-131">Пример</span><span class="sxs-lookup"><span data-stu-id="75cce-131">Example</span></span>

<span data-ttu-id="75cce-132">В следующем примере показано, как создать новый тип общего контента.</span><span class="sxs-lookup"><span data-stu-id="75cce-132">The following example shows how to create a new generic content type.</span></span>

### <a name="request"></a><span data-ttu-id="75cce-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="75cce-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="75cce-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="75cce-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contenttype"
}
-->

```http
POST https://graph.microsoft.com/beta/sites/{id}/contentTypes
Content-Type: application/json

{
    "name": "docSet",
    "description": "custom docset",
    "parentReference": {
        name: "Document Set",
        id: "0x0120D520"
    },
    "group": "Document Set Content Types" 
}
```
# <a name="javascript"></a>[<span data-ttu-id="75cce-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75cce-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="75cce-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="75cce-136">Response</span></span>
><span data-ttu-id="75cce-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="75cce-137">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType"
}
-->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "0x01002A2479FF33DD4BC3B1533A012B653717",
  "name": "docSet",
  "group":"Document Set Content Types",
  "description" : "custom docset",
  "base": {
        "name": "Document Set",
        "id": "0x0120D520"
   }
}
```


[contentType]: ../resources/contentType.md
[site]: ../resources/site.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a Content type in a site",
  "keywords": "content type",
  "section": "documentation",
  "tocPath": "sites/Create ContentType",
  "suppressions": [
  ]
}
-->
