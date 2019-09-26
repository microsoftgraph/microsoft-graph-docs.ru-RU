---
title: Создание объекта deviceConfigurationAssignment
description: Создание объекта deviceConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cb967a3e365b4b3a2347f93f6fa72cc9784091ca
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37174888"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="871fa-103">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="871fa-103">Create deviceConfigurationAssignment</span></span>

> <span data-ttu-id="871fa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="871fa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="871fa-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="871fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="871fa-106">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="871fa-106">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="871fa-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="871fa-107">Prerequisites</span></span>
<span data-ttu-id="871fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="871fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="871fa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="871fa-110">Permission type</span></span>|<span data-ttu-id="871fa-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="871fa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="871fa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="871fa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="871fa-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="871fa-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="871fa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="871fa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="871fa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="871fa-115">Not supported.</span></span>|
|<span data-ttu-id="871fa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="871fa-116">Application</span></span>|<span data-ttu-id="871fa-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="871fa-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="871fa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="871fa-118">HTTP Request</span></span>
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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="871fa-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="871fa-119">Request headers</span></span>
|<span data-ttu-id="871fa-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="871fa-120">Header</span></span>|<span data-ttu-id="871fa-121">Значение</span><span class="sxs-lookup"><span data-stu-id="871fa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="871fa-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="871fa-122">Authorization</span></span>|<span data-ttu-id="871fa-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="871fa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="871fa-124">Accept</span><span class="sxs-lookup"><span data-stu-id="871fa-124">Accept</span></span>|<span data-ttu-id="871fa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="871fa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="871fa-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="871fa-126">Request body</span></span>
<span data-ttu-id="871fa-127">В тексте запроса добавьте представление объекта deviceConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="871fa-127">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="871fa-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="871fa-128">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="871fa-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="871fa-129">Property</span></span>|<span data-ttu-id="871fa-130">Тип</span><span class="sxs-lookup"><span data-stu-id="871fa-130">Type</span></span>|<span data-ttu-id="871fa-131">Описание</span><span class="sxs-lookup"><span data-stu-id="871fa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="871fa-132">id</span><span class="sxs-lookup"><span data-stu-id="871fa-132">id</span></span>|<span data-ttu-id="871fa-133">String</span><span class="sxs-lookup"><span data-stu-id="871fa-133">String</span></span>|<span data-ttu-id="871fa-134">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="871fa-134">The key of the assignment.</span></span>|
|<span data-ttu-id="871fa-135">target</span><span class="sxs-lookup"><span data-stu-id="871fa-135">target</span></span>|[<span data-ttu-id="871fa-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="871fa-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="871fa-137">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="871fa-137">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="871fa-138">source</span><span class="sxs-lookup"><span data-stu-id="871fa-138">source</span></span>|[<span data-ttu-id="871fa-139">девицеандаппманажементассигнментсаурце</span><span class="sxs-lookup"><span data-stu-id="871fa-139">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="871fa-140">Источник назначения для конфигурации устройства, Direct или в упаковке/политике.</span><span class="sxs-lookup"><span data-stu-id="871fa-140">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="871fa-141">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="871fa-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="871fa-142">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="871fa-142">sourceId</span></span>|<span data-ttu-id="871fa-143">String.</span><span class="sxs-lookup"><span data-stu-id="871fa-143">String</span></span>|<span data-ttu-id="871fa-144">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="871fa-144">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="871fa-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="871fa-145">Response</span></span>
<span data-ttu-id="871fa-146">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="871fa-146">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="871fa-147">Пример</span><span class="sxs-lookup"><span data-stu-id="871fa-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="871fa-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="871fa-148">Request</span></span>
<span data-ttu-id="871fa-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="871fa-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
Content-type: application/json
Content-length: 230

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="871fa-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="871fa-150">Response</span></span>
<span data-ttu-id="871fa-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="871fa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 279

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```




