---
title: Создание deviceConfigurationGroupAssignment
description: Создание нового объекта deviceConfigurationGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 380da320217a63ccf115bc98f4b75ec6d844de0e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449147"
---
# <a name="create-deviceconfigurationgroupassignment"></a><span data-ttu-id="f479e-103">Создание deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="f479e-103">Create deviceConfigurationGroupAssignment</span></span>

<span data-ttu-id="f479e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f479e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f479e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f479e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f479e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f479e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f479e-107">Создание нового объекта [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="f479e-107">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f479e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f479e-108">Prerequisites</span></span>
<span data-ttu-id="f479e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f479e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f479e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f479e-111">Permission type</span></span>|<span data-ttu-id="f479e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f479e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f479e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f479e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f479e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f479e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f479e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f479e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f479e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f479e-116">Not supported.</span></span>|
|<span data-ttu-id="f479e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f479e-117">Application</span></span>|<span data-ttu-id="f479e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f479e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f479e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f479e-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="f479e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f479e-120">Request headers</span></span>
|<span data-ttu-id="f479e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f479e-121">Header</span></span>|<span data-ttu-id="f479e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f479e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f479e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f479e-123">Authorization</span></span>|<span data-ttu-id="f479e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f479e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f479e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f479e-125">Accept</span></span>|<span data-ttu-id="f479e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f479e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f479e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f479e-127">Request body</span></span>
<span data-ttu-id="f479e-128">В тексте запроса добавьте представление объекта deviceConfigurationGroupAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f479e-128">In the request body, supply a JSON representation for the deviceConfigurationGroupAssignment object.</span></span>

<span data-ttu-id="f479e-129">В следующей таблице приведены свойства, необходимые при создании deviceConfigurationGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="f479e-129">The following table shows the properties that are required when you create the deviceConfigurationGroupAssignment.</span></span>

|<span data-ttu-id="f479e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f479e-130">Property</span></span>|<span data-ttu-id="f479e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f479e-131">Type</span></span>|<span data-ttu-id="f479e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f479e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f479e-133">id</span><span class="sxs-lookup"><span data-stu-id="f479e-133">id</span></span>|<span data-ttu-id="f479e-134">String</span><span class="sxs-lookup"><span data-stu-id="f479e-134">String</span></span>|<span data-ttu-id="f479e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f479e-135">Key of the entity.</span></span>|
|<span data-ttu-id="f479e-136">таржетграупид</span><span class="sxs-lookup"><span data-stu-id="f479e-136">targetGroupId</span></span>|<span data-ttu-id="f479e-137">String</span><span class="sxs-lookup"><span data-stu-id="f479e-137">String</span></span>|<span data-ttu-id="f479e-138">Идентификатор группы AAD, на которую направляться конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="f479e-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="f479e-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="f479e-139">excludeGroup</span></span>|<span data-ttu-id="f479e-140">Логический</span><span class="sxs-lookup"><span data-stu-id="f479e-140">Boolean</span></span>|<span data-ttu-id="f479e-141">Указывает, следует ли исключить эту группу.</span><span class="sxs-lookup"><span data-stu-id="f479e-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="f479e-142">Значения по умолчанию, включаемые в группу</span><span class="sxs-lookup"><span data-stu-id="f479e-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="f479e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="f479e-143">Response</span></span>
<span data-ttu-id="f479e-144">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f479e-144">If successful, this method returns a `201 Created` response code and a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f479e-145">Пример</span><span class="sxs-lookup"><span data-stu-id="f479e-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="f479e-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="f479e-146">Request</span></span>
<span data-ttu-id="f479e-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f479e-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f479e-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="f479e-148">Response</span></span>
<span data-ttu-id="f479e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f479e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





