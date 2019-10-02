---
title: 'driveItem: восстановление'
description: Восстановление driveItem, который был удален и в данный момент находится в корзине.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
ms.date: 08/06/2019
doc_type: apiPageType
ms.openlocfilehash: f105ab748e6fff69f1138e4318ac66597a721391
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356298"
---
# <a name="driveitem-restore"></a><span data-ttu-id="adcfd-103">driveItem: восстановление</span><span class="sxs-lookup"><span data-stu-id="adcfd-103">driveItem: restore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adcfd-104">Восстановление [driveItem](../resources/driveitem.md) , который был удален и в данный момент находится в корзине.</span><span class="sxs-lookup"><span data-stu-id="adcfd-104">Restore a [driveItem](../resources/driveitem.md) that has been deleted and is currently in the recycle bin.</span></span> <span data-ttu-id="adcfd-105">**Примечание**: Эта функция в настоящее время доступна только для OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="adcfd-105">**NOTE**: This functionality is currently only available for OneDrive Personal.</span></span>

## <a name="permissions"></a><span data-ttu-id="adcfd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="adcfd-106">Permissions</span></span>

<span data-ttu-id="adcfd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adcfd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="adcfd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="adcfd-109">Permission type</span></span>                        | <span data-ttu-id="adcfd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="adcfd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="adcfd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="adcfd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="adcfd-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adcfd-112">Not supported.</span></span> |
| <span data-ttu-id="adcfd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="adcfd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adcfd-114">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adcfd-114">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="adcfd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="adcfd-115">Application</span></span>                            | <span data-ttu-id="adcfd-116">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adcfd-116">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="adcfd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="adcfd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/drive/items/{item-id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="adcfd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="adcfd-118">Request headers</span></span>

| <span data-ttu-id="adcfd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="adcfd-119">Name</span></span>          | <span data-ttu-id="adcfd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="adcfd-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="adcfd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="adcfd-121">Authorization</span></span> | <span data-ttu-id="adcfd-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="adcfd-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="adcfd-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="adcfd-123">Request body</span></span>

<span data-ttu-id="adcfd-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="adcfd-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="adcfd-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="adcfd-125">Parameter</span></span>     | <span data-ttu-id="adcfd-126">Тип</span><span class="sxs-lookup"><span data-stu-id="adcfd-126">Type</span></span>                                         | <span data-ttu-id="adcfd-127">Описание</span><span class="sxs-lookup"><span data-stu-id="adcfd-127">Description</span></span> |
|:--------------|:---------------------------------------------|:------------|
|<span data-ttu-id="adcfd-128">parentReference</span><span class="sxs-lookup"><span data-stu-id="adcfd-128">parentReference</span></span>|[<span data-ttu-id="adcfd-129">ItemReference</span><span class="sxs-lookup"><span data-stu-id="adcfd-129">ItemReference</span></span>](../resources/itemreference.md)| <span data-ttu-id="adcfd-130">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="adcfd-130">Optional.</span></span> <span data-ttu-id="adcfd-131">Ссылка на родительский элемент, на который будет восстановлен удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="adcfd-131">Reference to the parent item the deleted item will be restored to.</span></span> |
|<span data-ttu-id="adcfd-132">name</span><span class="sxs-lookup"><span data-stu-id="adcfd-132">name</span></span>           |<span data-ttu-id="adcfd-133">String</span><span class="sxs-lookup"><span data-stu-id="adcfd-133">String</span></span>                                        | <span data-ttu-id="adcfd-134">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="adcfd-134">Optional.</span></span> <span data-ttu-id="adcfd-135">Новое имя восстановленного элемента.</span><span class="sxs-lookup"><span data-stu-id="adcfd-135">The new name for the restored item.</span></span> <span data-ttu-id="adcfd-136">Если оно не предоставлено, будет использовано такое же имя, как в оригинале.</span><span class="sxs-lookup"><span data-stu-id="adcfd-136">If this isn't provided, the same name will be used as the original.</span></span> |

## <a name="response"></a><span data-ttu-id="adcfd-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="adcfd-137">Response</span></span>

<span data-ttu-id="adcfd-138">В случае успешного выполнения этот метод `200 OK` возвращает код отклика и восстановленный объект [driveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="adcfd-138">If successful, this method returns `200 OK` response code and the restored [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="adcfd-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="adcfd-139">Examples</span></span>

<span data-ttu-id="adcfd-140">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="adcfd-140">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="adcfd-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="adcfd-141">Request</span></span>

<span data-ttu-id="adcfd-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adcfd-142">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="adcfd-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="adcfd-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="adcfd-144">C#</span><span class="sxs-lookup"><span data-stu-id="adcfd-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/restore-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="adcfd-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adcfd-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/restore-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="adcfd-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adcfd-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/restore-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="adcfd-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="adcfd-147">Response</span></span>

<span data-ttu-id="adcfd-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="adcfd-148">The following is an example of the response.</span></span>

> <span data-ttu-id="adcfd-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="adcfd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
