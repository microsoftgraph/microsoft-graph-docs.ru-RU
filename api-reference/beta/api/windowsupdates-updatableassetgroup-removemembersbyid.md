---
title: 'updatableAssetGroup: removeMembersById'
description: Удалите членов одного типа из updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 1ea11298a7aa19d60b69b98b07c003887aae30b3
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068251"
---
# <a name="updatableassetgroup-removemembersbyid"></a><span data-ttu-id="9523f-103">updatableAssetGroup: removeMembersById</span><span class="sxs-lookup"><span data-stu-id="9523f-103">updatableAssetGroup: removeMembersById</span></span>
<span data-ttu-id="9523f-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="9523f-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9523f-105">Удалите членов одного типа из [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span><span class="sxs-lookup"><span data-stu-id="9523f-105">Remove members of the same type from an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="9523f-106">Вы также можете использовать метод [removeMembers для](windowsupdates-updatableassetgroup-removemembers.md) удаления участников.</span><span class="sxs-lookup"><span data-stu-id="9523f-106">You can also use the method [removeMembers](windowsupdates-updatableassetgroup-removemembers.md) to remove members.</span></span>

## <a name="permissions"></a><span data-ttu-id="9523f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9523f-107">Permissions</span></span>
<span data-ttu-id="9523f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9523f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9523f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9523f-110">Permission type</span></span>|<span data-ttu-id="9523f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9523f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9523f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9523f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9523f-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9523f-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="9523f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9523f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9523f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9523f-115">Not supported.</span></span>|
|<span data-ttu-id="9523f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9523f-116">Application</span></span>|<span data-ttu-id="9523f-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9523f-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9523f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9523f-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/removeMembersById
```

## <a name="request-headers"></a><span data-ttu-id="9523f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9523f-119">Request headers</span></span>
|<span data-ttu-id="9523f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9523f-120">Name</span></span>|<span data-ttu-id="9523f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9523f-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9523f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9523f-122">Authorization</span></span>|<span data-ttu-id="9523f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9523f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9523f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9523f-125">Content-Type</span></span>|<span data-ttu-id="9523f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9523f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9523f-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9523f-128">Request body</span></span>
<span data-ttu-id="9523f-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9523f-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9523f-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="9523f-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9523f-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="9523f-131">Parameter</span></span>|<span data-ttu-id="9523f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="9523f-132">Type</span></span>|<span data-ttu-id="9523f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="9523f-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9523f-134">ids</span><span class="sxs-lookup"><span data-stu-id="9523f-134">ids</span></span>|<span data-ttu-id="9523f-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9523f-135">String collection</span></span>|<span data-ttu-id="9523f-136">Список идентификаторов, соответствующих [updatableAsset](../resources/windowsupdates-updatableasset.md) ресурсам, которые необходимо удалить в качестве членов **updatableAssetGroup.**</span><span class="sxs-lookup"><span data-stu-id="9523f-136">List of identifiers corresponding to the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources to remove as members of the **updatableAssetGroup**.</span></span>|
|<span data-ttu-id="9523f-137">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="9523f-137">memberEntityType</span></span>|<span data-ttu-id="9523f-138">String</span><span class="sxs-lookup"><span data-stu-id="9523f-138">String</span></span>|<span data-ttu-id="9523f-139">Полный тип **updatableAsset** ресурсов.</span><span class="sxs-lookup"><span data-stu-id="9523f-139">The full type of the **updatableAsset** resources.</span></span> <span data-ttu-id="9523f-140">Возможные значения: `#microsoft.graph.windowsUpdates.azureADDevice` .</span><span class="sxs-lookup"><span data-stu-id="9523f-140">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`.</span></span>|

## <a name="response"></a><span data-ttu-id="9523f-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="9523f-141">Response</span></span>

<span data-ttu-id="9523f-142">В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="9523f-142">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="9523f-143">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9523f-143">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9523f-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="9523f-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9523f-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="9523f-145">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="9523f-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="9523f-146">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

