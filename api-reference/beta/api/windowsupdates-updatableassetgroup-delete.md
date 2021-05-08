---
title: Удаление updatableAssetGroup
description: Удаление объекта updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 1410314bfe4f3de461deb0a1da9f76330833096c
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239341"
---
# <a name="delete-updatableassetgroup"></a><span data-ttu-id="eaa14-103">Удаление updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="eaa14-103">Delete updatableAssetGroup</span></span>
<span data-ttu-id="eaa14-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="eaa14-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eaa14-105">Удаление [объекта updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="eaa14-105">Delete an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>

<span data-ttu-id="eaa14-106">Если объект [updatableAssetGroup,](../resources/windowsupdates-updatableassetgroup.md) его [объекты updatableAsset](../resources/windowsupdates-updatableasset.md) не удаляются.</span><span class="sxs-lookup"><span data-stu-id="eaa14-106">When an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object, its member [updatableAsset](../resources/windowsupdates-updatableasset.md) objects are not deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="eaa14-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eaa14-107">Permissions</span></span>
<span data-ttu-id="eaa14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaa14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaa14-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eaa14-110">Permission type</span></span>|<span data-ttu-id="eaa14-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eaa14-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eaa14-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eaa14-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eaa14-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaa14-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="eaa14-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eaa14-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eaa14-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaa14-115">Not supported.</span></span>|
|<span data-ttu-id="eaa14-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eaa14-116">Application</span></span>|<span data-ttu-id="eaa14-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaa14-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eaa14-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eaa14-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /admin/windows/updates/updatableAssets/{updatableAssetGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="eaa14-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eaa14-119">Request headers</span></span>
|<span data-ttu-id="eaa14-120">Имя</span><span class="sxs-lookup"><span data-stu-id="eaa14-120">Name</span></span>|<span data-ttu-id="eaa14-121">Описание</span><span class="sxs-lookup"><span data-stu-id="eaa14-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eaa14-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eaa14-122">Authorization</span></span>|<span data-ttu-id="eaa14-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eaa14-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eaa14-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eaa14-125">Request body</span></span>
<span data-ttu-id="eaa14-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eaa14-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eaa14-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="eaa14-127">Response</span></span>

<span data-ttu-id="eaa14-p103">При успешном выполнении этот метод возвращает код отклика `202 Accepted`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eaa14-p103">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eaa14-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="eaa14-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eaa14-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="eaa14-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="eaa14-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="eaa14-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_updatableassetgroup"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}
```
# <a name="c"></a>[<span data-ttu-id="eaa14-133">C#</span><span class="sxs-lookup"><span data-stu-id="eaa14-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-updatableassetgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eaa14-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eaa14-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-updatableassetgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eaa14-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eaa14-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-updatableassetgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eaa14-136">Java</span><span class="sxs-lookup"><span data-stu-id="eaa14-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-updatableassetgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="eaa14-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="eaa14-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

