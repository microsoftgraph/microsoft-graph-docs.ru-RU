---
title: Обновление windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary
description: Обновление свойств объекта WindowsDefenderApplicationControlSupplementalPolicyDeploymentSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a32cbbc7ed88871838d75c5c917191179fe6ff3a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133894"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary"></a><span data-ttu-id="55b7a-103">Обновление windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="55b7a-103">Update windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary</span></span>

<span data-ttu-id="55b7a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55b7a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55b7a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55b7a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55b7a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55b7a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55b7a-107">Обновление свойств объекта [WindowsDefenderApplicationControlSupplementalPolicyDeploymentSummary.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)</span><span class="sxs-lookup"><span data-stu-id="55b7a-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55b7a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="55b7a-108">Prerequisites</span></span>
<span data-ttu-id="55b7a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55b7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55b7a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55b7a-111">Permission type</span></span>|<span data-ttu-id="55b7a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55b7a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55b7a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55b7a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55b7a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55b7a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="55b7a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55b7a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55b7a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55b7a-116">Not supported.</span></span>|
|<span data-ttu-id="55b7a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="55b7a-117">Application</span></span>|<span data-ttu-id="55b7a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55b7a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55b7a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55b7a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deploySummary
```

## <a name="request-headers"></a><span data-ttu-id="55b7a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="55b7a-120">Request headers</span></span>
|<span data-ttu-id="55b7a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55b7a-121">Header</span></span>|<span data-ttu-id="55b7a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="55b7a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55b7a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="55b7a-123">Authorization</span></span>|<span data-ttu-id="55b7a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55b7a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55b7a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="55b7a-125">Accept</span></span>|<span data-ttu-id="55b7a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55b7a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55b7a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55b7a-127">Request body</span></span>
<span data-ttu-id="55b7a-128">В теле запроса поставляем представление JSON для [объекта windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)</span><span class="sxs-lookup"><span data-stu-id="55b7a-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="55b7a-129">В следующей таблице показаны свойства, необходимые при создании [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)</span><span class="sxs-lookup"><span data-stu-id="55b7a-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="55b7a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="55b7a-130">Property</span></span>|<span data-ttu-id="55b7a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="55b7a-131">Type</span></span>|<span data-ttu-id="55b7a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="55b7a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55b7a-133">id</span><span class="sxs-lookup"><span data-stu-id="55b7a-133">id</span></span>|<span data-ttu-id="55b7a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="55b7a-134">String</span></span>|<span data-ttu-id="55b7a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="55b7a-135">Key of the entity.</span></span>|
|<span data-ttu-id="55b7a-136">deployedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="55b7a-136">deployedDeviceCount</span></span>|<span data-ttu-id="55b7a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="55b7a-137">Int32</span></span>|<span data-ttu-id="55b7a-138">Количество устройств, успешно развернутых в этой дополнительной политике WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="55b7a-138">Number of Devices that have successfully deployed this WindowsDefenderApplicationControl supplemental policy.</span></span>|
|<span data-ttu-id="55b7a-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="55b7a-139">failedDeviceCount</span></span>|<span data-ttu-id="55b7a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="55b7a-140">Int32</span></span>|<span data-ttu-id="55b7a-141">Количество устройств, которые не развернули эту дополнительную политику WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="55b7a-141">Number of Devices that have failed to deploy this WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="55b7a-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="55b7a-142">Response</span></span>
<span data-ttu-id="55b7a-143">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="55b7a-143">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55b7a-144">Пример</span><span class="sxs-lookup"><span data-stu-id="55b7a-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="55b7a-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="55b7a-145">Request</span></span>
<span data-ttu-id="55b7a-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55b7a-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="55b7a-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="55b7a-147">Response</span></span>
<span data-ttu-id="55b7a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55b7a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




