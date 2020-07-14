---
title: Создание объекта deviceConfigurationAssignment
description: Создание объекта deviceConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6c4ca1a95833f02f938365a48081225194e2742b
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123234"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="3f4b8-103">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="3f4b8-103">Create deviceConfigurationAssignment</span></span>

<span data-ttu-id="3f4b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f4b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f4b8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f4b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f4b8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f4b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f4b8-107">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3f4b8-107">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f4b8-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3f4b8-108">Prerequisites</span></span>
<span data-ttu-id="3f4b8-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="3f4b8-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3f4b8-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f4b8-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f4b8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f4b8-111">Permission type</span></span>|<span data-ttu-id="3f4b8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f4b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f4b8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f4b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f4b8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f4b8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3f4b8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f4b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f4b8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f4b8-116">Not supported.</span></span>|
|<span data-ttu-id="3f4b8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f4b8-117">Application</span></span>|<span data-ttu-id="3f4b8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f4b8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f4b8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f4b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="3f4b8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3f4b8-120">Request headers</span></span>
|<span data-ttu-id="3f4b8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f4b8-121">Header</span></span>|<span data-ttu-id="3f4b8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3f4b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f4b8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f4b8-123">Authorization</span></span>|<span data-ttu-id="3f4b8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f4b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f4b8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3f4b8-125">Accept</span></span>|<span data-ttu-id="3f4b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f4b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f4b8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f4b8-127">Request body</span></span>
<span data-ttu-id="3f4b8-128">В тексте запроса добавьте представление объекта deviceConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f4b8-128">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="3f4b8-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="3f4b8-129">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="3f4b8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f4b8-130">Property</span></span>|<span data-ttu-id="3f4b8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3f4b8-131">Type</span></span>|<span data-ttu-id="3f4b8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3f4b8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f4b8-133">id</span><span class="sxs-lookup"><span data-stu-id="3f4b8-133">id</span></span>|<span data-ttu-id="3f4b8-134">String</span><span class="sxs-lookup"><span data-stu-id="3f4b8-134">String</span></span>|<span data-ttu-id="3f4b8-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="3f4b8-135">The key of the assignment.</span></span>|
|<span data-ttu-id="3f4b8-136">target</span><span class="sxs-lookup"><span data-stu-id="3f4b8-136">target</span></span>|[<span data-ttu-id="3f4b8-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3f4b8-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3f4b8-138">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="3f4b8-138">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="3f4b8-139">source</span><span class="sxs-lookup"><span data-stu-id="3f4b8-139">source</span></span>|[<span data-ttu-id="3f4b8-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="3f4b8-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="3f4b8-141">Источник назначения для конфигурации устройства, Direct или в упаковке/политике.</span><span class="sxs-lookup"><span data-stu-id="3f4b8-141">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="3f4b8-142">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f4b8-142">This property is read-only.</span></span> <span data-ttu-id="3f4b8-143">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="3f4b8-143">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="3f4b8-144">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="3f4b8-144">sourceId</span></span>|<span data-ttu-id="3f4b8-145">String</span><span class="sxs-lookup"><span data-stu-id="3f4b8-145">String</span></span>|<span data-ttu-id="3f4b8-146">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="3f4b8-146">The identifier of the source of the assignment.</span></span> <span data-ttu-id="3f4b8-147">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f4b8-147">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="3f4b8-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f4b8-148">Response</span></span>
<span data-ttu-id="3f4b8-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3f4b8-149">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f4b8-150">Пример</span><span class="sxs-lookup"><span data-stu-id="3f4b8-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f4b8-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f4b8-151">Request</span></span>
<span data-ttu-id="3f4b8-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f4b8-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
Content-type: application/json
Content-length: 385

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="3f4b8-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f4b8-153">Response</span></span>
<span data-ttu-id="3f4b8-154">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="3f4b8-154">Here is an example of the response.</span></span> <span data-ttu-id="3f4b8-155">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="3f4b8-155">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3f4b8-156">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="3f4b8-156">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 434

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```



