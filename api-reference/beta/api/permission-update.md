---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Изменение разрешений на общий доступ
ms.openlocfilehash: 96662cac4a58dcff9ed7faa40f61c8a09bfc88b3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074588"
---
# <a name="update-sharing-permission"></a><span data-ttu-id="9d314-102">Изменение разрешений на общий доступ</span><span class="sxs-lookup"><span data-stu-id="9d314-102">Update sharing permission</span></span>

> <span data-ttu-id="9d314-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9d314-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d314-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d314-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9d314-105">В этой статье рассказывается, как обновить свойства разрешения на общий доступ путем обновления ресурса разрешения.</span><span class="sxs-lookup"><span data-stu-id="9d314-105">Update the properties of a sharing permission by patching the permission resource.</span></span>

<span data-ttu-id="9d314-106">Таким способом можно изменить только свойство **roles**.</span><span class="sxs-lookup"><span data-stu-id="9d314-106">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d314-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d314-107">Permissions</span></span>

<span data-ttu-id="9d314-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d314-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d314-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d314-110">Permission type</span></span>      | <span data-ttu-id="9d314-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d314-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d314-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d314-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9d314-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d314-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9d314-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d314-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d314-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d314-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="9d314-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d314-116">Application</span></span> | <span data-ttu-id="9d314-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d314-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d314-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d314-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="9d314-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d314-119">Optional request headers</span></span>

| <span data-ttu-id="9d314-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9d314-120">Name</span></span>          | <span data-ttu-id="9d314-121">Тип</span><span class="sxs-lookup"><span data-stu-id="9d314-121">Type</span></span>   | <span data-ttu-id="9d314-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9d314-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="9d314-123">if-match</span><span class="sxs-lookup"><span data-stu-id="9d314-123">if-match</span></span>      | <span data-ttu-id="9d314-124">string</span><span class="sxs-lookup"><span data-stu-id="9d314-124">string</span></span> | <span data-ttu-id="9d314-125">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="9d314-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d314-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d314-126">Request body</span></span>

<span data-ttu-id="9d314-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="9d314-127">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="9d314-128">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="9d314-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="9d314-129">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9d314-129">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9d314-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d314-130">Property</span></span>     | <span data-ttu-id="9d314-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9d314-131">Type</span></span>   | <span data-ttu-id="9d314-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9d314-132">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="9d314-133">**roles**</span><span class="sxs-lookup"><span data-stu-id="9d314-133">**roles**</span></span>    | <span data-ttu-id="9d314-134">String</span><span class="sxs-lookup"><span data-stu-id="9d314-134">String</span></span> | <span data-ttu-id="9d314-135">Массив типов разрешений.</span><span class="sxs-lookup"><span data-stu-id="9d314-135">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="9d314-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d314-136">Response</span></span>

<span data-ttu-id="9d314-137">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [permission](../resources/permission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9d314-137">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d314-138">Пример</span><span class="sxs-lookup"><span data-stu-id="9d314-138">Example</span></span>

<span data-ttu-id="9d314-139">Вот пример запроса, изменяющего роль в разрешении на общий доступ на роль "только чтение".</span><span class="sxs-lookup"><span data-stu-id="9d314-139">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>

<!-- {"blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite"} -->

```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```

### <a name="response"></a><span data-ttu-id="9d314-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d314-140">Response</span></span>

<span data-ttu-id="9d314-141">При успешном выполнении этот метод возвращает ресурс [Permission](../resources/permission.md), представляющий обновленное состояние разрешения, в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9d314-141">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
