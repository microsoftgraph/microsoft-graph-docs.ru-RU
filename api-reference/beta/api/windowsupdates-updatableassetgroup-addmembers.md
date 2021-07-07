---
title: 'updatableAssetGroup: addMembers'
description: Добавление участников в updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 99d56de596cb28f21bffdd915911fd6ca6c9417f
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316489"
---
# <a name="updatableassetgroup-addmembers"></a><span data-ttu-id="9510e-103">updatableAssetGroup: addMembers</span><span class="sxs-lookup"><span data-stu-id="9510e-103">updatableAssetGroup: addMembers</span></span>
<span data-ttu-id="9510e-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="9510e-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9510e-105">Добавление участников в [updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="9510e-105">Add members to an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="9510e-106">В качестве участников можно добавить [ресурсы azureADDevice,](../resources/windowsupdates-azureaddevice.md) но не добавлять **updatableAssetGroup** в качестве участников.</span><span class="sxs-lookup"><span data-stu-id="9510e-106">You can add [azureADDevice](../resources/windowsupdates-azureaddevice.md) resources as members, but may not add **updatableAssetGroup** resources as members.</span></span>

<span data-ttu-id="9510e-107">Добавление устройства Azure AD в качестве члена группы updatable asset автоматически создает объект **azureADDevice,** если он еще не существует.</span><span class="sxs-lookup"><span data-stu-id="9510e-107">Adding an Azure AD device as a member of an updatable asset group automatically creates an **azureADDevice** object, if it does not already exist.</span></span>

<span data-ttu-id="9510e-108">Вы также можете использовать метод [addMembersById](windowsupdates-updatableassetgroup-addmembersbyid.md) для добавления участников.</span><span class="sxs-lookup"><span data-stu-id="9510e-108">You can also use the method [addMembersById](windowsupdates-updatableassetgroup-addmembersbyid.md) to add members.</span></span>

## <a name="permissions"></a><span data-ttu-id="9510e-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9510e-109">Permissions</span></span>
<span data-ttu-id="9510e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9510e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9510e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9510e-112">Permission type</span></span>|<span data-ttu-id="9510e-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9510e-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9510e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9510e-114">Delegated (work or school account)</span></span>|<span data-ttu-id="9510e-115">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9510e-115">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="9510e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9510e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9510e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9510e-117">Not supported.</span></span>|
|<span data-ttu-id="9510e-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9510e-118">Application</span></span>|<span data-ttu-id="9510e-119">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9510e-119">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9510e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9510e-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/addMembers
```

## <a name="request-headers"></a><span data-ttu-id="9510e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9510e-121">Request headers</span></span>
|<span data-ttu-id="9510e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="9510e-122">Name</span></span>|<span data-ttu-id="9510e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9510e-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9510e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9510e-124">Authorization</span></span>|<span data-ttu-id="9510e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9510e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9510e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9510e-127">Content-Type</span></span>|<span data-ttu-id="9510e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9510e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9510e-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9510e-130">Request body</span></span>
<span data-ttu-id="9510e-131">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9510e-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9510e-132">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="9510e-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9510e-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="9510e-133">Parameter</span></span>|<span data-ttu-id="9510e-134">Тип</span><span class="sxs-lookup"><span data-stu-id="9510e-134">Type</span></span>|<span data-ttu-id="9510e-135">Описание</span><span class="sxs-lookup"><span data-stu-id="9510e-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9510e-136">assets</span><span class="sxs-lookup"><span data-stu-id="9510e-136">assets</span></span>|<span data-ttu-id="9510e-137">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="9510e-137">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="9510e-138">Список **updatableAsset** ресурсов, которые необходимо добавить в качестве членов **updatableAssetGroup.**</span><span class="sxs-lookup"><span data-stu-id="9510e-138">List of **updatableAsset** resources to add as members of the **updatableAssetGroup**.</span></span>|

## <a name="response"></a><span data-ttu-id="9510e-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="9510e-139">Response</span></span>

<span data-ttu-id="9510e-140">В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="9510e-140">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="9510e-141">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9510e-141">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9510e-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="9510e-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9510e-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="9510e-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updatableassetgroup_addmembers"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/addMembers
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

### <a name="response"></a><span data-ttu-id="9510e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="9510e-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```
