---
title: 'updatableAssetGroup: removeMembersById'
description: Удалите членов одного типа из updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: dde1a86c363a2c8b7fe3492316bdcf5fc3593f26
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239046"
---
# <a name="updatableassetgroup-removemembersbyid"></a><span data-ttu-id="82f6d-103">updatableAssetGroup: removeMembersById</span><span class="sxs-lookup"><span data-stu-id="82f6d-103">updatableAssetGroup: removeMembersById</span></span>
<span data-ttu-id="82f6d-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="82f6d-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82f6d-105">Удалите членов одного типа из [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span><span class="sxs-lookup"><span data-stu-id="82f6d-105">Remove members of the same type from an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="82f6d-106">Вы также можете использовать метод [removeMembers для](windowsupdates-updatableassetgroup-removemembers.md) удаления участников.</span><span class="sxs-lookup"><span data-stu-id="82f6d-106">You can also use the method [removeMembers](windowsupdates-updatableassetgroup-removemembers.md) to remove members.</span></span>

## <a name="permissions"></a><span data-ttu-id="82f6d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82f6d-107">Permissions</span></span>
<span data-ttu-id="82f6d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82f6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82f6d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82f6d-110">Permission type</span></span>|<span data-ttu-id="82f6d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82f6d-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82f6d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82f6d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82f6d-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82f6d-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="82f6d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82f6d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82f6d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82f6d-115">Not supported.</span></span>|
|<span data-ttu-id="82f6d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82f6d-116">Application</span></span>|<span data-ttu-id="82f6d-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82f6d-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82f6d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82f6d-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/removeMembersById
```

## <a name="request-headers"></a><span data-ttu-id="82f6d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82f6d-119">Request headers</span></span>
|<span data-ttu-id="82f6d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="82f6d-120">Name</span></span>|<span data-ttu-id="82f6d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="82f6d-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="82f6d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82f6d-122">Authorization</span></span>|<span data-ttu-id="82f6d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82f6d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="82f6d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="82f6d-125">Content-Type</span></span>|<span data-ttu-id="82f6d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82f6d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="82f6d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82f6d-128">Request body</span></span>
<span data-ttu-id="82f6d-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82f6d-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="82f6d-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="82f6d-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="82f6d-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="82f6d-131">Parameter</span></span>|<span data-ttu-id="82f6d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="82f6d-132">Type</span></span>|<span data-ttu-id="82f6d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="82f6d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82f6d-134">ids</span><span class="sxs-lookup"><span data-stu-id="82f6d-134">ids</span></span>|<span data-ttu-id="82f6d-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="82f6d-135">String collection</span></span>|<span data-ttu-id="82f6d-136">Список идентификаторов, соответствующих [updatableAsset](../resources/windowsupdates-updatableasset.md) ресурсам, которые необходимо удалить в качестве членов **updatableAssetGroup.**</span><span class="sxs-lookup"><span data-stu-id="82f6d-136">List of identifiers corresponding to the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources to remove as members of the **updatableAssetGroup**.</span></span>|
|<span data-ttu-id="82f6d-137">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="82f6d-137">memberEntityType</span></span>|<span data-ttu-id="82f6d-138">Строка</span><span class="sxs-lookup"><span data-stu-id="82f6d-138">String</span></span>|<span data-ttu-id="82f6d-139">Полный тип **updatableAsset** ресурсов.</span><span class="sxs-lookup"><span data-stu-id="82f6d-139">The full type of the **updatableAsset** resources.</span></span> <span data-ttu-id="82f6d-140">Возможные значения: `#microsoft.graph.windowsUpdates.azureADDevice` .</span><span class="sxs-lookup"><span data-stu-id="82f6d-140">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`.</span></span>|

## <a name="response"></a><span data-ttu-id="82f6d-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="82f6d-141">Response</span></span>

<span data-ttu-id="82f6d-142">В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="82f6d-142">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="82f6d-143">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="82f6d-143">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="82f6d-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="82f6d-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="82f6d-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="82f6d-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="82f6d-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="82f6d-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updatableassetgroup_removemembersbyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/removeMembersById
Content-Type: application/json

{
  "ids": [
    "String",
    "String",
    "String"
  ],
  "memberEntityType": "#microsoft.graph.windowsUpdates.azureADDevice"
}
```
# <a name="c"></a>[<span data-ttu-id="82f6d-147">C#</span><span class="sxs-lookup"><span data-stu-id="82f6d-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updatableassetgroup-removemembersbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82f6d-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82f6d-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updatableassetgroup-removemembersbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82f6d-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82f6d-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updatableassetgroup-removemembersbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="82f6d-150">Java</span><span class="sxs-lookup"><span data-stu-id="82f6d-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/updatableassetgroup-removemembersbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="82f6d-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="82f6d-151">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

