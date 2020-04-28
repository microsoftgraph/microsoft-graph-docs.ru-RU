---
title: Создание объекта managedDeviceMobileAppConfigurationUserStatus
description: Создание объекта managedDeviceMobileAppConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: afc02c9e870a78b41da2360c6626fbb9f1ec297b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43416026"
---
# <a name="create-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="50d9c-103">Создание объекта managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="50d9c-103">Create managedDeviceMobileAppConfigurationUserStatus</span></span>

<span data-ttu-id="50d9c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50d9c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50d9c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50d9c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50d9c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50d9c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50d9c-107">Создание объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="50d9c-107">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50d9c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="50d9c-108">Prerequisites</span></span>
<span data-ttu-id="50d9c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50d9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50d9c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50d9c-111">Permission type</span></span>|<span data-ttu-id="50d9c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="50d9c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50d9c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50d9c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50d9c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50d9c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="50d9c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50d9c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50d9c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50d9c-116">Not supported.</span></span>|
|<span data-ttu-id="50d9c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50d9c-117">Application</span></span>|<span data-ttu-id="50d9c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50d9c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50d9c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50d9c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="50d9c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="50d9c-120">Request headers</span></span>
|<span data-ttu-id="50d9c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50d9c-121">Header</span></span>|<span data-ttu-id="50d9c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="50d9c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50d9c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50d9c-123">Authorization</span></span>|<span data-ttu-id="50d9c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50d9c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50d9c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="50d9c-125">Accept</span></span>|<span data-ttu-id="50d9c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50d9c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50d9c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="50d9c-127">Request body</span></span>
<span data-ttu-id="50d9c-128">В тексте запроса добавьте представление объекта managedDeviceMobileAppConfigurationUserStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50d9c-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationUserStatus object.</span></span>

<span data-ttu-id="50d9c-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="50d9c-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationUserStatus.</span></span>

|<span data-ttu-id="50d9c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="50d9c-130">Property</span></span>|<span data-ttu-id="50d9c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="50d9c-131">Type</span></span>|<span data-ttu-id="50d9c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="50d9c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50d9c-133">id</span><span class="sxs-lookup"><span data-stu-id="50d9c-133">id</span></span>|<span data-ttu-id="50d9c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="50d9c-134">String</span></span>|<span data-ttu-id="50d9c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="50d9c-135">Key of the entity.</span></span>|
|<span data-ttu-id="50d9c-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="50d9c-136">userDisplayName</span></span>|<span data-ttu-id="50d9c-137">String</span><span class="sxs-lookup"><span data-stu-id="50d9c-137">String</span></span>|<span data-ttu-id="50d9c-138">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="50d9c-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="50d9c-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="50d9c-139">devicesCount</span></span>|<span data-ttu-id="50d9c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="50d9c-140">Int32</span></span>|<span data-ttu-id="50d9c-141">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="50d9c-141">Devices count for that user.</span></span>|
|<span data-ttu-id="50d9c-142">status</span><span class="sxs-lookup"><span data-stu-id="50d9c-142">status</span></span>|[<span data-ttu-id="50d9c-143">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="50d9c-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="50d9c-144">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="50d9c-144">Compliance status of the policy report.</span></span> <span data-ttu-id="50d9c-145">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="50d9c-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="50d9c-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="50d9c-146">lastReportedDateTime</span></span>|<span data-ttu-id="50d9c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50d9c-147">DateTimeOffset</span></span>|<span data-ttu-id="50d9c-148">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="50d9c-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="50d9c-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="50d9c-149">userPrincipalName</span></span>|<span data-ttu-id="50d9c-150">String</span><span class="sxs-lookup"><span data-stu-id="50d9c-150">String</span></span>|<span data-ttu-id="50d9c-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="50d9c-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="50d9c-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="50d9c-152">Response</span></span>
<span data-ttu-id="50d9c-153">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="50d9c-153">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50d9c-154">Пример</span><span class="sxs-lookup"><span data-stu-id="50d9c-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="50d9c-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="50d9c-155">Request</span></span>
<span data-ttu-id="50d9c-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50d9c-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="50d9c-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="50d9c-157">Response</span></span>
<span data-ttu-id="50d9c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50d9c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



