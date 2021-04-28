---
title: 'updatableAssetGroup: removeMembers'
description: Удаление участников из updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 2964bfc1fad02d81bab33936fde1e2cf03293830
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068278"
---
# <a name="updatableassetgroup-removemembers"></a><span data-ttu-id="a2e0b-103">updatableAssetGroup: removeMembers</span><span class="sxs-lookup"><span data-stu-id="a2e0b-103">updatableAssetGroup: removeMembers</span></span>
<span data-ttu-id="a2e0b-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="a2e0b-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2e0b-105">Удаление участников [из updatableAssetGroup.](../resources/windowsupdates-updatableassetgroup.md)</span><span class="sxs-lookup"><span data-stu-id="a2e0b-105">Remove members from an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="a2e0b-106">Вы также можете использовать метод [removeMembersById](windowsupdates-updatableassetgroup-removemembersbyid.md) для удаления участников.</span><span class="sxs-lookup"><span data-stu-id="a2e0b-106">You can also use the method [removeMembersById](windowsupdates-updatableassetgroup-removemembersbyid.md) to remove members.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2e0b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2e0b-107">Permissions</span></span>
<span data-ttu-id="a2e0b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2e0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2e0b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2e0b-110">Permission type</span></span>|<span data-ttu-id="a2e0b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2e0b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2e0b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2e0b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2e0b-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2e0b-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="a2e0b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2e0b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2e0b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2e0b-115">Not supported.</span></span>|
|<span data-ttu-id="a2e0b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2e0b-116">Application</span></span>|<span data-ttu-id="a2e0b-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2e0b-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2e0b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2e0b-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /updatableAssetGroup/{updatableAssetGroupId}/removeMembers
```

## <a name="request-headers"></a><span data-ttu-id="a2e0b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2e0b-119">Request headers</span></span>
|<span data-ttu-id="a2e0b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a2e0b-120">Name</span></span>|<span data-ttu-id="a2e0b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a2e0b-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a2e0b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2e0b-122">Authorization</span></span>|<span data-ttu-id="a2e0b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2e0b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a2e0b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a2e0b-125">Content-Type</span></span>|<span data-ttu-id="a2e0b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2e0b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2e0b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2e0b-128">Request body</span></span>
<span data-ttu-id="a2e0b-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2e0b-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a2e0b-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a2e0b-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a2e0b-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="a2e0b-131">Parameter</span></span>|<span data-ttu-id="a2e0b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="a2e0b-132">Type</span></span>|<span data-ttu-id="a2e0b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a2e0b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2e0b-134">assets</span><span class="sxs-lookup"><span data-stu-id="a2e0b-134">assets</span></span>|<span data-ttu-id="a2e0b-135">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="a2e0b-135">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="a2e0b-136">Список **updatableAsset** ресурсов, которые необходимо удалить в качестве членов **updatableAssetGroup.**</span><span class="sxs-lookup"><span data-stu-id="a2e0b-136">List of **updatableAsset** resources to remove as members of the **updatableAssetGroup**.</span></span>|

## <a name="response"></a><span data-ttu-id="a2e0b-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2e0b-137">Response</span></span>

<span data-ttu-id="a2e0b-138">В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="a2e0b-138">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="a2e0b-139">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a2e0b-139">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a2e0b-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="a2e0b-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a2e0b-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2e0b-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updatableassetgroup_removemembers"
}
-->
``` http
POST https://graph.microsoft.com/beta/updatableAssetGroup/{updatableAssetGroupId}/removeMembers
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

### <a name="response"></a><span data-ttu-id="a2e0b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2e0b-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

