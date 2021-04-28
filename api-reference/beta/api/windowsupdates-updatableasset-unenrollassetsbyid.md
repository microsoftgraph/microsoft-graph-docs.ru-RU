---
title: 'updatableAsset: unenrollAssetsById'
description: Unenroll updatableAsset resources of the same type from update management by the deployment service.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 8e738a6ecfcf5f6a11e2433f20c784d53fc8eedd
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067568"
---
# <a name="updatableasset-unenrollassetsbyid"></a><span data-ttu-id="3cb45-103">updatableAsset: unenrollAssetsById</span><span class="sxs-lookup"><span data-stu-id="3cb45-103">updatableAsset: unenrollAssetsById</span></span>
<span data-ttu-id="3cb45-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="3cb45-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cb45-105">Unenroll [updatableAsset](../resources/windowsupdates-updatableasset.md) resources of the same type from update management by the deployment service.</span><span class="sxs-lookup"><span data-stu-id="3cb45-105">Unenroll [updatableAsset](../resources/windowsupdates-updatableasset.md) resources of the same type from update management by the deployment service.</span></span>

<span data-ttu-id="3cb45-106">Вы также можете использовать метод [unenrollAssets](windowsupdates-updatableasset-unenrollassets.md) для разгрузки активов.</span><span class="sxs-lookup"><span data-stu-id="3cb45-106">You can also use the method [unenrollAssets](windowsupdates-updatableasset-unenrollassets.md) to unenroll assets.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cb45-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3cb45-107">Permissions</span></span>
<span data-ttu-id="3cb45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cb45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cb45-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3cb45-110">Permission type</span></span>|<span data-ttu-id="3cb45-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3cb45-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cb45-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3cb45-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3cb45-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cb45-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="3cb45-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3cb45-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cb45-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cb45-115">Not supported.</span></span>|
|<span data-ttu-id="3cb45-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3cb45-116">Application</span></span>|<span data-ttu-id="3cb45-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cb45-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cb45-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cb45-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/unenrollAssetsById
```

## <a name="request-headers"></a><span data-ttu-id="3cb45-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3cb45-119">Request headers</span></span>
|<span data-ttu-id="3cb45-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3cb45-120">Name</span></span>|<span data-ttu-id="3cb45-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3cb45-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3cb45-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3cb45-122">Authorization</span></span>|<span data-ttu-id="3cb45-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3cb45-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3cb45-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3cb45-125">Content-Type</span></span>|<span data-ttu-id="3cb45-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3cb45-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cb45-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3cb45-128">Request body</span></span>
<span data-ttu-id="3cb45-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3cb45-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3cb45-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="3cb45-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3cb45-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="3cb45-131">Parameter</span></span>|<span data-ttu-id="3cb45-132">Тип</span><span class="sxs-lookup"><span data-stu-id="3cb45-132">Type</span></span>|<span data-ttu-id="3cb45-133">Описание</span><span class="sxs-lookup"><span data-stu-id="3cb45-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cb45-134">updateCategory</span><span class="sxs-lookup"><span data-stu-id="3cb45-134">updateCategory</span></span>|<span data-ttu-id="3cb45-135">microsoft.graph.windowsUpdates.updateCategory</span><span class="sxs-lookup"><span data-stu-id="3cb45-135">microsoft.graph.windowsUpdates.updateCategory</span></span>|<span data-ttu-id="3cb45-136">Категория обновлений для службы для остановки управления.</span><span class="sxs-lookup"><span data-stu-id="3cb45-136">The category of updates for the service to stop managing.</span></span> <span data-ttu-id="3cb45-137">Поддерживает подмножество значений **для updateCategory.**</span><span class="sxs-lookup"><span data-stu-id="3cb45-137">Supports a subset of the values for **updateCategory**.</span></span> <span data-ttu-id="3cb45-138">Возможные значения: `feature` .</span><span class="sxs-lookup"><span data-stu-id="3cb45-138">Possible values are: `feature`.</span></span>|
|<span data-ttu-id="3cb45-139">memberEntityType</span><span class="sxs-lookup"><span data-stu-id="3cb45-139">memberEntityType</span></span>|<span data-ttu-id="3cb45-140">String</span><span class="sxs-lookup"><span data-stu-id="3cb45-140">String</span></span>|<span data-ttu-id="3cb45-141">Полный тип **updatableAsset** ресурсов.</span><span class="sxs-lookup"><span data-stu-id="3cb45-141">The full type of the **updatableAsset** resources.</span></span> <span data-ttu-id="3cb45-142">Возможные значения: `#microsoft.graph.windowsUpdates.azureADDevice` .</span><span class="sxs-lookup"><span data-stu-id="3cb45-142">Possible values are: `#microsoft.graph.windowsUpdates.azureADDevice`.</span></span>|
|<span data-ttu-id="3cb45-143">ids</span><span class="sxs-lookup"><span data-stu-id="3cb45-143">ids</span></span>|<span data-ttu-id="3cb45-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3cb45-144">String collection</span></span>|<span data-ttu-id="3cb45-145">Список идентификаторов, соответствующих **updatableAsset** ресурсам, чтобы отстраить от управления обновлением службой данного **обновленияCategory.**</span><span class="sxs-lookup"><span data-stu-id="3cb45-145">List of identifiers corresponding to the **updatableAsset** resources to unenroll from update management by the service for the given **updateCategory**.</span></span>|

## <a name="response"></a><span data-ttu-id="3cb45-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="3cb45-146">Response</span></span>

<span data-ttu-id="3cb45-147">В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="3cb45-147">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="3cb45-148">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3cb45-148">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3cb45-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="3cb45-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3cb45-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="3cb45-150">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updatableasset_unenrollassetsbyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/unenrollAssetsById
Content-Type: application/json

{
  "updateCategory": "feature",
  "memberEntityType": "#microsoft.graph.windowsUpdates.azureADDevice",
  "ids": [
    "String",
    "String",
    "String"
  ]
}
```

### <a name="response"></a><span data-ttu-id="3cb45-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cb45-151">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

