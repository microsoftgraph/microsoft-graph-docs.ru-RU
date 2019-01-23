---
title: Обновление объекта managedDeviceMobileAppConfigurationUserStatus
description: Обновление свойств объекта managedDeviceMobileAppConfigurationUserStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 05ea762bafe2d5a950c4d5e582ec4e185f6d2425
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405158"
---
# <a name="update-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="a30b4-103">Обновление объекта managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="a30b4-103">Update managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="a30b4-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a30b4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a30b4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a30b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a30b4-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a30b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a30b4-107">Обновление свойств объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a30b4-107">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a30b4-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a30b4-108">Prerequisites</span></span>
<span data-ttu-id="a30b4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a30b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a30b4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a30b4-111">Permission type</span></span>|<span data-ttu-id="a30b4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a30b4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a30b4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a30b4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a30b4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a30b4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a30b4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a30b4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a30b4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a30b4-116">Not supported.</span></span>|
|<span data-ttu-id="a30b4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a30b4-117">Application</span></span>|<span data-ttu-id="a30b4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a30b4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a30b4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a30b4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="a30b4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a30b4-120">Request headers</span></span>
|<span data-ttu-id="a30b4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a30b4-121">Header</span></span>|<span data-ttu-id="a30b4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a30b4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a30b4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a30b4-123">Authorization</span></span>|<span data-ttu-id="a30b4-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a30b4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a30b4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a30b4-125">Accept</span></span>|<span data-ttu-id="a30b4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a30b4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a30b4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a30b4-127">Request body</span></span>
<span data-ttu-id="a30b4-128">В тексте запроса добавьте представление объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a30b4-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="a30b4-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a30b4-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="a30b4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a30b4-130">Property</span></span>|<span data-ttu-id="a30b4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a30b4-131">Type</span></span>|<span data-ttu-id="a30b4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a30b4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a30b4-133">id</span><span class="sxs-lookup"><span data-stu-id="a30b4-133">id</span></span>|<span data-ttu-id="a30b4-134">String</span><span class="sxs-lookup"><span data-stu-id="a30b4-134">String</span></span>|<span data-ttu-id="a30b4-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a30b4-135">Key of the entity.</span></span>|
|<span data-ttu-id="a30b4-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="a30b4-136">userDisplayName</span></span>|<span data-ttu-id="a30b4-137">String</span><span class="sxs-lookup"><span data-stu-id="a30b4-137">String</span></span>|<span data-ttu-id="a30b4-138">Имя пользователя в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="a30b4-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="a30b4-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="a30b4-139">devicesCount</span></span>|<span data-ttu-id="a30b4-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a30b4-140">Int32</span></span>|<span data-ttu-id="a30b4-141">Количество устройств для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="a30b4-141">Devices count for that user.</span></span>|
|<span data-ttu-id="a30b4-142">status</span><span class="sxs-lookup"><span data-stu-id="a30b4-142">status</span></span>|[<span data-ttu-id="a30b4-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a30b4-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a30b4-144">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="a30b4-144">Compliance status of the policy report.</span></span> <span data-ttu-id="a30b4-145">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a30b4-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a30b4-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a30b4-146">lastReportedDateTime</span></span>|<span data-ttu-id="a30b4-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a30b4-147">DateTimeOffset</span></span>|<span data-ttu-id="a30b4-148">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="a30b4-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="a30b4-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a30b4-149">userPrincipalName</span></span>|<span data-ttu-id="a30b4-150">String</span><span class="sxs-lookup"><span data-stu-id="a30b4-150">String</span></span>|<span data-ttu-id="a30b4-151">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="a30b4-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="a30b4-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="a30b4-152">Response</span></span>
<span data-ttu-id="a30b4-153">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a30b4-153">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a30b4-154">Пример</span><span class="sxs-lookup"><span data-stu-id="a30b4-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="a30b4-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="a30b4-155">Request</span></span>
<span data-ttu-id="a30b4-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a30b4-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a30b4-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="a30b4-157">Response</span></span>
<span data-ttu-id="a30b4-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a30b4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




