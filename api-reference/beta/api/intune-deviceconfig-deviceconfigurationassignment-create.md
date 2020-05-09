---
title: Создание объекта deviceConfigurationAssignment
description: Создание объекта deviceConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f45636a129ad8a193ef0cdd2f2d73cf20dad611
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178670"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="16cc1-103">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="16cc1-103">Create deviceConfigurationAssignment</span></span>

<span data-ttu-id="16cc1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16cc1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16cc1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16cc1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16cc1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16cc1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16cc1-107">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="16cc1-107">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16cc1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="16cc1-108">Prerequisites</span></span>
<span data-ttu-id="16cc1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16cc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16cc1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16cc1-111">Permission type</span></span>|<span data-ttu-id="16cc1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="16cc1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16cc1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16cc1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16cc1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16cc1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16cc1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16cc1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16cc1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16cc1-116">Not supported.</span></span>|
|<span data-ttu-id="16cc1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16cc1-117">Application</span></span>|<span data-ttu-id="16cc1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16cc1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16cc1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16cc1-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="16cc1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="16cc1-120">Request headers</span></span>
|<span data-ttu-id="16cc1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16cc1-121">Header</span></span>|<span data-ttu-id="16cc1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="16cc1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16cc1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16cc1-123">Authorization</span></span>|<span data-ttu-id="16cc1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16cc1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16cc1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="16cc1-125">Accept</span></span>|<span data-ttu-id="16cc1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16cc1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16cc1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16cc1-127">Request body</span></span>
<span data-ttu-id="16cc1-128">В тексте запроса добавьте представление объекта deviceConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16cc1-128">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="16cc1-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="16cc1-129">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="16cc1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="16cc1-130">Property</span></span>|<span data-ttu-id="16cc1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="16cc1-131">Type</span></span>|<span data-ttu-id="16cc1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="16cc1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16cc1-133">id</span><span class="sxs-lookup"><span data-stu-id="16cc1-133">id</span></span>|<span data-ttu-id="16cc1-134">Строка</span><span class="sxs-lookup"><span data-stu-id="16cc1-134">String</span></span>|<span data-ttu-id="16cc1-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="16cc1-135">The key of the assignment.</span></span>|
|<span data-ttu-id="16cc1-136">target</span><span class="sxs-lookup"><span data-stu-id="16cc1-136">target</span></span>|[<span data-ttu-id="16cc1-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="16cc1-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="16cc1-138">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="16cc1-138">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="16cc1-139">source</span><span class="sxs-lookup"><span data-stu-id="16cc1-139">source</span></span>|[<span data-ttu-id="16cc1-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="16cc1-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="16cc1-141">Источник назначения для конфигурации устройства, Direct или в упаковке/политике.</span><span class="sxs-lookup"><span data-stu-id="16cc1-141">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="16cc1-142">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16cc1-142">This property is read-only.</span></span> <span data-ttu-id="16cc1-143">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="16cc1-143">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="16cc1-144">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="16cc1-144">sourceId</span></span>|<span data-ttu-id="16cc1-145">Строка</span><span class="sxs-lookup"><span data-stu-id="16cc1-145">String</span></span>|<span data-ttu-id="16cc1-146">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="16cc1-146">The identifier of the source of the assignment.</span></span> <span data-ttu-id="16cc1-147">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16cc1-147">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="16cc1-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="16cc1-148">Response</span></span>
<span data-ttu-id="16cc1-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16cc1-149">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16cc1-150">Пример</span><span class="sxs-lookup"><span data-stu-id="16cc1-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="16cc1-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="16cc1-151">Request</span></span>
<span data-ttu-id="16cc1-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16cc1-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
Content-type: application/json
Content-length: 218

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="16cc1-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="16cc1-153">Response</span></span>
<span data-ttu-id="16cc1-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16cc1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 267

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```



