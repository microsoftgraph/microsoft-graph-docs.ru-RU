---
title: 'driveItem: восстановление'
description: Восстановление driveItem, который был удален и в настоящее время находится в корзине.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
ms.date: 08/06/2019
doc_type: apiPageType
ms.openlocfilehash: fc1d9e1dc44af3ccbca132d8d54f1413e029f614
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046267"
---
# <a name="driveitem-restore"></a><span data-ttu-id="26d4d-103">driveItem: восстановление</span><span class="sxs-lookup"><span data-stu-id="26d4d-103">driveItem: restore</span></span>

<span data-ttu-id="26d4d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26d4d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26d4d-105">Восстановление [driveItem,](../resources/driveitem.md) который был удален и в настоящее время находится в корзине.</span><span class="sxs-lookup"><span data-stu-id="26d4d-105">Restore a [driveItem](../resources/driveitem.md) that has been deleted and is currently in the recycle bin.</span></span> <span data-ttu-id="26d4d-106">**ПРИМЕЧАНИЕ.** В настоящее время эта функция доступна только для OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="26d4d-106">**NOTE**: This functionality is currently only available for OneDrive Personal.</span></span>

## <a name="permissions"></a><span data-ttu-id="26d4d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26d4d-107">Permissions</span></span>

<span data-ttu-id="26d4d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26d4d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26d4d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26d4d-110">Permission type</span></span>                        | <span data-ttu-id="26d4d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26d4d-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="26d4d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26d4d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="26d4d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26d4d-113">Not supported.</span></span> |
| <span data-ttu-id="26d4d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26d4d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26d4d-115">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26d4d-115">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="26d4d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26d4d-116">Application</span></span>                            | <span data-ttu-id="26d4d-117">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26d4d-117">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="26d4d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26d4d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/drive/items/{item-id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="26d4d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26d4d-119">Request headers</span></span>

| <span data-ttu-id="26d4d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="26d4d-120">Name</span></span>          | <span data-ttu-id="26d4d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="26d4d-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="26d4d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="26d4d-122">Authorization</span></span> | <span data-ttu-id="26d4d-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="26d4d-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="26d4d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26d4d-124">Request body</span></span>

<span data-ttu-id="26d4d-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="26d4d-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="26d4d-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="26d4d-126">Parameter</span></span>     | <span data-ttu-id="26d4d-127">Тип</span><span class="sxs-lookup"><span data-stu-id="26d4d-127">Type</span></span>                                         | <span data-ttu-id="26d4d-128">Описание</span><span class="sxs-lookup"><span data-stu-id="26d4d-128">Description</span></span> |
|:--------------|:---------------------------------------------|:------------|
|<span data-ttu-id="26d4d-129">parentReference</span><span class="sxs-lookup"><span data-stu-id="26d4d-129">parentReference</span></span>|[<span data-ttu-id="26d4d-130">ItemReference</span><span class="sxs-lookup"><span data-stu-id="26d4d-130">ItemReference</span></span>](../resources/itemreference.md)| <span data-ttu-id="26d4d-131">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="26d4d-131">Optional.</span></span> <span data-ttu-id="26d4d-132">Ссылка на родительский элемент, в который будет восстановлен удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="26d4d-132">Reference to the parent item the deleted item will be restored to.</span></span> |
|<span data-ttu-id="26d4d-133">name</span><span class="sxs-lookup"><span data-stu-id="26d4d-133">name</span></span>           |<span data-ttu-id="26d4d-134">String</span><span class="sxs-lookup"><span data-stu-id="26d4d-134">String</span></span>                                        | <span data-ttu-id="26d4d-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="26d4d-135">Optional.</span></span> <span data-ttu-id="26d4d-136">Новое имя восстановленного элемента.</span><span class="sxs-lookup"><span data-stu-id="26d4d-136">The new name for the restored item.</span></span> <span data-ttu-id="26d4d-137">Если оно не предоставлено, будет использовано такое же имя, как в оригинале.</span><span class="sxs-lookup"><span data-stu-id="26d4d-137">If this isn't provided, the same name will be used as the original.</span></span> |

## <a name="response"></a><span data-ttu-id="26d4d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="26d4d-138">Response</span></span>

<span data-ttu-id="26d4d-139">В случае успешной работы этот метод возвращает код отклика и `200 OK` восстановленный [объект driveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="26d4d-139">If successful, this method returns `200 OK` response code and the restored [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26d4d-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="26d4d-140">Examples</span></span>

<span data-ttu-id="26d4d-141">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="26d4d-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="26d4d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="26d4d-142">Request</span></span>

<span data-ttu-id="26d4d-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26d4d-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="26d4d-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="26d4d-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="26d4d-145">C#</span><span class="sxs-lookup"><span data-stu-id="26d4d-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="26d4d-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26d4d-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="26d4d-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26d4d-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="26d4d-148">Java</span><span class="sxs-lookup"><span data-stu-id="26d4d-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/restore-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="26d4d-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="26d4d-149">Response</span></span>

<span data-ttu-id="26d4d-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="26d4d-150">The following is an example of the response.</span></span>

> <span data-ttu-id="26d4d-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="26d4d-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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


