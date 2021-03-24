---
title: Создание deviceConfigurationGroupAssignment
description: Создайте новый объект deviceConfigurationGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 23cddf27e1622dcf6a661f8fcbbf24f49b436aba
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128077"
---
# <a name="create-deviceconfigurationgroupassignment"></a><span data-ttu-id="a035d-103">Создание deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="a035d-103">Create deviceConfigurationGroupAssignment</span></span>

<span data-ttu-id="a035d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a035d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a035d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a035d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a035d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a035d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a035d-107">Создайте новый [объект deviceConfigurationGroupAssignment.](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a035d-107">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a035d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a035d-108">Prerequisites</span></span>
<span data-ttu-id="a035d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a035d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a035d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a035d-111">Permission type</span></span>|<span data-ttu-id="a035d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a035d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a035d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a035d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a035d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a035d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a035d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a035d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a035d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a035d-116">Not supported.</span></span>|
|<span data-ttu-id="a035d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a035d-117">Application</span></span>|<span data-ttu-id="a035d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a035d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a035d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a035d-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="a035d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a035d-120">Request headers</span></span>
|<span data-ttu-id="a035d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a035d-121">Header</span></span>|<span data-ttu-id="a035d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a035d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a035d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a035d-123">Authorization</span></span>|<span data-ttu-id="a035d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a035d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a035d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a035d-125">Accept</span></span>|<span data-ttu-id="a035d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a035d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a035d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a035d-127">Request body</span></span>
<span data-ttu-id="a035d-128">В теле запроса поставляем представление JSON для объекта deviceConfigurationGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="a035d-128">In the request body, supply a JSON representation for the deviceConfigurationGroupAssignment object.</span></span>

<span data-ttu-id="a035d-129">В следующей таблице показаны свойства, необходимые при создании устройстваConfigurationGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="a035d-129">The following table shows the properties that are required when you create the deviceConfigurationGroupAssignment.</span></span>

|<span data-ttu-id="a035d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a035d-130">Property</span></span>|<span data-ttu-id="a035d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a035d-131">Type</span></span>|<span data-ttu-id="a035d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a035d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a035d-133">id</span><span class="sxs-lookup"><span data-stu-id="a035d-133">id</span></span>|<span data-ttu-id="a035d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a035d-134">String</span></span>|<span data-ttu-id="a035d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a035d-135">Key of the entity.</span></span>|
|<span data-ttu-id="a035d-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="a035d-136">targetGroupId</span></span>|<span data-ttu-id="a035d-137">Строка</span><span class="sxs-lookup"><span data-stu-id="a035d-137">String</span></span>|<span data-ttu-id="a035d-138">Id группы AAD, на который ориентирована конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="a035d-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="a035d-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="a035d-139">excludeGroup</span></span>|<span data-ttu-id="a035d-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="a035d-140">Boolean</span></span>|<span data-ttu-id="a035d-141">Указывает, следует ли исключить эту группу.</span><span class="sxs-lookup"><span data-stu-id="a035d-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="a035d-142">По умолчанию, которые следует включить в группу</span><span class="sxs-lookup"><span data-stu-id="a035d-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="a035d-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="a035d-143">Response</span></span>
<span data-ttu-id="a035d-144">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a035d-144">If successful, this method returns a `201 Created` response code and a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a035d-145">Пример</span><span class="sxs-lookup"><span data-stu-id="a035d-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="a035d-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="a035d-146">Request</span></span>
<span data-ttu-id="a035d-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a035d-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a035d-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="a035d-148">Response</span></span>
<span data-ttu-id="a035d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a035d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




