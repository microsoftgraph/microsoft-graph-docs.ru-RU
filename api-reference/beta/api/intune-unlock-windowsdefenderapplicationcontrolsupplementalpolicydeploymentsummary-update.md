---
title: Обновление Виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари
description: Обновление свойств объекта Виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1d98bf402c1dc580d3490177fb20dd6bf5e990dd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799754"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary"></a><span data-ttu-id="25b1e-103">Обновление Виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари</span><span class="sxs-lookup"><span data-stu-id="25b1e-103">Update windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary</span></span>

> <span data-ttu-id="25b1e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25b1e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25b1e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="25b1e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25b1e-106">Обновление свойств объекта [виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="25b1e-106">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25b1e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="25b1e-107">Prerequisites</span></span>
<span data-ttu-id="25b1e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25b1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25b1e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25b1e-110">Permission type</span></span>|<span data-ttu-id="25b1e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="25b1e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25b1e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25b1e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="25b1e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25b1e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="25b1e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25b1e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25b1e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25b1e-115">Not supported.</span></span>|
|<span data-ttu-id="25b1e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="25b1e-116">Application</span></span>|<span data-ttu-id="25b1e-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25b1e-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="25b1e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25b1e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deploySummary
```

## <a name="request-headers"></a><span data-ttu-id="25b1e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="25b1e-119">Request headers</span></span>
|<span data-ttu-id="25b1e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="25b1e-120">Header</span></span>|<span data-ttu-id="25b1e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="25b1e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25b1e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="25b1e-122">Authorization</span></span>|<span data-ttu-id="25b1e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25b1e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25b1e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="25b1e-124">Accept</span></span>|<span data-ttu-id="25b1e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="25b1e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25b1e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25b1e-126">Request body</span></span>
<span data-ttu-id="25b1e-127">В тексте запроса добавьте представление объекта [виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25b1e-127">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="25b1e-128">В следующей таблице приведены свойства, необходимые при создании [виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="25b1e-128">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="25b1e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="25b1e-129">Property</span></span>|<span data-ttu-id="25b1e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="25b1e-130">Type</span></span>|<span data-ttu-id="25b1e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="25b1e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25b1e-132">id</span><span class="sxs-lookup"><span data-stu-id="25b1e-132">id</span></span>|<span data-ttu-id="25b1e-133">String</span><span class="sxs-lookup"><span data-stu-id="25b1e-133">String</span></span>|<span data-ttu-id="25b1e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="25b1e-134">Key of the entity.</span></span>|
|<span data-ttu-id="25b1e-135">деплойеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="25b1e-135">deployedDeviceCount</span></span>|<span data-ttu-id="25b1e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="25b1e-136">Int32</span></span>|<span data-ttu-id="25b1e-137">Количество устройств, успешно развернутых в этой дополнительной политике Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="25b1e-137">Number of Devices that have successfully deployed this WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="25b1e-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="25b1e-138">failedDeviceCount</span></span>|<span data-ttu-id="25b1e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="25b1e-139">Int32</span></span>|<span data-ttu-id="25b1e-140">Количество устройств, которые не удалось развернуть эту дополнительную политику Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="25b1e-140">Number of Devices that have failed to deploy this WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="25b1e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="25b1e-141">Response</span></span>
<span data-ttu-id="25b1e-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="25b1e-142">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25b1e-143">Пример</span><span class="sxs-lookup"><span data-stu-id="25b1e-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="25b1e-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="25b1e-144">Request</span></span>
<span data-ttu-id="25b1e-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25b1e-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deploySummary
Content-type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary",
  "deployedDeviceCount": 3,
  "failedDeviceCount": 1
}
```

### <a name="response"></a><span data-ttu-id="25b1e-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="25b1e-146">Response</span></span>
<span data-ttu-id="25b1e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25b1e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary",
  "id": "2f8656ed-56ed-2f86-ed56-862fed56862f",
  "deployedDeviceCount": 3,
  "failedDeviceCount": 1
}
```




