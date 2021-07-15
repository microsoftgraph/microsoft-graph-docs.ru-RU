---
title: 'updatableAssetGroup: removeMembers'
description: Удаление участников из updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: bd2275ce1971d341214899a5b56cecdd9c820e3c
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440459"
---
# <a name="updatableassetgroup-removemembers"></a><span data-ttu-id="97d50-103">updatableAssetGroup: removeMembers</span><span class="sxs-lookup"><span data-stu-id="97d50-103">updatableAssetGroup: removeMembers</span></span>
<span data-ttu-id="97d50-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="97d50-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97d50-105">Удаление участников [из updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="97d50-105">Remove members from an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="97d50-106">Вы также можете использовать метод [removeMembersById](windowsupdates-updatableassetgroup-removemembersbyid.md) для удаления участников.</span><span class="sxs-lookup"><span data-stu-id="97d50-106">You can also use the method [removeMembersById](windowsupdates-updatableassetgroup-removemembersbyid.md) to remove members.</span></span>

## <a name="permissions"></a><span data-ttu-id="97d50-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97d50-107">Permissions</span></span>
<span data-ttu-id="97d50-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97d50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97d50-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97d50-110">Permission type</span></span>|<span data-ttu-id="97d50-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97d50-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97d50-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97d50-112">Delegated (work or school account)</span></span>|<span data-ttu-id="97d50-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97d50-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="97d50-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97d50-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97d50-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97d50-115">Not supported.</span></span>|
|<span data-ttu-id="97d50-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="97d50-116">Application</span></span>|<span data-ttu-id="97d50-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97d50-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97d50-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97d50-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/removeMembers
```

## <a name="request-headers"></a><span data-ttu-id="97d50-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97d50-119">Request headers</span></span>
|<span data-ttu-id="97d50-120">Имя</span><span class="sxs-lookup"><span data-stu-id="97d50-120">Name</span></span>|<span data-ttu-id="97d50-121">Описание</span><span class="sxs-lookup"><span data-stu-id="97d50-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="97d50-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97d50-122">Authorization</span></span>|<span data-ttu-id="97d50-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97d50-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="97d50-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97d50-125">Content-Type</span></span>|<span data-ttu-id="97d50-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97d50-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="97d50-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97d50-128">Request body</span></span>
<span data-ttu-id="97d50-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97d50-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="97d50-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="97d50-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="97d50-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="97d50-131">Parameter</span></span>|<span data-ttu-id="97d50-132">Тип</span><span class="sxs-lookup"><span data-stu-id="97d50-132">Type</span></span>|<span data-ttu-id="97d50-133">Описание</span><span class="sxs-lookup"><span data-stu-id="97d50-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97d50-134">assets</span><span class="sxs-lookup"><span data-stu-id="97d50-134">assets</span></span>|<span data-ttu-id="97d50-135">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="97d50-135">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="97d50-136">Список **updatableAsset** ресурсов, которые необходимо удалить в качестве членов **updatableAssetGroup.**</span><span class="sxs-lookup"><span data-stu-id="97d50-136">List of **updatableAsset** resources to remove as members of the **updatableAssetGroup**.</span></span>|

## <a name="response"></a><span data-ttu-id="97d50-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="97d50-137">Response</span></span>

<span data-ttu-id="97d50-138">В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="97d50-138">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="97d50-139">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="97d50-139">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="97d50-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="97d50-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="97d50-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="97d50-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="97d50-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="97d50-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updatableassetgroup_removemembers"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/removeMembers
Content-Type: application/json

{
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="97d50-143">C#</span><span class="sxs-lookup"><span data-stu-id="97d50-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updatableassetgroup-removemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97d50-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97d50-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updatableassetgroup-removemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97d50-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97d50-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updatableassetgroup-removemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97d50-146">Java</span><span class="sxs-lookup"><span data-stu-id="97d50-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/updatableassetgroup-removemembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="97d50-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="97d50-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```
