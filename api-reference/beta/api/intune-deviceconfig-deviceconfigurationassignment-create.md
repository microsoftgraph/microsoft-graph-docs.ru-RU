---
title: Создание объекта deviceConfigurationAssignment
description: Создание объекта deviceConfigurationAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6d4fb0aa58e899ff9e60d7ddd9f3ec705c1ca0a1
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534164"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="a129d-103">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a129d-103">Create deviceConfigurationAssignment</span></span>

> <span data-ttu-id="a129d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a129d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a129d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a129d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a129d-106">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a129d-106">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a129d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a129d-107">Prerequisites</span></span>
<span data-ttu-id="a129d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a129d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a129d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a129d-110">Permission type</span></span>|<span data-ttu-id="a129d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a129d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a129d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a129d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a129d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a129d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a129d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a129d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a129d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a129d-115">Not supported.</span></span>|
|<span data-ttu-id="a129d-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="a129d-116">Application</span></span>|<span data-ttu-id="a129d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a129d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a129d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a129d-118">HTTP Request</span></span>
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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a129d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a129d-119">Request headers</span></span>
|<span data-ttu-id="a129d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a129d-120">Header</span></span>|<span data-ttu-id="a129d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a129d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a129d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a129d-122">Authorization</span></span>|<span data-ttu-id="a129d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a129d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a129d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a129d-124">Accept</span></span>|<span data-ttu-id="a129d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a129d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a129d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a129d-126">Request body</span></span>
<span data-ttu-id="a129d-127">В тексте запроса добавьте представление объекта deviceConfigurationAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a129d-127">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="a129d-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="a129d-128">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="a129d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a129d-129">Property</span></span>|<span data-ttu-id="a129d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a129d-130">Type</span></span>|<span data-ttu-id="a129d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a129d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a129d-132">id</span><span class="sxs-lookup"><span data-stu-id="a129d-132">id</span></span>|<span data-ttu-id="a129d-133">String</span><span class="sxs-lookup"><span data-stu-id="a129d-133">String</span></span>|<span data-ttu-id="a129d-134">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="a129d-134">The key of the assignment.</span></span>|
|<span data-ttu-id="a129d-135">target</span><span class="sxs-lookup"><span data-stu-id="a129d-135">target</span></span>|[<span data-ttu-id="a129d-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a129d-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a129d-137">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="a129d-137">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="a129d-138">source</span><span class="sxs-lookup"><span data-stu-id="a129d-138">source</span></span>|[<span data-ttu-id="a129d-139">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="a129d-139">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="a129d-140">Источник назначения для конфигурации устройства, Direct или в упаковке/политике.</span><span class="sxs-lookup"><span data-stu-id="a129d-140">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="a129d-141">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a129d-141">This property is read-only.</span></span> <span data-ttu-id="a129d-142">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="a129d-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="a129d-143">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="a129d-143">sourceId</span></span>|<span data-ttu-id="a129d-144">String</span><span class="sxs-lookup"><span data-stu-id="a129d-144">String</span></span>|<span data-ttu-id="a129d-145">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="a129d-145">The identifier of the source of the assignment.</span></span> <span data-ttu-id="a129d-146">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a129d-146">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="a129d-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="a129d-147">Response</span></span>
<span data-ttu-id="a129d-148">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a129d-148">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a129d-149">Пример</span><span class="sxs-lookup"><span data-stu-id="a129d-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="a129d-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="a129d-150">Request</span></span>
<span data-ttu-id="a129d-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a129d-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a129d-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="a129d-152">Response</span></span>
<span data-ttu-id="a129d-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a129d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






