---
title: 'updatableAssetGroup: addMembersById'
description: Добавьте членов одного типа в updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 004b8600644f6fcc8a599b53761f66491f62ebd8
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067586"
---
# <a name="updatableassetgroup-addmembersbyid"></a><span data-ttu-id="c07c2-103">updatableAssetGroup: addMembersById</span><span class="sxs-lookup"><span data-stu-id="c07c2-103">updatableAssetGroup: addMembersById</span></span>
<span data-ttu-id="c07c2-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="c07c2-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c07c2-105">Добавьте членов одного типа в [updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="c07c2-105">Add members of the same type to an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="c07c2-106">Можно также использовать метод [addMembers для](windowsupdates-updatableassetgroup-addmembers.md) добавления участников.</span><span class="sxs-lookup"><span data-stu-id="c07c2-106">You can also use the method [addMembers](windowsupdates-updatableassetgroup-addmembers.md) to add members.</span></span>

## <a name="permissions"></a><span data-ttu-id="c07c2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c07c2-107">Permissions</span></span>
<span data-ttu-id="c07c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c07c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c07c2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c07c2-110">Permission type</span></span>|<span data-ttu-id="c07c2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c07c2-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c07c2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c07c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c07c2-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c07c2-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="c07c2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c07c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c07c2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c07c2-115">Not supported.</span></span>|
|<span data-ttu-id="c07c2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c07c2-116">Application</span></span>|<span data-ttu-id="c07c2-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c07c2-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c07c2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c07c2-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/addMembersById
```

## <a name="request-headers"></a><span data-ttu-id="c07c2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c07c2-119">Request headers</span></span>
|<span data-ttu-id="c07c2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c07c2-120">Name</span></span>|<span data-ttu-id="c07c2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c07c2-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c07c2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c07c2-122">Authorization</span></span>|<span data-ttu-id="c07c2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c07c2-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c07c2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c07c2-125">Content-Type</span></span>|<span data-ttu-id="c07c2-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c07c2-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c07c2-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c07c2-128">Request body</span></span>
<span data-ttu-id="c07c2-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c07c2-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c07c2-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c07c2-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c07c2-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="c07c2-131">Parameter</span></span>|<span data-ttu-id="c07c2-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c07c2-132">Type</span></span>|<span data-ttu-id="c07c2-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c07c2-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c07c2-134">ids</span><span class="sxs-lookup"><span data-stu-id="c07c2-134">ids</span></span>|<span data-ttu-id="c07c2-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c07c2-135">String collection</span></span>|<span data-ttu-id="c07c2-136">Список идентификаторов, соответствующих [updatableAsset](../resources/windowsupdates-updatableasset.md) ресурсам, которые необходимо добавить в качестве членов **updatableAssetGroup.**</span><span class="sxs-lookup"><span data-stu-id="c07c2-136">List of identifiers corresponding to the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources to add as members of the **updatableAssetGroup**.</span></span>|
|<span data-ttu-id="c07c2-137">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="c07c2-137">memberEntityType</span></span>|<span data-ttu-id="c07c2-138">String</span><span class="sxs-lookup"><span data-stu-id="c07c2-138">String</span></span>|<span data-ttu-id="c07c2-139">Полный тип **updatableAsset** ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c07c2-139">The full type of the **updatableAsset** resources.</span></span> <span data-ttu-id="c07c2-140">Возможные значения: `#microsoft.graph.windowsUpdates.azureADDevice` .</span><span class="sxs-lookup"><span data-stu-id="c07c2-140">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`.</span></span>|

## <a name="response"></a><span data-ttu-id="c07c2-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="c07c2-141">Response</span></span>

<span data-ttu-id="c07c2-142">В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="c07c2-142">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="c07c2-143">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c07c2-143">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c07c2-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="c07c2-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c07c2-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="c07c2-145">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="c07c2-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="c07c2-146">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

