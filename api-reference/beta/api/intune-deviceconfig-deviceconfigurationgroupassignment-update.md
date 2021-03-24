---
title: Обновление устройстваConfigurationGroupAssignment
description: Обновление свойств объекта deviceConfigurationGroupAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dd267a5a634797af0d773e749d1b222f604a1739
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137506"
---
# <a name="update-deviceconfigurationgroupassignment"></a><span data-ttu-id="d37c5-103">Обновление устройстваConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="d37c5-103">Update deviceConfigurationGroupAssignment</span></span>

<span data-ttu-id="d37c5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d37c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d37c5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d37c5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d37c5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d37c5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d37c5-107">Обновление свойств объекта [deviceConfigurationGroupAssignment.](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d37c5-107">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d37c5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d37c5-108">Prerequisites</span></span>
<span data-ttu-id="d37c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d37c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d37c5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d37c5-111">Permission type</span></span>|<span data-ttu-id="d37c5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d37c5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d37c5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d37c5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d37c5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d37c5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d37c5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d37c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d37c5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d37c5-116">Not supported.</span></span>|
|<span data-ttu-id="d37c5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d37c5-117">Application</span></span>|<span data-ttu-id="d37c5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d37c5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d37c5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d37c5-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d37c5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d37c5-120">Request headers</span></span>
|<span data-ttu-id="d37c5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d37c5-121">Header</span></span>|<span data-ttu-id="d37c5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d37c5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d37c5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d37c5-123">Authorization</span></span>|<span data-ttu-id="d37c5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d37c5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d37c5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d37c5-125">Accept</span></span>|<span data-ttu-id="d37c5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d37c5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d37c5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d37c5-127">Request body</span></span>
<span data-ttu-id="d37c5-128">В теле запроса поставляем представление JSON для [объекта deviceConfigurationGroupAssignment.](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d37c5-128">In the request body, supply a JSON representation for the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

<span data-ttu-id="d37c5-129">В следующей таблице показаны свойства, необходимые при создании [устройстваConfigurationGroupAssignment.](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d37c5-129">The following table shows the properties that are required when you create the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>

|<span data-ttu-id="d37c5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d37c5-130">Property</span></span>|<span data-ttu-id="d37c5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d37c5-131">Type</span></span>|<span data-ttu-id="d37c5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d37c5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d37c5-133">id</span><span class="sxs-lookup"><span data-stu-id="d37c5-133">id</span></span>|<span data-ttu-id="d37c5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d37c5-134">String</span></span>|<span data-ttu-id="d37c5-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d37c5-135">Key of the entity.</span></span>|
|<span data-ttu-id="d37c5-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="d37c5-136">targetGroupId</span></span>|<span data-ttu-id="d37c5-137">Строка</span><span class="sxs-lookup"><span data-stu-id="d37c5-137">String</span></span>|<span data-ttu-id="d37c5-138">Id группы AAD, на который ориентирована конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="d37c5-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="d37c5-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="d37c5-139">excludeGroup</span></span>|<span data-ttu-id="d37c5-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="d37c5-140">Boolean</span></span>|<span data-ttu-id="d37c5-141">Указывает, следует ли исключить эту группу.</span><span class="sxs-lookup"><span data-stu-id="d37c5-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="d37c5-142">По умолчанию, которые следует включить в группу</span><span class="sxs-lookup"><span data-stu-id="d37c5-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="d37c5-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d37c5-143">Response</span></span>
<span data-ttu-id="d37c5-144">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d37c5-144">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d37c5-145">Пример</span><span class="sxs-lookup"><span data-stu-id="d37c5-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="d37c5-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="d37c5-146">Request</span></span>
<span data-ttu-id="d37c5-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d37c5-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d37c5-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="d37c5-148">Response</span></span>
<span data-ttu-id="d37c5-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d37c5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




