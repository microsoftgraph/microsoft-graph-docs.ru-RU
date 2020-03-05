---
title: 'driveItem: восстановление'
description: Восстановление driveItem, который был удален и в данный момент находится в корзине.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
ms.date: 08/06/2019
doc_type: apiPageType
ms.openlocfilehash: b2dbdca5ff9ab0c55a721b0d47db174ed00bf8c5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432413"
---
# <a name="driveitem-restore"></a><span data-ttu-id="73244-103">driveItem: восстановление</span><span class="sxs-lookup"><span data-stu-id="73244-103">driveItem: restore</span></span>

<span data-ttu-id="73244-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="73244-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73244-105">Восстановление [driveItem](../resources/driveitem.md) , который был удален и в данный момент находится в корзине.</span><span class="sxs-lookup"><span data-stu-id="73244-105">Restore a [driveItem](../resources/driveitem.md) that has been deleted and is currently in the recycle bin.</span></span> <span data-ttu-id="73244-106">**Примечание**: Эта функция в настоящее время доступна только для OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="73244-106">**NOTE**: This functionality is currently only available for OneDrive Personal.</span></span>

## <a name="permissions"></a><span data-ttu-id="73244-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73244-107">Permissions</span></span>

<span data-ttu-id="73244-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73244-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73244-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73244-110">Permission type</span></span>                        | <span data-ttu-id="73244-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73244-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="73244-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73244-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="73244-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73244-113">Not supported.</span></span> |
| <span data-ttu-id="73244-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73244-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73244-115">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73244-115">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="73244-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73244-116">Application</span></span>                            | <span data-ttu-id="73244-117">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73244-117">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73244-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73244-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/drive/items/{item-id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="73244-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73244-119">Request headers</span></span>

| <span data-ttu-id="73244-120">Имя</span><span class="sxs-lookup"><span data-stu-id="73244-120">Name</span></span>          | <span data-ttu-id="73244-121">Описание</span><span class="sxs-lookup"><span data-stu-id="73244-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="73244-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="73244-122">Authorization</span></span> | <span data-ttu-id="73244-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="73244-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="73244-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73244-124">Request body</span></span>

<span data-ttu-id="73244-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="73244-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="73244-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="73244-126">Parameter</span></span>     | <span data-ttu-id="73244-127">Тип</span><span class="sxs-lookup"><span data-stu-id="73244-127">Type</span></span>                                         | <span data-ttu-id="73244-128">Описание</span><span class="sxs-lookup"><span data-stu-id="73244-128">Description</span></span> |
|:--------------|:---------------------------------------------|:------------|
|<span data-ttu-id="73244-129">parentReference</span><span class="sxs-lookup"><span data-stu-id="73244-129">parentReference</span></span>|[<span data-ttu-id="73244-130">ItemReference</span><span class="sxs-lookup"><span data-stu-id="73244-130">ItemReference</span></span>](../resources/itemreference.md)| <span data-ttu-id="73244-131">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="73244-131">Optional.</span></span> <span data-ttu-id="73244-132">Ссылка на родительский элемент, на который будет восстановлен удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="73244-132">Reference to the parent item the deleted item will be restored to.</span></span> |
|<span data-ttu-id="73244-133">name</span><span class="sxs-lookup"><span data-stu-id="73244-133">name</span></span>           |<span data-ttu-id="73244-134">String</span><span class="sxs-lookup"><span data-stu-id="73244-134">String</span></span>                                        | <span data-ttu-id="73244-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="73244-135">Optional.</span></span> <span data-ttu-id="73244-136">Новое имя восстановленного элемента.</span><span class="sxs-lookup"><span data-stu-id="73244-136">The new name for the restored item.</span></span> <span data-ttu-id="73244-137">Если оно не предоставлено, будет использовано такое же имя, как в оригинале.</span><span class="sxs-lookup"><span data-stu-id="73244-137">If this isn't provided, the same name will be used as the original.</span></span> |

## <a name="response"></a><span data-ttu-id="73244-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="73244-138">Response</span></span>

<span data-ttu-id="73244-139">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и восстановленный объект [driveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="73244-139">If successful, this method returns `200 OK` response code and the restored [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73244-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="73244-140">Examples</span></span>

<span data-ttu-id="73244-141">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="73244-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="73244-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="73244-142">Request</span></span>

<span data-ttu-id="73244-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73244-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="73244-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="73244-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "restore-item",
  "scopes": "files.readwrite",
  "target": "action"
}-->

```http
POST https://graph.microsoft.com/beta/me/drive/items/{item-id}/restore
Content-type: application/json

{
  "parentReference": {
    "id": "String",
  },
  "name": "String"
}
```
# <a name="c"></a>[<span data-ttu-id="73244-145">C#</span><span class="sxs-lookup"><span data-stu-id="73244-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73244-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73244-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73244-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73244-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="73244-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="73244-148">Response</span></span>

<span data-ttu-id="73244-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="73244-149">The following is an example of the response.</span></span>

> <span data-ttu-id="73244-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73244-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1312abc!1231",
  "name": "new-restored-item-name.txt",
  "size": 19121,
  "lastModifiedDateTime": "2017-12-12T10:40:59Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Restore a DriveItem.",
  "keywords": "retore,item,driveitem",
  "section": "documentation",
  "tocPath": "Items/Restore"
}-->
