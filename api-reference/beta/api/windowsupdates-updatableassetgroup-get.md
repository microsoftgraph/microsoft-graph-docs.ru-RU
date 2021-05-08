---
title: Get updatableAssetGroup
description: Ознакомьтесь с свойствами и отношениями объекта updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 96019f9fac94e79e51963ce98a878799b58d918e
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52238953"
---
# <a name="get-updatableassetgroup"></a><span data-ttu-id="3add9-103">Get updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="3add9-103">Get updatableAssetGroup</span></span>
<span data-ttu-id="3add9-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="3add9-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3add9-105">Ознакомьтесь с свойствами и отношениями объекта [updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="3add9-105">Read the properties and relationships of an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3add9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3add9-106">Permissions</span></span>
<span data-ttu-id="3add9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3add9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3add9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3add9-109">Permission type</span></span>|<span data-ttu-id="3add9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3add9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3add9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3add9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3add9-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3add9-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="3add9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3add9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3add9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3add9-114">Not supported.</span></span>|
|<span data-ttu-id="3add9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3add9-115">Application</span></span>|<span data-ttu-id="3add9-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3add9-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3add9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3add9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/updatableAssets/{updatableAssetGroupId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3add9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3add9-118">Optional query parameters</span></span>
<span data-ttu-id="3add9-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3add9-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3add9-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3add9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3add9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3add9-121">Request headers</span></span>
|<span data-ttu-id="3add9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="3add9-122">Name</span></span>|<span data-ttu-id="3add9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3add9-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3add9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3add9-124">Authorization</span></span>|<span data-ttu-id="3add9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3add9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3add9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3add9-127">Request body</span></span>
<span data-ttu-id="3add9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3add9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3add9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3add9-129">Response</span></span>

<span data-ttu-id="3add9-130">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3add9-130">If successful, this method returns a `200 OK` response code and an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3add9-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="3add9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3add9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3add9-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3add9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3add9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_updatableassetgroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/5c55730b-730b-5c55-0b73-555c0b73555c
```
# <a name="c"></a>[<span data-ttu-id="3add9-134">C#</span><span class="sxs-lookup"><span data-stu-id="3add9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-updatableassetgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3add9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3add9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-updatableassetgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3add9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3add9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-updatableassetgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3add9-137">Java</span><span class="sxs-lookup"><span data-stu-id="3add9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-updatableassetgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="3add9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3add9-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAssetGroup"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
    "id": "5c55730b-730b-5c55-0b73-555c0b73555c"
  }
}
```

