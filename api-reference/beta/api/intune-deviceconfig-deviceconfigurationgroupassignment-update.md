---
title: Обновление deviceConfigurationGroupAssignment
description: Обновление свойств объекта deviceConfigurationGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2d07f58364da6b00dc0763a570dad05ac0b33644
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792893"
---
# <a name="update-deviceconfigurationgroupassignment"></a><span data-ttu-id="c1789-103">Обновление deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="c1789-103">Update deviceConfigurationGroupAssignment</span></span>

<span data-ttu-id="c1789-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1789-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1789-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1789-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1789-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1789-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1789-107">Обновление свойств объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c1789-107">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1789-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c1789-108">Prerequisites</span></span>
<span data-ttu-id="c1789-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c1789-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c1789-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1789-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1789-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1789-111">Permission type</span></span>|<span data-ttu-id="c1789-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1789-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1789-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1789-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1789-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1789-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c1789-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1789-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1789-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1789-116">Not supported.</span></span>|
|<span data-ttu-id="c1789-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1789-117">Application</span></span>|<span data-ttu-id="c1789-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1789-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1789-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1789-119">HTTP Request</span></span>
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c1789-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c1789-120">Request headers</span></span>
|<span data-ttu-id="c1789-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1789-121">Header</span></span>|<span data-ttu-id="c1789-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c1789-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1789-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1789-123">Authorization</span></span>|<span data-ttu-id="c1789-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1789-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1789-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c1789-125">Accept</span></span>|<span data-ttu-id="c1789-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1789-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1789-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c1789-127">Request body</span></span>
<span data-ttu-id="c1789-128">В тексте запроса добавьте представление объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1789-128">In the request body, supply a JSON representation for the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

<span data-ttu-id="c1789-129">В следующей таблице приведены свойства, необходимые при создании [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c1789-129">The following table shows the properties that are required when you create the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>

|<span data-ttu-id="c1789-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1789-130">Property</span></span>|<span data-ttu-id="c1789-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c1789-131">Type</span></span>|<span data-ttu-id="c1789-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c1789-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1789-133">id</span><span class="sxs-lookup"><span data-stu-id="c1789-133">id</span></span>|<span data-ttu-id="c1789-134">String</span><span class="sxs-lookup"><span data-stu-id="c1789-134">String</span></span>|<span data-ttu-id="c1789-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c1789-135">Key of the entity.</span></span>|
|<span data-ttu-id="c1789-136">таржетграупид</span><span class="sxs-lookup"><span data-stu-id="c1789-136">targetGroupId</span></span>|<span data-ttu-id="c1789-137">String</span><span class="sxs-lookup"><span data-stu-id="c1789-137">String</span></span>|<span data-ttu-id="c1789-138">Идентификатор группы AAD, на которую направляться конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="c1789-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="c1789-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="c1789-139">excludeGroup</span></span>|<span data-ttu-id="c1789-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1789-140">Boolean</span></span>|<span data-ttu-id="c1789-141">Указывает, следует ли исключить эту группу.</span><span class="sxs-lookup"><span data-stu-id="c1789-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="c1789-142">Значения по умолчанию, включаемые в группу</span><span class="sxs-lookup"><span data-stu-id="c1789-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="c1789-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1789-143">Response</span></span>
<span data-ttu-id="c1789-144">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c1789-144">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1789-145">Пример</span><span class="sxs-lookup"><span data-stu-id="c1789-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1789-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1789-146">Request</span></span>
<span data-ttu-id="c1789-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1789-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c1789-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1789-148">Response</span></span>
<span data-ttu-id="c1789-149">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="c1789-149">Here is an example of the response.</span></span> <span data-ttu-id="c1789-150">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="c1789-150">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c1789-151">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="c1789-151">All of the properties will be returned from an actual call.</span></span>
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



