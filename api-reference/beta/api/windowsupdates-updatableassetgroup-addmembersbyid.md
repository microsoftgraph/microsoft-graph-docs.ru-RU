---
title: 'updatableAssetGroup: addMembersById'
description: Добавьте членов одного типа в updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 27585b3ad87c4154140024705227612a988c7a76
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239490"
---
# <a name="updatableassetgroup-addmembersbyid"></a><span data-ttu-id="6ce16-103">updatableAssetGroup: addMembersById</span><span class="sxs-lookup"><span data-stu-id="6ce16-103">updatableAssetGroup: addMembersById</span></span>
<span data-ttu-id="6ce16-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="6ce16-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ce16-105">Добавьте членов одного типа в [updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="6ce16-105">Add members of the same type to an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="6ce16-106">Можно также использовать метод [addMembers для](windowsupdates-updatableassetgroup-addmembers.md) добавления участников.</span><span class="sxs-lookup"><span data-stu-id="6ce16-106">You can also use the method [addMembers](windowsupdates-updatableassetgroup-addmembers.md) to add members.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ce16-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ce16-107">Permissions</span></span>
<span data-ttu-id="6ce16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ce16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ce16-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ce16-110">Permission type</span></span>|<span data-ttu-id="6ce16-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ce16-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ce16-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ce16-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6ce16-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ce16-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="6ce16-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ce16-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ce16-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ce16-115">Not supported.</span></span>|
|<span data-ttu-id="6ce16-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ce16-116">Application</span></span>|<span data-ttu-id="6ce16-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ce16-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ce16-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ce16-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/addMembersById
```

## <a name="request-headers"></a><span data-ttu-id="6ce16-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ce16-119">Request headers</span></span>
|<span data-ttu-id="6ce16-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6ce16-120">Name</span></span>|<span data-ttu-id="6ce16-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6ce16-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6ce16-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ce16-122">Authorization</span></span>|<span data-ttu-id="6ce16-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ce16-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6ce16-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6ce16-125">Content-Type</span></span>|<span data-ttu-id="6ce16-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ce16-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ce16-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ce16-128">Request body</span></span>
<span data-ttu-id="6ce16-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ce16-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6ce16-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="6ce16-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6ce16-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="6ce16-131">Parameter</span></span>|<span data-ttu-id="6ce16-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6ce16-132">Type</span></span>|<span data-ttu-id="6ce16-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6ce16-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ce16-134">ids</span><span class="sxs-lookup"><span data-stu-id="6ce16-134">ids</span></span>|<span data-ttu-id="6ce16-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6ce16-135">String collection</span></span>|<span data-ttu-id="6ce16-136">Список идентификаторов, соответствующих [updatableAsset](../resources/windowsupdates-updatableasset.md) ресурсам, которые необходимо добавить в качестве членов **updatableAssetGroup.**</span><span class="sxs-lookup"><span data-stu-id="6ce16-136">List of identifiers corresponding to the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources to add as members of the **updatableAssetGroup**.</span></span>|
|<span data-ttu-id="6ce16-137">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="6ce16-137">memberEntityType</span></span>|<span data-ttu-id="6ce16-138">Строка</span><span class="sxs-lookup"><span data-stu-id="6ce16-138">String</span></span>|<span data-ttu-id="6ce16-139">Полный тип **updatableAsset** ресурсов.</span><span class="sxs-lookup"><span data-stu-id="6ce16-139">The full type of the **updatableAsset** resources.</span></span> <span data-ttu-id="6ce16-140">Возможные значения: `#microsoft.graph.windowsUpdates.azureADDevice` .</span><span class="sxs-lookup"><span data-stu-id="6ce16-140">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`.</span></span>|

## <a name="response"></a><span data-ttu-id="6ce16-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ce16-141">Response</span></span>

<span data-ttu-id="6ce16-142">В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="6ce16-142">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="6ce16-143">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6ce16-143">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6ce16-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="6ce16-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6ce16-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ce16-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6ce16-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ce16-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updatableassetgroup_addmembersbyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/addMembersById
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
# <a name="c"></a>[<span data-ttu-id="6ce16-147">C#</span><span class="sxs-lookup"><span data-stu-id="6ce16-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updatableassetgroup-addmembersbyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ce16-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ce16-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updatableassetgroup-addmembersbyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ce16-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ce16-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updatableassetgroup-addmembersbyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6ce16-150">Java</span><span class="sxs-lookup"><span data-stu-id="6ce16-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/updatableassetgroup-addmembersbyid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6ce16-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ce16-151">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

