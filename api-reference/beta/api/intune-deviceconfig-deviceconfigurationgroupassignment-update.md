---
title: Обновление deviceConfigurationGroupAssignment
description: Обновление свойств объекта deviceConfigurationGroupAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f349047b9039ce6db1fed0af93af5e967aac132c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42753637"
---
# <a name="update-deviceconfigurationgroupassignment"></a><span data-ttu-id="d2d19-103">Обновление deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="d2d19-103">Update deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="d2d19-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2d19-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2d19-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2d19-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2d19-106">Обновление свойств объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="d2d19-106">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2d19-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d2d19-107">Prerequisites</span></span>
<span data-ttu-id="d2d19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2d19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2d19-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2d19-110">Permission type</span></span>|<span data-ttu-id="d2d19-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2d19-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2d19-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2d19-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d2d19-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2d19-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d2d19-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2d19-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2d19-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2d19-115">Not supported.</span></span>|
|<span data-ttu-id="d2d19-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d2d19-116">Application</span></span>|<span data-ttu-id="d2d19-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2d19-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2d19-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2d19-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d2d19-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d2d19-119">Request headers</span></span>
|<span data-ttu-id="d2d19-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2d19-120">Header</span></span>|<span data-ttu-id="d2d19-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d2d19-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2d19-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2d19-122">Authorization</span></span>|<span data-ttu-id="d2d19-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2d19-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2d19-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d2d19-124">Accept</span></span>|<span data-ttu-id="d2d19-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d2d19-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2d19-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2d19-126">Request body</span></span>
<span data-ttu-id="d2d19-127">В тексте запроса добавьте представление объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2d19-127">In the request body, supply a JSON representation for the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

<span data-ttu-id="d2d19-128">В следующей таблице приведены свойства, необходимые при создании [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d2d19-128">The following table shows the properties that are required when you create the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>

|<span data-ttu-id="d2d19-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2d19-129">Property</span></span>|<span data-ttu-id="d2d19-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d2d19-130">Type</span></span>|<span data-ttu-id="d2d19-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d2d19-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2d19-132">id</span><span class="sxs-lookup"><span data-stu-id="d2d19-132">id</span></span>|<span data-ttu-id="d2d19-133">String</span><span class="sxs-lookup"><span data-stu-id="d2d19-133">String</span></span>|<span data-ttu-id="d2d19-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d2d19-134">Key of the entity.</span></span>|
|<span data-ttu-id="d2d19-135">таржетграупид</span><span class="sxs-lookup"><span data-stu-id="d2d19-135">targetGroupId</span></span>|<span data-ttu-id="d2d19-136">String</span><span class="sxs-lookup"><span data-stu-id="d2d19-136">String</span></span>|<span data-ttu-id="d2d19-137">Идентификатор группы AAD, на которую направляться конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="d2d19-137">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="d2d19-138">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="d2d19-138">excludeGroup</span></span>|<span data-ttu-id="d2d19-139">Логический</span><span class="sxs-lookup"><span data-stu-id="d2d19-139">Boolean</span></span>|<span data-ttu-id="d2d19-140">Указывает, следует ли исключить эту группу.</span><span class="sxs-lookup"><span data-stu-id="d2d19-140">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="d2d19-141">Значения по умолчанию, включаемые в группу</span><span class="sxs-lookup"><span data-stu-id="d2d19-141">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="d2d19-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2d19-142">Response</span></span>
<span data-ttu-id="d2d19-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2d19-143">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2d19-144">Пример</span><span class="sxs-lookup"><span data-stu-id="d2d19-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2d19-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2d19-145">Request</span></span>
<span data-ttu-id="d2d19-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2d19-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
Content-type: application/json
Content-length: 146

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

### <a name="response"></a><span data-ttu-id="d2d19-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2d19-147">Response</span></span>
<span data-ttu-id="d2d19-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2d19-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 195

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```




