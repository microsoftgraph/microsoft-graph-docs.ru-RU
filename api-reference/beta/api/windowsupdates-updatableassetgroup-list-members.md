---
title: Список updatable членов группы активов
description: Список участников ресурса updatableAssetGroup. Участники имеют тип azureADDevice.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 747bf224d4dfbddf0d7845e3ca6f4d23e48912d1
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52266694"
---
# <a name="list-updatable-asset-group-members"></a><span data-ttu-id="719d8-104">Список updatable членов группы активов</span><span class="sxs-lookup"><span data-stu-id="719d8-104">List updatable asset group members</span></span>
<span data-ttu-id="719d8-105">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="719d8-105">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="719d8-106">Список участников ресурса [updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="719d8-106">List the members of an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) resource.</span></span> <span data-ttu-id="719d8-107">Участники имеют тип [azureADDevice.](../resources/windowsupdates-azureaddevice.md)</span><span class="sxs-lookup"><span data-stu-id="719d8-107">Members are of the [azureADDevice](../resources/windowsupdates-azureaddevice.md) type.</span></span>

<span data-ttu-id="719d8-108">Эта операция ссылается на **свойство** навигации участников ресурса **updatableAssetGroup.**</span><span class="sxs-lookup"><span data-stu-id="719d8-108">This operation references the **members** navigation property of an **updatableAssetGroup** resource.</span></span> <span data-ttu-id="719d8-109">Чтобы ссылаться на свойство типа, полученное из [updatableAsset,](../resources/windowsupdates-updatableasset.md)включайте полный тип производных ресурсов в URL-адрес запроса, т.е. `.../microsoft.graph.windowsUpdates.updatableAssetGroup/members` .</span><span class="sxs-lookup"><span data-stu-id="719d8-109">To reference a property of a type derived from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full derived resource type in the query URL, i.e., `.../microsoft.graph.windowsUpdates.updatableAssetGroup/members`.</span></span>

## <a name="permissions"></a><span data-ttu-id="719d8-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="719d8-110">Permissions</span></span>
<span data-ttu-id="719d8-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="719d8-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="719d8-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="719d8-113">Permission type</span></span>|<span data-ttu-id="719d8-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="719d8-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="719d8-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="719d8-115">Delegated (work or school account)</span></span>|<span data-ttu-id="719d8-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="719d8-116">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="719d8-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="719d8-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="719d8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="719d8-118">Not supported.</span></span>|
|<span data-ttu-id="719d8-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="719d8-119">Application</span></span>|<span data-ttu-id="719d8-120">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="719d8-120">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="719d8-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="719d8-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/microsoft.graph.windowsUpdates.updatableAssetGroup/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="719d8-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="719d8-122">Optional query parameters</span></span>
<span data-ttu-id="719d8-123">Этот метод поддерживает некоторые параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$count` , , , , , и `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="719d8-123">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

<span data-ttu-id="719d8-124">Чтобы использовать параметр запроса для свойства, которое не унаследовано от [updatableAsset,](../resources/windowsupdates-updatableasset.md)включайте полный тип ресурса для свойства.</span><span class="sxs-lookup"><span data-stu-id="719d8-124">To use a query parameter on a property that is not inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md), include the full resource type for the property.</span></span> <span data-ttu-id="719d8-125">Например, чтобы применить `$select` к свойству **ошибок** [azureADDevice,](../resources/windowsupdates-azureaddevice.md)используйте `$select=microsoft.graph.windowsUpdates.azureADDevice/errors` .</span><span class="sxs-lookup"><span data-stu-id="719d8-125">For example, to apply `$select` on the **errors** property of [azureADDevice](../resources/windowsupdates-azureaddevice.md), use `$select=microsoft.graph.windowsUpdates.azureADDevice/errors`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="719d8-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="719d8-126">Request headers</span></span>
|<span data-ttu-id="719d8-127">Имя</span><span class="sxs-lookup"><span data-stu-id="719d8-127">Name</span></span>|<span data-ttu-id="719d8-128">Описание</span><span class="sxs-lookup"><span data-stu-id="719d8-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="719d8-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="719d8-129">Authorization</span></span>|<span data-ttu-id="719d8-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="719d8-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="719d8-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="719d8-132">Request body</span></span>
<span data-ttu-id="719d8-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="719d8-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="719d8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="719d8-134">Response</span></span>

<span data-ttu-id="719d8-135">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [updatableAsset](../resources/windowsupdates-updatableasset.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="719d8-135">If successful, this method returns a `200 OK` response code and a collection of [updatableAsset](../resources/windowsupdates-updatableasset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="719d8-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="719d8-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="719d8-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="719d8-137">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="719d8-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="719d8-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_updatableasset"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/microsoft.graph.windowsUpdates.updatableAssetGroup/members
```
# <a name="c"></a>[<span data-ttu-id="719d8-139">C#</span><span class="sxs-lookup"><span data-stu-id="719d8-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-updatableasset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="719d8-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="719d8-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-updatableasset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="719d8-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="719d8-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-updatableasset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="719d8-142">Java</span><span class="sxs-lookup"><span data-stu-id="719d8-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-updatableasset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="719d8-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="719d8-143">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.updatableAsset)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "f5ba7065-7065-f5ba-6570-baf56570baf5"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "6d49dfaf-9c24-42f7-9628-c136e35774c8"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "1f61492e-4e34-4dee-904a-0d38299e76b2"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "bfe3c2d1-4cef-4952-8c5e-30d56ccf0cdc"
    }
  ]
}
```

