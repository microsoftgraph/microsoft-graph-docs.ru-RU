---
title: Создание объекта managedDeviceMobileAppConfigurationUserStatus
description: Создание объекта managedDeviceMobileAppConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7124189a5fa5d1121daf352e50584bdadce6fd8c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974484"
---
# <a name="create-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="04a77-103">Создание объекта managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="04a77-103">Create managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="04a77-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04a77-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04a77-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04a77-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04a77-106">Создание объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="04a77-106">Create a new [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04a77-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="04a77-107">Prerequisites</span></span>
<span data-ttu-id="04a77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04a77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04a77-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04a77-110">Permission type</span></span>|<span data-ttu-id="04a77-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="04a77-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04a77-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04a77-112">Delegated (work or school account)</span></span>|<span data-ttu-id="04a77-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04a77-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04a77-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04a77-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04a77-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04a77-115">Not supported.</span></span>|
|<span data-ttu-id="04a77-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04a77-116">Application</span></span>|<span data-ttu-id="04a77-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04a77-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04a77-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04a77-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="04a77-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04a77-119">Request headers</span></span>
|<span data-ttu-id="04a77-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04a77-120">Header</span></span>|<span data-ttu-id="04a77-121">Значение</span><span class="sxs-lookup"><span data-stu-id="04a77-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04a77-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04a77-122">Authorization</span></span>|<span data-ttu-id="04a77-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04a77-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04a77-124">Accept</span><span class="sxs-lookup"><span data-stu-id="04a77-124">Accept</span></span>|<span data-ttu-id="04a77-125">application/json</span><span class="sxs-lookup"><span data-stu-id="04a77-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04a77-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04a77-126">Request body</span></span>
<span data-ttu-id="04a77-127">В тексте запроса добавьте представление объекта managedDeviceMobileAppConfigurationUserStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04a77-127">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationUserStatus object.</span></span>

<span data-ttu-id="04a77-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта managedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="04a77-128">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationUserStatus.</span></span>

|<span data-ttu-id="04a77-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="04a77-129">Property</span></span>|<span data-ttu-id="04a77-130">Тип</span><span class="sxs-lookup"><span data-stu-id="04a77-130">Type</span></span>|<span data-ttu-id="04a77-131">Описание</span><span class="sxs-lookup"><span data-stu-id="04a77-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04a77-132">id</span><span class="sxs-lookup"><span data-stu-id="04a77-132">id</span></span>|<span data-ttu-id="04a77-133">Строка</span><span class="sxs-lookup"><span data-stu-id="04a77-133">String</span></span>|<span data-ttu-id="04a77-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="04a77-134">Key of the entity.</span></span>|
|<span data-ttu-id="04a77-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="04a77-135">userDisplayName</span></span>|<span data-ttu-id="04a77-136">String</span><span class="sxs-lookup"><span data-stu-id="04a77-136">String</span></span>|<span data-ttu-id="04a77-137">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="04a77-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="04a77-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="04a77-138">devicesCount</span></span>|<span data-ttu-id="04a77-139">Int32</span><span class="sxs-lookup"><span data-stu-id="04a77-139">Int32</span></span>|<span data-ttu-id="04a77-140">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="04a77-140">Devices count for that user.</span></span>|
|<span data-ttu-id="04a77-141">status</span><span class="sxs-lookup"><span data-stu-id="04a77-141">status</span></span>|[<span data-ttu-id="04a77-142">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="04a77-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="04a77-143">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="04a77-143">Compliance status of the policy report.</span></span> <span data-ttu-id="04a77-144">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="04a77-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="04a77-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="04a77-145">lastReportedDateTime</span></span>|<span data-ttu-id="04a77-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04a77-146">DateTimeOffset</span></span>|<span data-ttu-id="04a77-147">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="04a77-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="04a77-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="04a77-148">userPrincipalName</span></span>|<span data-ttu-id="04a77-149">String</span><span class="sxs-lookup"><span data-stu-id="04a77-149">String</span></span>|<span data-ttu-id="04a77-150">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="04a77-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="04a77-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="04a77-151">Response</span></span>
<span data-ttu-id="04a77-152">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04a77-152">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04a77-153">Пример</span><span class="sxs-lookup"><span data-stu-id="04a77-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="04a77-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="04a77-154">Request</span></span>
<span data-ttu-id="04a77-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04a77-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="04a77-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="04a77-156">Response</span></span>
<span data-ttu-id="04a77-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04a77-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




