---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Изменение разрешений на общий доступ
localization_priority: Normal
ms.openlocfilehash: b2c3c41c9feecf7b2874ffdcc468593b6eeb7444
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482072"
---
# <a name="update-sharing-permission"></a><span data-ttu-id="99d74-102">Обновление разрешения на общий доступ</span><span class="sxs-lookup"><span data-stu-id="99d74-102">Update sharing permission</span></span>

<span data-ttu-id="99d74-103">В этой статье рассказывается, как обновить свойства разрешения на общий доступ путем обновления ресурса разрешения.</span><span class="sxs-lookup"><span data-stu-id="99d74-103">Update the properties of a sharing permission by patching the permission resource.</span></span>

<span data-ttu-id="99d74-104">Таким способом можно изменить только свойство **roles**.</span><span class="sxs-lookup"><span data-stu-id="99d74-104">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="99d74-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99d74-105">Permissions</span></span>

<span data-ttu-id="99d74-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99d74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99d74-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99d74-108">Permission type</span></span>      | <span data-ttu-id="99d74-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99d74-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99d74-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99d74-110">Delegated (work or school account)</span></span> | <span data-ttu-id="99d74-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99d74-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="99d74-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99d74-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99d74-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99d74-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="99d74-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99d74-114">Application</span></span> | <span data-ttu-id="99d74-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99d74-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="99d74-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99d74-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="99d74-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99d74-117">Optional request headers</span></span>

| <span data-ttu-id="99d74-118">Имя</span><span class="sxs-lookup"><span data-stu-id="99d74-118">Name</span></span>          | <span data-ttu-id="99d74-119">Тип</span><span class="sxs-lookup"><span data-stu-id="99d74-119">Type</span></span>   | <span data-ttu-id="99d74-120">Описание</span><span class="sxs-lookup"><span data-stu-id="99d74-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="99d74-121">if-match</span><span class="sxs-lookup"><span data-stu-id="99d74-121">if-match</span></span>      | <span data-ttu-id="99d74-122">string</span><span class="sxs-lookup"><span data-stu-id="99d74-122">string</span></span> | <span data-ttu-id="99d74-123">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="99d74-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99d74-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99d74-124">Request body</span></span>

<span data-ttu-id="99d74-125">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="99d74-125">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="99d74-126">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="99d74-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="99d74-127">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="99d74-127">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="99d74-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="99d74-128">Property</span></span> | <span data-ttu-id="99d74-129">Тип</span><span class="sxs-lookup"><span data-stu-id="99d74-129">Type</span></span>              | <span data-ttu-id="99d74-130">Описание</span><span class="sxs-lookup"><span data-stu-id="99d74-130">Description</span></span>                   |
|:---------|:------------------|:------------------------------|
| <span data-ttu-id="99d74-131">roles</span><span class="sxs-lookup"><span data-stu-id="99d74-131">roles</span></span>    | <span data-ttu-id="99d74-132">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="99d74-132">String collection</span></span> | <span data-ttu-id="99d74-133">Массив типов разрешений.</span><span class="sxs-lookup"><span data-stu-id="99d74-133">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="99d74-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="99d74-134">Response</span></span>

<span data-ttu-id="99d74-135">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [permission](../resources/permission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="99d74-135">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99d74-136">Пример</span><span class="sxs-lookup"><span data-stu-id="99d74-136">Example</span></span>

<span data-ttu-id="99d74-137">Вот пример запроса, изменяющего роль в разрешении на общий доступ на роль "только чтение".</span><span class="sxs-lookup"><span data-stu-id="99d74-137">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>

<!-- { "blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```

### <a name="response"></a><span data-ttu-id="99d74-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="99d74-138">Response</span></span>

<span data-ttu-id="99d74-139">При успешном выполнении этот метод возвращает ресурс [Permission](../resources/permission.md), представляющий обновленное состояние разрешения, в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="99d74-139">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "read" ]
}
```

## <a name="error-responses"></a><span data-ttu-id="99d74-140">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="99d74-140">Error responses</span></span>

<span data-ttu-id="99d74-141">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="99d74-141">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "Sharing/Update permission"
} -->
