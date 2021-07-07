---
title: 'updatableAsset: unenrollAssets'
description: Unenroll updatableAsset resources from update management by the deployment service.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 8f32ca029e94da476eb1b6c491057a3d4343b523
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317191"
---
# <a name="updatableasset-unenrollassets"></a><span data-ttu-id="05ae6-103">updatableAsset: unenrollAssets</span><span class="sxs-lookup"><span data-stu-id="05ae6-103">updatableAsset: unenrollAssets</span></span>
<span data-ttu-id="05ae6-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="05ae6-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05ae6-105">Unenroll [updatableAsset](../resources/windowsupdates-updatableasset.md) resources from update management by the deployment service.</span><span class="sxs-lookup"><span data-stu-id="05ae6-105">Unenroll [updatableAsset](../resources/windowsupdates-updatableasset.md) resources from update management by the deployment service.</span></span>

<span data-ttu-id="05ae6-106">Вы также можете использовать метод [unenrollAssetsById](windowsupdates-updatableasset-unenrollassetsbyid.md) для разгрузки активов.</span><span class="sxs-lookup"><span data-stu-id="05ae6-106">You can also use the method [unenrollAssetsById](windowsupdates-updatableasset-unenrollassetsbyid.md) to unenroll assets.</span></span>

## <a name="permissions"></a><span data-ttu-id="05ae6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05ae6-107">Permissions</span></span>
<span data-ttu-id="05ae6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05ae6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05ae6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05ae6-110">Permission type</span></span>|<span data-ttu-id="05ae6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="05ae6-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05ae6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05ae6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="05ae6-113">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05ae6-113">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="05ae6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05ae6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05ae6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05ae6-115">Not supported.</span></span>|
|<span data-ttu-id="05ae6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05ae6-116">Application</span></span>|<span data-ttu-id="05ae6-117">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05ae6-117">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05ae6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05ae6-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/unenrollAssets
```

## <a name="request-headers"></a><span data-ttu-id="05ae6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05ae6-119">Request headers</span></span>
|<span data-ttu-id="05ae6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="05ae6-120">Name</span></span>|<span data-ttu-id="05ae6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="05ae6-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="05ae6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05ae6-122">Authorization</span></span>|<span data-ttu-id="05ae6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05ae6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="05ae6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="05ae6-125">Content-Type</span></span>|<span data-ttu-id="05ae6-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05ae6-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="05ae6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="05ae6-128">Request body</span></span>
<span data-ttu-id="05ae6-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05ae6-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="05ae6-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="05ae6-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="05ae6-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="05ae6-131">Parameter</span></span>|<span data-ttu-id="05ae6-132">Тип</span><span class="sxs-lookup"><span data-stu-id="05ae6-132">Type</span></span>|<span data-ttu-id="05ae6-133">Описание</span><span class="sxs-lookup"><span data-stu-id="05ae6-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05ae6-134">updateCategory</span><span class="sxs-lookup"><span data-stu-id="05ae6-134">updateCategory</span></span>|<span data-ttu-id="05ae6-135">microsoft.graph.windowsUpdates.updateCategory</span><span class="sxs-lookup"><span data-stu-id="05ae6-135">microsoft.graph.windowsUpdates.updateCategory</span></span>|<span data-ttu-id="05ae6-136">Категория обновлений для службы для остановки управления.</span><span class="sxs-lookup"><span data-stu-id="05ae6-136">The category of updates for the service to stop managing.</span></span> <span data-ttu-id="05ae6-137">Поддерживает подмножество значений **для updateCategory.**</span><span class="sxs-lookup"><span data-stu-id="05ae6-137">Supports a subset of the values for **updateCategory**.</span></span> <span data-ttu-id="05ae6-138">Возможные значения: `feature` .</span><span class="sxs-lookup"><span data-stu-id="05ae6-138">Possible values are: `feature`.</span></span>|
|<span data-ttu-id="05ae6-139">assets</span><span class="sxs-lookup"><span data-stu-id="05ae6-139">assets</span></span>|<span data-ttu-id="05ae6-140">[коллекция microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="05ae6-140">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="05ae6-141">Список **ресурсов updatableAsset** для отката от управления обновлениями службой для данного **обновленияCategory**.</span><span class="sxs-lookup"><span data-stu-id="05ae6-141">List of **updatableAsset** resources to unenroll from update management by the service for the given **updateCategory**.</span></span>|



## <a name="response"></a><span data-ttu-id="05ae6-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="05ae6-142">Response</span></span>

<span data-ttu-id="05ae6-143">В случае успешного выполнения это действие возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="05ae6-143">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="05ae6-144">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="05ae6-144">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="05ae6-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="05ae6-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="05ae6-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="05ae6-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updatableasset_unenrollassets"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/unenrollAssets
Content-Type: application/json

{
  "updateCategory": "String",
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```


### <a name="response"></a><span data-ttu-id="05ae6-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="05ae6-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

