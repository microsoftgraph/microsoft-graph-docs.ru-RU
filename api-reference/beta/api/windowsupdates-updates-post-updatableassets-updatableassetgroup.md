---
title: Создание updatableAssetGroup
description: Создание нового объекта updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 4a7bb68439cd3fd2eade0eaf11b43e2bbf51a5b2
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52238448"
---
# <a name="create-updatableassetgroup"></a><span data-ttu-id="6eeb8-103">Создание updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="6eeb8-103">Create updatableAssetGroup</span></span>
<span data-ttu-id="6eeb8-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="6eeb8-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6eeb8-105">Создание нового [объекта updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="6eeb8-105">Create a new [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>

<span data-ttu-id="6eeb8-106">Ресурс **updatableAssetGroup** наследуется от [updatableAsset.](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="6eeb8-106">The **updatableAssetGroup** resource inherits from [updatableAsset](../resources/windowsupdates-updatableasset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6eeb8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6eeb8-107">Permissions</span></span>
<span data-ttu-id="6eeb8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6eeb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6eeb8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6eeb8-110">Permission type</span></span>|<span data-ttu-id="6eeb8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6eeb8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6eeb8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6eeb8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6eeb8-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6eeb8-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="6eeb8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6eeb8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6eeb8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6eeb8-115">Not supported.</span></span>|
|<span data-ttu-id="6eeb8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6eeb8-116">Application</span></span>|<span data-ttu-id="6eeb8-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6eeb8-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6eeb8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6eeb8-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets
```

## <a name="request-headers"></a><span data-ttu-id="6eeb8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6eeb8-119">Request headers</span></span>
|<span data-ttu-id="6eeb8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6eeb8-120">Name</span></span>|<span data-ttu-id="6eeb8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6eeb8-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6eeb8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6eeb8-122">Authorization</span></span>|<span data-ttu-id="6eeb8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6eeb8-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6eeb8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6eeb8-125">Content-Type</span></span>|<span data-ttu-id="6eeb8-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6eeb8-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6eeb8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6eeb8-128">Request body</span></span>
<span data-ttu-id="6eeb8-129">В теле запроса поставляем представление JSON объекта [updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="6eeb8-129">In the request body, supply a JSON representation of the [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>

<span data-ttu-id="6eeb8-130">Свойства не требуются.</span><span class="sxs-lookup"><span data-stu-id="6eeb8-130">No properties are required.</span></span>


## <a name="response"></a><span data-ttu-id="6eeb8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6eeb8-131">Response</span></span>

<span data-ttu-id="6eeb8-132">В случае успешной работы этот метод возвращает код ответа и объект `201 Created` [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6eeb8-132">If successful, this method returns a `201 Created` response code and an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6eeb8-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="6eeb8-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6eeb8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6eeb8-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6eeb8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6eeb8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_updatableassetgroup_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets
Content-Type: application/json
Content-length: 76

{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup"
}
```
# <a name="c"></a>[<span data-ttu-id="6eeb8-136">C#</span><span class="sxs-lookup"><span data-stu-id="6eeb8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-updatableassetgroup-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6eeb8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6eeb8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-updatableassetgroup-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6eeb8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6eeb8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-updatableassetgroup-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6eeb8-139">Java</span><span class="sxs-lookup"><span data-stu-id="6eeb8-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-updatableassetgroup-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6eeb8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="6eeb8-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAssetGroup"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
  "id": "5c55730b-730b-5c55-0b73-555c0b73555c"
}
```

