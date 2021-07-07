---
title: 'updatableAssetGroup: removeMembers'
description: Удаление участников из updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 80ab7cab56a72633d7a4cb6f1c81d51cf0263d98
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317184"
---
# <a name="updatableassetgroup-removemembers"></a><span data-ttu-id="43df5-103">updatableAssetGroup: removeMembers</span><span class="sxs-lookup"><span data-stu-id="43df5-103">updatableAssetGroup: removeMembers</span></span>
<span data-ttu-id="43df5-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="43df5-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43df5-105">Удаление участников [из updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="43df5-105">Remove members from an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="43df5-106">Вы также можете использовать метод [removeMembersById](windowsupdates-updatableassetgroup-removemembersbyid.md) для удаления участников.</span><span class="sxs-lookup"><span data-stu-id="43df5-106">You can also use the method [removeMembersById](windowsupdates-updatableassetgroup-removemembersbyid.md) to remove members.</span></span>

## <a name="permissions"></a><span data-ttu-id="43df5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="43df5-107">Permissions</span></span>
<span data-ttu-id="43df5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43df5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43df5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43df5-110">Permission type</span></span>|<span data-ttu-id="43df5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="43df5-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43df5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43df5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43df5-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43df5-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="43df5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43df5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43df5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43df5-115">Not supported.</span></span>|
|<span data-ttu-id="43df5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43df5-116">Application</span></span>|<span data-ttu-id="43df5-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43df5-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43df5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43df5-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/removeMembers
```

## <a name="request-headers"></a><span data-ttu-id="43df5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43df5-119">Request headers</span></span>
|<span data-ttu-id="43df5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="43df5-120">Name</span></span>|<span data-ttu-id="43df5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="43df5-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="43df5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43df5-122">Authorization</span></span>|<span data-ttu-id="43df5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43df5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="43df5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="43df5-125">Content-Type</span></span>|<span data-ttu-id="43df5-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43df5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="43df5-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43df5-128">Request body</span></span>
<span data-ttu-id="43df5-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43df5-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="43df5-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="43df5-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="43df5-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="43df5-131">Parameter</span></span>|<span data-ttu-id="43df5-132">Тип</span><span class="sxs-lookup"><span data-stu-id="43df5-132">Type</span></span>|<span data-ttu-id="43df5-133">Описание</span><span class="sxs-lookup"><span data-stu-id="43df5-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43df5-134">assets</span><span class="sxs-lookup"><span data-stu-id="43df5-134">assets</span></span>|<span data-ttu-id="43df5-135">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="43df5-135">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="43df5-136">Список **updatableAsset** ресурсов, которые необходимо удалить в качестве членов **updatableAssetGroup.**</span><span class="sxs-lookup"><span data-stu-id="43df5-136">List of **updatableAsset** resources to remove as members of the **updatableAssetGroup**.</span></span>|

## <a name="response"></a><span data-ttu-id="43df5-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="43df5-137">Response</span></span>

<span data-ttu-id="43df5-138">В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="43df5-138">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="43df5-139">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="43df5-139">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="43df5-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="43df5-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="43df5-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="43df5-141">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="43df5-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="43df5-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```
