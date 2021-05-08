---
title: Список ресурсов updatableAssetGroup
description: Получите список объектов updatableAssetGroup и их свойств.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: d0529c59c00e84e122e5be3e5658c963535fd6d9
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239269"
---
# <a name="list-updatableassetgroup-resources"></a><span data-ttu-id="9a3ce-103">Список ресурсов updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="9a3ce-103">List updatableAssetGroup resources</span></span>
<span data-ttu-id="9a3ce-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="9a3ce-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a3ce-105">Получите список [объектов updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="9a3ce-105">Get a list of [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) objects and their properties.</span></span>

<span data-ttu-id="9a3ce-106">Эта операция фильтрует полностью квалифицированный тип ресурса, который наследуется от `microsoft.graph.windowsUpdates.updatableAssetGroup` [updatableAsset.](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="9a3ce-106">This operation filters on the fully qualified resource type, `microsoft.graph.windowsUpdates.updatableAssetGroup`, which inherits from [updatableAsset](../resources/windowsupdates-updatableasset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9a3ce-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a3ce-107">Permissions</span></span>
<span data-ttu-id="9a3ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a3ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a3ce-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a3ce-110">Permission type</span></span>|<span data-ttu-id="9a3ce-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a3ce-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a3ce-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a3ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9a3ce-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a3ce-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="9a3ce-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a3ce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a3ce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a3ce-115">Not supported.</span></span>|
|<span data-ttu-id="9a3ce-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a3ce-116">Application</span></span>|<span data-ttu-id="9a3ce-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a3ce-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a3ce-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a3ce-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/?$filter=isof('microsoft.graph.windowsUpdates.updatableAssetGroup')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9a3ce-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9a3ce-119">Optional query parameters</span></span>
<span data-ttu-id="9a3ce-120">Этот метод поддерживает некоторые параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$count` , , , , , и `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="9a3ce-120">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a3ce-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a3ce-121">Request headers</span></span>
|<span data-ttu-id="9a3ce-122">Имя</span><span class="sxs-lookup"><span data-stu-id="9a3ce-122">Name</span></span>|<span data-ttu-id="9a3ce-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9a3ce-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9a3ce-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a3ce-124">Authorization</span></span>|<span data-ttu-id="9a3ce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a3ce-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a3ce-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a3ce-127">Request body</span></span>
<span data-ttu-id="9a3ce-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9a3ce-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a3ce-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a3ce-129">Response</span></span>

<span data-ttu-id="9a3ce-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9a3ce-130">If successful, this method returns a `200 OK` response code and a collection of [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9a3ce-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="9a3ce-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9a3ce-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a3ce-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9a3ce-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a3ce-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_updatableassetgroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/?$filter=isof('microsoft.graph.windowsUpdates.updatableAssetGroup')
```
# <a name="c"></a>[<span data-ttu-id="9a3ce-134">C#</span><span class="sxs-lookup"><span data-stu-id="9a3ce-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-updatableassetgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a3ce-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a3ce-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-updatableassetgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a3ce-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a3ce-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-updatableassetgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a3ce-137">Java</span><span class="sxs-lookup"><span data-stu-id="9a3ce-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-updatableassetgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9a3ce-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a3ce-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.updatableAssetGroup)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
      "id": "5c55730b-730b-5c55-0b73-555c0b73555c"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
      "id": "deb43c16-77ff-465d-aa79-366a107a6c7a"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
      "id": "312643e6-b805-419f-bdf7-1a104dd6c8b9"
    }
  ]
}
```

