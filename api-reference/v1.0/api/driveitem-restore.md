---
title: 'driveItem: восстановление'
description: Восстановление driveItem, который был удален и в данный момент находится в корзине.
localization_priority: Normal
author: learafa
ms.prod: files
doc_type: apiPageType
ms.openlocfilehash: 4b7198543c97fdb59179a2898ddcc367feb6c19d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073259"
---
# <a name="driveitem-restore"></a><span data-ttu-id="912ad-103">driveItem: восстановление</span><span class="sxs-lookup"><span data-stu-id="912ad-103">driveItem: restore</span></span>

<span data-ttu-id="912ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="912ad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="912ad-105">Восстановление [driveItem](../resources/driveitem.md) , который был удален и в данный момент находится в корзине.</span><span class="sxs-lookup"><span data-stu-id="912ad-105">Restore a [driveItem](../resources/driveitem.md) that has been deleted and is currently in the recycle bin.</span></span> <span data-ttu-id="912ad-106">**Примечание**: Эта функция в настоящее время доступна только для OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="912ad-106">**NOTE**: This functionality is currently only available for OneDrive Personal.</span></span>

## <a name="permissions"></a><span data-ttu-id="912ad-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="912ad-107">Permissions</span></span>

<span data-ttu-id="912ad-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="912ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="912ad-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="912ad-110">Permission type</span></span>                        | <span data-ttu-id="912ad-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="912ad-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="912ad-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="912ad-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="912ad-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="912ad-113">Not supported.</span></span> |
| <span data-ttu-id="912ad-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="912ad-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="912ad-115">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="912ad-115">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="912ad-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="912ad-116">Application</span></span>                            | <span data-ttu-id="912ad-117">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="912ad-117">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="912ad-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="912ad-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/drive/items/{item-id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="912ad-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="912ad-119">Request headers</span></span>

| <span data-ttu-id="912ad-120">Имя</span><span class="sxs-lookup"><span data-stu-id="912ad-120">Name</span></span>          | <span data-ttu-id="912ad-121">Описание</span><span class="sxs-lookup"><span data-stu-id="912ad-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="912ad-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="912ad-122">Authorization</span></span> | <span data-ttu-id="912ad-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="912ad-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="912ad-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="912ad-125">Request body</span></span>

<span data-ttu-id="912ad-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="912ad-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="912ad-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="912ad-127">Parameter</span></span>     | <span data-ttu-id="912ad-128">Тип</span><span class="sxs-lookup"><span data-stu-id="912ad-128">Type</span></span>                                         | <span data-ttu-id="912ad-129">Описание</span><span class="sxs-lookup"><span data-stu-id="912ad-129">Description</span></span> |
|:--------------|:---------------------------------------------|:------------|
|<span data-ttu-id="912ad-130">parentReference</span><span class="sxs-lookup"><span data-stu-id="912ad-130">parentReference</span></span>|[<span data-ttu-id="912ad-131">ItemReference</span><span class="sxs-lookup"><span data-stu-id="912ad-131">ItemReference</span></span>](../resources/itemreference.md)| <span data-ttu-id="912ad-132">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="912ad-132">Optional.</span></span> <span data-ttu-id="912ad-133">Ссылка на родительский элемент, на который будет восстановлен удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="912ad-133">Reference to the parent item the deleted item will be restored to.</span></span> |
|<span data-ttu-id="912ad-134">name</span><span class="sxs-lookup"><span data-stu-id="912ad-134">name</span></span>           |<span data-ttu-id="912ad-135">String</span><span class="sxs-lookup"><span data-stu-id="912ad-135">String</span></span>                                        | <span data-ttu-id="912ad-136">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="912ad-136">Optional.</span></span> <span data-ttu-id="912ad-137">Новое имя восстановленного элемента.</span><span class="sxs-lookup"><span data-stu-id="912ad-137">The new name for the restored item.</span></span> <span data-ttu-id="912ad-138">Если оно не предоставлено, будет использовано такое же имя, как в оригинале.</span><span class="sxs-lookup"><span data-stu-id="912ad-138">If this isn't provided, the same name will be used as the original.</span></span> |

## <a name="response"></a><span data-ttu-id="912ad-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="912ad-139">Response</span></span>

<span data-ttu-id="912ad-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и восстановленный объект [driveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="912ad-140">If successful, this method returns a `200 OK` response code and the restored [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="912ad-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="912ad-141">Examples</span></span>

<span data-ttu-id="912ad-142">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="912ad-142">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="912ad-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="912ad-143">Request</span></span>

<span data-ttu-id="912ad-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="912ad-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="912ad-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="912ad-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="912ad-146">C#</span><span class="sxs-lookup"><span data-stu-id="912ad-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="912ad-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="912ad-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="912ad-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="912ad-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="912ad-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="912ad-149">Response</span></span>

<span data-ttu-id="912ad-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="912ad-150">The following is an example of the response.</span></span>

> <span data-ttu-id="912ad-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="912ad-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

