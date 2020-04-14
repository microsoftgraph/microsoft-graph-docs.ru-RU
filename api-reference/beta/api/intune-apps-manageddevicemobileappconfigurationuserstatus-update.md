---
title: Обновление объекта managedDeviceMobileAppConfigurationUserStatus
description: Обновление свойств объекта managedDeviceMobileAppConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4816581d58f6a5efa325bb5f3cebcd00dcfacf60
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43415930"
---
# <a name="update-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="cae84-103">Обновление объекта managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="cae84-103">Update managedDeviceMobileAppConfigurationUserStatus</span></span>

<span data-ttu-id="cae84-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cae84-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cae84-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae84-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cae84-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cae84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cae84-107">Обновление свойств объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="cae84-107">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cae84-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cae84-108">Prerequisites</span></span>
<span data-ttu-id="cae84-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cae84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cae84-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cae84-111">Permission type</span></span>|<span data-ttu-id="cae84-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cae84-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cae84-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cae84-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cae84-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cae84-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cae84-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cae84-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cae84-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae84-116">Not supported.</span></span>|
|<span data-ttu-id="cae84-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cae84-117">Application</span></span>|<span data-ttu-id="cae84-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cae84-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cae84-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cae84-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="cae84-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cae84-120">Request headers</span></span>
|<span data-ttu-id="cae84-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cae84-121">Header</span></span>|<span data-ttu-id="cae84-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cae84-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cae84-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cae84-123">Authorization</span></span>|<span data-ttu-id="cae84-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cae84-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cae84-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cae84-125">Accept</span></span>|<span data-ttu-id="cae84-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cae84-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cae84-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cae84-127">Request body</span></span>
<span data-ttu-id="cae84-128">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cae84-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="cae84-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="cae84-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="cae84-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cae84-130">Property</span></span>|<span data-ttu-id="cae84-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cae84-131">Type</span></span>|<span data-ttu-id="cae84-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cae84-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cae84-133">id</span><span class="sxs-lookup"><span data-stu-id="cae84-133">id</span></span>|<span data-ttu-id="cae84-134">Строка</span><span class="sxs-lookup"><span data-stu-id="cae84-134">String</span></span>|<span data-ttu-id="cae84-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cae84-135">Key of the entity.</span></span>|
|<span data-ttu-id="cae84-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="cae84-136">userDisplayName</span></span>|<span data-ttu-id="cae84-137">String</span><span class="sxs-lookup"><span data-stu-id="cae84-137">String</span></span>|<span data-ttu-id="cae84-138">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="cae84-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="cae84-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="cae84-139">devicesCount</span></span>|<span data-ttu-id="cae84-140">Int32</span><span class="sxs-lookup"><span data-stu-id="cae84-140">Int32</span></span>|<span data-ttu-id="cae84-141">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="cae84-141">Devices count for that user.</span></span>|
|<span data-ttu-id="cae84-142">status</span><span class="sxs-lookup"><span data-stu-id="cae84-142">status</span></span>|[<span data-ttu-id="cae84-143">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="cae84-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="cae84-144">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="cae84-144">Compliance status of the policy report.</span></span> <span data-ttu-id="cae84-145">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="cae84-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="cae84-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="cae84-146">lastReportedDateTime</span></span>|<span data-ttu-id="cae84-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cae84-147">DateTimeOffset</span></span>|<span data-ttu-id="cae84-148">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="cae84-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="cae84-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cae84-149">userPrincipalName</span></span>|<span data-ttu-id="cae84-150">String</span><span class="sxs-lookup"><span data-stu-id="cae84-150">String</span></span>|<span data-ttu-id="cae84-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="cae84-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="cae84-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="cae84-152">Response</span></span>
<span data-ttu-id="cae84-153">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cae84-153">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cae84-154">Пример</span><span class="sxs-lookup"><span data-stu-id="cae84-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="cae84-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="cae84-155">Request</span></span>
<span data-ttu-id="cae84-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cae84-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cae84-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="cae84-157">Response</span></span>
<span data-ttu-id="cae84-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cae84-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



