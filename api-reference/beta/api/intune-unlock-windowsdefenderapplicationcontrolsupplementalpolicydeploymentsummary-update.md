---
title: Обновление Виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари
description: Обновление свойств объекта Виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ebc8e6e2cd7741debdc9e40f7d6aff92e2551be
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095802"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary"></a><span data-ttu-id="ebbb3-103">Обновление Виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари</span><span class="sxs-lookup"><span data-stu-id="ebbb3-103">Update windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary</span></span>

<span data-ttu-id="ebbb3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebbb3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebbb3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebbb3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebbb3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ebbb3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebbb3-107">Обновление свойств объекта [виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="ebbb3-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebbb3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ebbb3-108">Prerequisites</span></span>
<span data-ttu-id="ebbb3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebbb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebbb3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebbb3-111">Permission type</span></span>|<span data-ttu-id="ebbb3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebbb3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebbb3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebbb3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ebbb3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebbb3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ebbb3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebbb3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebbb3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebbb3-116">Not supported.</span></span>|
|<span data-ttu-id="ebbb3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebbb3-117">Application</span></span>|<span data-ttu-id="ebbb3-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebbb3-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebbb3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebbb3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deploySummary
```

## <a name="request-headers"></a><span data-ttu-id="ebbb3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ebbb3-120">Request headers</span></span>
|<span data-ttu-id="ebbb3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ebbb3-121">Header</span></span>|<span data-ttu-id="ebbb3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ebbb3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebbb3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ebbb3-123">Authorization</span></span>|<span data-ttu-id="ebbb3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ebbb3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebbb3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ebbb3-125">Accept</span></span>|<span data-ttu-id="ebbb3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ebbb3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebbb3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ebbb3-127">Request body</span></span>
<span data-ttu-id="ebbb3-128">В тексте запроса добавьте представление объекта [виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ebbb3-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="ebbb3-129">В следующей таблице приведены свойства, необходимые при создании [виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="ebbb3-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="ebbb3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebbb3-130">Property</span></span>|<span data-ttu-id="ebbb3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ebbb3-131">Type</span></span>|<span data-ttu-id="ebbb3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ebbb3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebbb3-133">id</span><span class="sxs-lookup"><span data-stu-id="ebbb3-133">id</span></span>|<span data-ttu-id="ebbb3-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ebbb3-134">String</span></span>|<span data-ttu-id="ebbb3-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ebbb3-135">Key of the entity.</span></span>|
|<span data-ttu-id="ebbb3-136">деплойеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="ebbb3-136">deployedDeviceCount</span></span>|<span data-ttu-id="ebbb3-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ebbb3-137">Int32</span></span>|<span data-ttu-id="ebbb3-138">Количество устройств, успешно развернутых в этой дополнительной политике Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="ebbb3-138">Number of Devices that have successfully deployed this WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="ebbb3-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ebbb3-139">failedDeviceCount</span></span>|<span data-ttu-id="ebbb3-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ebbb3-140">Int32</span></span>|<span data-ttu-id="ebbb3-141">Количество устройств, которые не удалось развернуть эту дополнительную политику Виндовсдефендераппликатионконтрол.</span><span class="sxs-lookup"><span data-stu-id="ebbb3-141">Number of Devices that have failed to deploy this WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="ebbb3-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebbb3-142">Response</span></span>
<span data-ttu-id="ebbb3-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсдефендераппликатионконтролсупплементалполицидеплойментсуммари](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ebbb3-143">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebbb3-144">Пример</span><span class="sxs-lookup"><span data-stu-id="ebbb3-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebbb3-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebbb3-145">Request</span></span>
<span data-ttu-id="ebbb3-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebbb3-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ebbb3-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebbb3-147">Response</span></span>
<span data-ttu-id="ebbb3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ebbb3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






