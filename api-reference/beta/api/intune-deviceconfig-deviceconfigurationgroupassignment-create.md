---
title: Создание deviceConfigurationGroupAssignment
description: Создание нового объекта deviceConfigurationGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 95936153eb25d3dbf81931f090dd413dc325f126
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38083881"
---
# <a name="create-deviceconfigurationgroupassignment"></a><span data-ttu-id="a7cc5-103">Создание deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="a7cc5-103">Create deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="a7cc5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7cc5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7cc5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7cc5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7cc5-106">Создание нового объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a7cc5-106">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7cc5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a7cc5-107">Prerequisites</span></span>
<span data-ttu-id="a7cc5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7cc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7cc5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7cc5-110">Permission type</span></span>|<span data-ttu-id="a7cc5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7cc5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7cc5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7cc5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a7cc5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7cc5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a7cc5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7cc5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7cc5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7cc5-115">Not supported.</span></span>|
|<span data-ttu-id="a7cc5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7cc5-116">Application</span></span>|<span data-ttu-id="a7cc5-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7cc5-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7cc5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7cc5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="a7cc5-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a7cc5-119">Request headers</span></span>
|<span data-ttu-id="a7cc5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7cc5-120">Header</span></span>|<span data-ttu-id="a7cc5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a7cc5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7cc5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7cc5-122">Authorization</span></span>|<span data-ttu-id="a7cc5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7cc5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7cc5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a7cc5-124">Accept</span></span>|<span data-ttu-id="a7cc5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a7cc5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7cc5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7cc5-126">Request body</span></span>
<span data-ttu-id="a7cc5-127">В тексте запроса добавьте представление объекта deviceConfigurationGroupAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7cc5-127">In the request body, supply a JSON representation for the deviceConfigurationGroupAssignment object.</span></span>

<span data-ttu-id="a7cc5-128">В следующей таблице приведены свойства, необходимые при создании deviceConfigurationGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="a7cc5-128">The following table shows the properties that are required when you create the deviceConfigurationGroupAssignment.</span></span>

|<span data-ttu-id="a7cc5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7cc5-129">Property</span></span>|<span data-ttu-id="a7cc5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a7cc5-130">Type</span></span>|<span data-ttu-id="a7cc5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a7cc5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7cc5-132">id</span><span class="sxs-lookup"><span data-stu-id="a7cc5-132">id</span></span>|<span data-ttu-id="a7cc5-133">String</span><span class="sxs-lookup"><span data-stu-id="a7cc5-133">String</span></span>|<span data-ttu-id="a7cc5-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a7cc5-134">Key of the entity.</span></span>|
|<span data-ttu-id="a7cc5-135">таржетграупид</span><span class="sxs-lookup"><span data-stu-id="a7cc5-135">targetGroupId</span></span>|<span data-ttu-id="a7cc5-136">String</span><span class="sxs-lookup"><span data-stu-id="a7cc5-136">String</span></span>|<span data-ttu-id="a7cc5-137">Идентификатор группы AAD, на которую направляться конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="a7cc5-137">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="a7cc5-138">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="a7cc5-138">excludeGroup</span></span>|<span data-ttu-id="a7cc5-139">Логический</span><span class="sxs-lookup"><span data-stu-id="a7cc5-139">Boolean</span></span>|<span data-ttu-id="a7cc5-140">Указывает, следует ли исключить эту группу.</span><span class="sxs-lookup"><span data-stu-id="a7cc5-140">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="a7cc5-141">Значения по умолчанию, включаемые в группу</span><span class="sxs-lookup"><span data-stu-id="a7cc5-141">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="a7cc5-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7cc5-142">Response</span></span>
<span data-ttu-id="a7cc5-143">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a7cc5-143">If successful, this method returns a `201 Created` response code and a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7cc5-144">Пример</span><span class="sxs-lookup"><span data-stu-id="a7cc5-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7cc5-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7cc5-145">Request</span></span>
<span data-ttu-id="a7cc5-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7cc5-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 146

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

### <a name="response"></a><span data-ttu-id="a7cc5-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7cc5-147">Response</span></span>
<span data-ttu-id="a7cc5-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7cc5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 195

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```






