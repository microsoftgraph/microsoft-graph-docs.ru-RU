---
title: Обновление объекта managedDeviceMobileAppConfigurationUserStatus
description: Обновление свойств объекта managedDeviceMobileAppConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0b1b0cfab88b44adaaa95b2b519ce5cc34c94d5b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754205"
---
# <a name="update-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="a3e3f-103">Обновление объекта managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="a3e3f-103">Update managedDeviceMobileAppConfigurationUserStatus</span></span>

<span data-ttu-id="a3e3f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3e3f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3e3f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3e3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3e3f-106">Обновление свойств объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a3e3f-106">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3e3f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a3e3f-107">Prerequisites</span></span>
<span data-ttu-id="a3e3f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3e3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3e3f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3e3f-110">Permission type</span></span>|<span data-ttu-id="a3e3f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3e3f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3e3f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3e3f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3e3f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3e3f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a3e3f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3e3f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3e3f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3e3f-115">Not supported.</span></span>|
|<span data-ttu-id="a3e3f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="a3e3f-116">Application</span></span>|<span data-ttu-id="a3e3f-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3e3f-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3e3f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3e3f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="a3e3f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a3e3f-119">Request headers</span></span>
|<span data-ttu-id="a3e3f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3e3f-120">Header</span></span>|<span data-ttu-id="a3e3f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a3e3f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3e3f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3e3f-122">Authorization</span></span>|<span data-ttu-id="a3e3f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3e3f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3e3f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a3e3f-124">Accept</span></span>|<span data-ttu-id="a3e3f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a3e3f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3e3f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3e3f-126">Request body</span></span>
<span data-ttu-id="a3e3f-127">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3e3f-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="a3e3f-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a3e3f-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="a3e3f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3e3f-129">Property</span></span>|<span data-ttu-id="a3e3f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a3e3f-130">Type</span></span>|<span data-ttu-id="a3e3f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a3e3f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3e3f-132">id</span><span class="sxs-lookup"><span data-stu-id="a3e3f-132">id</span></span>|<span data-ttu-id="a3e3f-133">String</span><span class="sxs-lookup"><span data-stu-id="a3e3f-133">String</span></span>|<span data-ttu-id="a3e3f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a3e3f-134">Key of the entity.</span></span>|
|<span data-ttu-id="a3e3f-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="a3e3f-135">userDisplayName</span></span>|<span data-ttu-id="a3e3f-136">String</span><span class="sxs-lookup"><span data-stu-id="a3e3f-136">String</span></span>|<span data-ttu-id="a3e3f-137">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="a3e3f-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="a3e3f-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="a3e3f-138">devicesCount</span></span>|<span data-ttu-id="a3e3f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a3e3f-139">Int32</span></span>|<span data-ttu-id="a3e3f-140">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="a3e3f-140">Devices count for that user.</span></span>|
|<span data-ttu-id="a3e3f-141">status</span><span class="sxs-lookup"><span data-stu-id="a3e3f-141">status</span></span>|[<span data-ttu-id="a3e3f-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a3e3f-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a3e3f-143">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="a3e3f-143">Compliance status of the policy report.</span></span> <span data-ttu-id="a3e3f-144">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a3e3f-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a3e3f-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3e3f-145">lastReportedDateTime</span></span>|<span data-ttu-id="a3e3f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3e3f-146">DateTimeOffset</span></span>|<span data-ttu-id="a3e3f-147">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="a3e3f-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="a3e3f-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a3e3f-148">userPrincipalName</span></span>|<span data-ttu-id="a3e3f-149">String</span><span class="sxs-lookup"><span data-stu-id="a3e3f-149">String</span></span>|<span data-ttu-id="a3e3f-150">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="a3e3f-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="a3e3f-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3e3f-151">Response</span></span>
<span data-ttu-id="a3e3f-152">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a3e3f-152">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3e3f-153">Пример</span><span class="sxs-lookup"><span data-stu-id="a3e3f-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3e3f-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3e3f-154">Request</span></span>
<span data-ttu-id="a3e3f-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3e3f-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
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

### <a name="response"></a><span data-ttu-id="a3e3f-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3e3f-156">Response</span></span>
<span data-ttu-id="a3e3f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3e3f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




