---
title: 'updatableAssetGroup: addMembers'
description: Добавление участников в updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: dbb5cd4c156940379eaf114235099d9fd53fb08f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068168"
---
# <a name="updatableassetgroup-addmembers"></a><span data-ttu-id="9a1f1-103">updatableAssetGroup: addMembers</span><span class="sxs-lookup"><span data-stu-id="9a1f1-103">updatableAssetGroup: addMembers</span></span>
<span data-ttu-id="9a1f1-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="9a1f1-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a1f1-105">Добавление участников в [updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="9a1f1-105">Add members to an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="9a1f1-106">В качестве участников можно добавить [ресурсы azureADDevice,](../resources/windowsupdates-azureaddevice.md) но не добавлять **updatableAssetGroup** в качестве участников.</span><span class="sxs-lookup"><span data-stu-id="9a1f1-106">You can add [azureADDevice](../resources/windowsupdates-azureaddevice.md) resources as members, but may not add **updatableAssetGroup** resources as members.</span></span>

<span data-ttu-id="9a1f1-107">Добавление устройства Azure AD в качестве члена группы updatable asset автоматически создает объект **azureADDevice,** если он еще не существует.</span><span class="sxs-lookup"><span data-stu-id="9a1f1-107">Adding an Azure AD device as a member of an updatable asset group automatically creates an **azureADDevice** object, if it does not already exist.</span></span>

<span data-ttu-id="9a1f1-108">Вы также можете использовать метод [addMembersById](windowsupdates-updatableassetgroup-addmembersbyid.md) для добавления участников.</span><span class="sxs-lookup"><span data-stu-id="9a1f1-108">You can also use the method [addMembersById](windowsupdates-updatableassetgroup-addmembersbyid.md) to add members.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a1f1-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a1f1-109">Permissions</span></span>
<span data-ttu-id="9a1f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a1f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a1f1-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a1f1-112">Permission type</span></span>|<span data-ttu-id="9a1f1-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a1f1-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a1f1-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a1f1-114">Delegated (work or school account)</span></span>|<span data-ttu-id="9a1f1-115">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a1f1-115">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="9a1f1-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a1f1-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a1f1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a1f1-117">Not supported.</span></span>|
|<span data-ttu-id="9a1f1-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a1f1-118">Application</span></span>|<span data-ttu-id="9a1f1-119">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a1f1-119">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a1f1-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a1f1-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /updatableAssetGroup/{updatableAssetGroupId}/addMembers
```

## <a name="request-headers"></a><span data-ttu-id="9a1f1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a1f1-121">Request headers</span></span>
|<span data-ttu-id="9a1f1-122">Имя</span><span class="sxs-lookup"><span data-stu-id="9a1f1-122">Name</span></span>|<span data-ttu-id="9a1f1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9a1f1-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9a1f1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a1f1-124">Authorization</span></span>|<span data-ttu-id="9a1f1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a1f1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9a1f1-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9a1f1-127">Content-Type</span></span>|<span data-ttu-id="9a1f1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a1f1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a1f1-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a1f1-130">Request body</span></span>
<span data-ttu-id="9a1f1-131">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a1f1-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9a1f1-132">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="9a1f1-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9a1f1-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="9a1f1-133">Parameter</span></span>|<span data-ttu-id="9a1f1-134">Тип</span><span class="sxs-lookup"><span data-stu-id="9a1f1-134">Type</span></span>|<span data-ttu-id="9a1f1-135">Описание</span><span class="sxs-lookup"><span data-stu-id="9a1f1-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a1f1-136">assets</span><span class="sxs-lookup"><span data-stu-id="9a1f1-136">assets</span></span>|<span data-ttu-id="9a1f1-137">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="9a1f1-137">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="9a1f1-138">Список **updatableAsset** ресурсов, которые необходимо добавить в качестве членов **updatableAssetGroup.**</span><span class="sxs-lookup"><span data-stu-id="9a1f1-138">List of **updatableAsset** resources to add as members of the **updatableAssetGroup**.</span></span>|

## <a name="response"></a><span data-ttu-id="9a1f1-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a1f1-139">Response</span></span>

<span data-ttu-id="9a1f1-140">В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="9a1f1-140">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="9a1f1-141">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9a1f1-141">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9a1f1-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="9a1f1-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9a1f1-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a1f1-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updatableassetgroup_addmembers"
}
-->
``` http
POST https://graph.microsoft.com/beta/updatableAssetGroup/{updatableAssetGroupId}/addMembers
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

### <a name="response"></a><span data-ttu-id="9a1f1-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a1f1-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```
