---
title: Обновление объекта managedDeviceMobileAppConfigurationUserStatus
description: Обновление свойств объекта managedDeviceMobileAppConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8ef878eb9816576e55c16074e8983c9d7895e961
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140107"
---
# <a name="update-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="0f6c0-103">Обновление объекта managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="0f6c0-103">Update managedDeviceMobileAppConfigurationUserStatus</span></span>

<span data-ttu-id="0f6c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f6c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f6c0-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f6c0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f6c0-107">Обновление свойств объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="0f6c0-107">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f6c0-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0f6c0-108">Prerequisites</span></span>
<span data-ttu-id="0f6c0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f6c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f6c0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f6c0-111">Permission type</span></span>|<span data-ttu-id="0f6c0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f6c0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f6c0-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f6c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f6c0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f6c0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0f6c0-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f6c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f6c0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-116">Not supported.</span></span>|
|<span data-ttu-id="0f6c0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0f6c0-117">Application</span></span>|<span data-ttu-id="0f6c0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f6c0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f6c0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f6c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="0f6c0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0f6c0-120">Request headers</span></span>
|<span data-ttu-id="0f6c0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0f6c0-121">Header</span></span>|<span data-ttu-id="0f6c0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0f6c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f6c0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f6c0-123">Authorization</span></span>|<span data-ttu-id="0f6c0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f6c0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0f6c0-125">Accept</span></span>|<span data-ttu-id="0f6c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f6c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f6c0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f6c0-127">Request body</span></span>
<span data-ttu-id="0f6c0-128">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="0f6c0-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="0f6c0-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="0f6c0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f6c0-130">Property</span></span>|<span data-ttu-id="0f6c0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0f6c0-131">Type</span></span>|<span data-ttu-id="0f6c0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0f6c0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f6c0-133">id</span><span class="sxs-lookup"><span data-stu-id="0f6c0-133">id</span></span>|<span data-ttu-id="0f6c0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0f6c0-134">String</span></span>|<span data-ttu-id="0f6c0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-135">Key of the entity.</span></span>|
|<span data-ttu-id="0f6c0-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="0f6c0-136">userDisplayName</span></span>|<span data-ttu-id="0f6c0-137">String</span><span class="sxs-lookup"><span data-stu-id="0f6c0-137">String</span></span>|<span data-ttu-id="0f6c0-138">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="0f6c0-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="0f6c0-139">devicesCount</span></span>|<span data-ttu-id="0f6c0-140">Int32</span><span class="sxs-lookup"><span data-stu-id="0f6c0-140">Int32</span></span>|<span data-ttu-id="0f6c0-141">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-141">Devices count for that user.</span></span>|
|<span data-ttu-id="0f6c0-142">status</span><span class="sxs-lookup"><span data-stu-id="0f6c0-142">status</span></span>|[<span data-ttu-id="0f6c0-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="0f6c0-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="0f6c0-144">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-144">Compliance status of the policy report.</span></span> <span data-ttu-id="0f6c0-145">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="0f6c0-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f6c0-146">lastReportedDateTime</span></span>|<span data-ttu-id="0f6c0-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f6c0-147">DateTimeOffset</span></span>|<span data-ttu-id="0f6c0-148">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="0f6c0-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0f6c0-149">userPrincipalName</span></span>|<span data-ttu-id="0f6c0-150">String</span><span class="sxs-lookup"><span data-stu-id="0f6c0-150">String</span></span>|<span data-ttu-id="0f6c0-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="0f6c0-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f6c0-152">Response</span></span>
<span data-ttu-id="0f6c0-153">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-153">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f6c0-154">Пример</span><span class="sxs-lookup"><span data-stu-id="0f6c0-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f6c0-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f6c0-155">Request</span></span>
<span data-ttu-id="0f6c0-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="0f6c0-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f6c0-157">Response</span></span>
<span data-ttu-id="0f6c0-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0f6c0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "id": "44960944-0944-4496-4409-964444099644",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




