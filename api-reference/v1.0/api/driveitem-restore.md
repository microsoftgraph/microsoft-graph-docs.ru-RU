---
title: 'driveItem: восстановление'
description: Восстановление driveItem, который был удален и в настоящее время находится в корзине.
localization_priority: Normal
author: learafa
ms.prod: files
doc_type: apiPageType
ms.openlocfilehash: 391788bccc09876a1bed78da932dd574f1e23cfb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054051"
---
# <a name="driveitem-restore"></a><span data-ttu-id="dda64-103">driveItem: восстановление</span><span class="sxs-lookup"><span data-stu-id="dda64-103">driveItem: restore</span></span>

<span data-ttu-id="dda64-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dda64-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dda64-105">Восстановление [driveItem,](../resources/driveitem.md) который был удален и в настоящее время находится в корзине.</span><span class="sxs-lookup"><span data-stu-id="dda64-105">Restore a [driveItem](../resources/driveitem.md) that has been deleted and is currently in the recycle bin.</span></span> <span data-ttu-id="dda64-106">**ПРИМЕЧАНИЕ.** В настоящее время эта функция доступна только для OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="dda64-106">**NOTE**: This functionality is currently only available for OneDrive Personal.</span></span>

## <a name="permissions"></a><span data-ttu-id="dda64-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dda64-107">Permissions</span></span>

<span data-ttu-id="dda64-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dda64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dda64-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dda64-110">Permission type</span></span>                        | <span data-ttu-id="dda64-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dda64-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dda64-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dda64-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="dda64-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dda64-113">Not supported.</span></span> |
| <span data-ttu-id="dda64-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dda64-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dda64-115">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dda64-115">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="dda64-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="dda64-116">Application</span></span>                            | <span data-ttu-id="dda64-117">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dda64-117">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dda64-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dda64-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/drive/items/{item-id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="dda64-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dda64-119">Request headers</span></span>

| <span data-ttu-id="dda64-120">Имя</span><span class="sxs-lookup"><span data-stu-id="dda64-120">Name</span></span>          | <span data-ttu-id="dda64-121">Описание</span><span class="sxs-lookup"><span data-stu-id="dda64-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="dda64-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dda64-122">Authorization</span></span> | <span data-ttu-id="dda64-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dda64-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dda64-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dda64-125">Request body</span></span>

<span data-ttu-id="dda64-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="dda64-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dda64-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="dda64-127">Parameter</span></span>     | <span data-ttu-id="dda64-128">Тип</span><span class="sxs-lookup"><span data-stu-id="dda64-128">Type</span></span>                                         | <span data-ttu-id="dda64-129">Описание</span><span class="sxs-lookup"><span data-stu-id="dda64-129">Description</span></span> |
|:--------------|:---------------------------------------------|:------------|
|<span data-ttu-id="dda64-130">parentReference</span><span class="sxs-lookup"><span data-stu-id="dda64-130">parentReference</span></span>|[<span data-ttu-id="dda64-131">ItemReference</span><span class="sxs-lookup"><span data-stu-id="dda64-131">ItemReference</span></span>](../resources/itemreference.md)| <span data-ttu-id="dda64-132">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="dda64-132">Optional.</span></span> <span data-ttu-id="dda64-133">Ссылка на родительский элемент, в который будет восстановлен удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="dda64-133">Reference to the parent item the deleted item will be restored to.</span></span> |
|<span data-ttu-id="dda64-134">name</span><span class="sxs-lookup"><span data-stu-id="dda64-134">name</span></span>           |<span data-ttu-id="dda64-135">String</span><span class="sxs-lookup"><span data-stu-id="dda64-135">String</span></span>                                        | <span data-ttu-id="dda64-136">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="dda64-136">Optional.</span></span> <span data-ttu-id="dda64-137">Новое имя восстановленного элемента.</span><span class="sxs-lookup"><span data-stu-id="dda64-137">The new name for the restored item.</span></span> <span data-ttu-id="dda64-138">Если оно не предоставлено, будет использовано такое же имя, как в оригинале.</span><span class="sxs-lookup"><span data-stu-id="dda64-138">If this isn't provided, the same name will be used as the original.</span></span> |

## <a name="response"></a><span data-ttu-id="dda64-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="dda64-139">Response</span></span>

<span data-ttu-id="dda64-140">В случае успешной работы этот метод возвращает код отклика и `200 OK` восстановленный [объект driveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dda64-140">If successful, this method returns a `200 OK` response code and the restored [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dda64-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="dda64-141">Examples</span></span>

<span data-ttu-id="dda64-142">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="dda64-142">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="dda64-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="dda64-143">Request</span></span>

<span data-ttu-id="dda64-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dda64-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dda64-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="dda64-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dda64-146">C#</span><span class="sxs-lookup"><span data-stu-id="dda64-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dda64-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dda64-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dda64-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dda64-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dda64-149">Java</span><span class="sxs-lookup"><span data-stu-id="dda64-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/restore-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dda64-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="dda64-150">Response</span></span>

<span data-ttu-id="dda64-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dda64-151">The following is an example of the response.</span></span>

> <span data-ttu-id="dda64-152">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dda64-152">**Note:** The response object shown here might be shortened for readability.</span></span>

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

