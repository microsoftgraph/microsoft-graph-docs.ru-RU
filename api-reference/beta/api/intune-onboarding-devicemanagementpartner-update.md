---
title: Обновление объекта deviceManagementPartner
description: Обновление свойств объекта deviceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e75644c57fdee030bd0fc8858d49ed7f0625dbe2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145455"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="39ab7-103">Обновление объекта deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="39ab7-103">Update deviceManagementPartner</span></span>

<span data-ttu-id="39ab7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39ab7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="39ab7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39ab7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39ab7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="39ab7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39ab7-107">Обновление свойств объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="39ab7-107">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39ab7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="39ab7-108">Prerequisites</span></span>
<span data-ttu-id="39ab7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39ab7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39ab7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39ab7-111">Permission type</span></span>|<span data-ttu-id="39ab7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39ab7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39ab7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39ab7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="39ab7-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39ab7-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="39ab7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39ab7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39ab7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39ab7-116">Not supported.</span></span>|
|<span data-ttu-id="39ab7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="39ab7-117">Application</span></span>|<span data-ttu-id="39ab7-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39ab7-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="39ab7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39ab7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="39ab7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="39ab7-120">Request headers</span></span>
|<span data-ttu-id="39ab7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="39ab7-121">Header</span></span>|<span data-ttu-id="39ab7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="39ab7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39ab7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="39ab7-123">Authorization</span></span>|<span data-ttu-id="39ab7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39ab7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39ab7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="39ab7-125">Accept</span></span>|<span data-ttu-id="39ab7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="39ab7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39ab7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39ab7-127">Request body</span></span>
<span data-ttu-id="39ab7-128">В теле запроса добавьте представление объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39ab7-128">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="39ab7-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="39ab7-129">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="39ab7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="39ab7-130">Property</span></span>|<span data-ttu-id="39ab7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="39ab7-131">Type</span></span>|<span data-ttu-id="39ab7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="39ab7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39ab7-133">id</span><span class="sxs-lookup"><span data-stu-id="39ab7-133">id</span></span>|<span data-ttu-id="39ab7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="39ab7-134">String</span></span>|<span data-ttu-id="39ab7-135">Id объекта</span><span class="sxs-lookup"><span data-stu-id="39ab7-135">Id of the entity</span></span>|
|<span data-ttu-id="39ab7-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="39ab7-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="39ab7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39ab7-137">DateTimeOffset</span></span>|<span data-ttu-id="39ab7-138">Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".</span><span class="sxs-lookup"><span data-stu-id="39ab7-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="39ab7-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="39ab7-139">partnerState</span></span>|[<span data-ttu-id="39ab7-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="39ab7-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="39ab7-141">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="39ab7-141">Partner state of this tenant.</span></span> <span data-ttu-id="39ab7-142">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="39ab7-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="39ab7-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="39ab7-143">partnerAppType</span></span>|[<span data-ttu-id="39ab7-144">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="39ab7-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="39ab7-145">Тип приложения-партнера.</span><span class="sxs-lookup"><span data-stu-id="39ab7-145">Partner App type.</span></span> <span data-ttu-id="39ab7-146">Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="39ab7-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="39ab7-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="39ab7-147">singleTenantAppId</span></span>|<span data-ttu-id="39ab7-148">String</span><span class="sxs-lookup"><span data-stu-id="39ab7-148">String</span></span>|<span data-ttu-id="39ab7-149">Идентификатор одноклиентского приложения партнера</span><span class="sxs-lookup"><span data-stu-id="39ab7-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="39ab7-150">displayName</span><span class="sxs-lookup"><span data-stu-id="39ab7-150">displayName</span></span>|<span data-ttu-id="39ab7-151">Строка</span><span class="sxs-lookup"><span data-stu-id="39ab7-151">String</span></span>|<span data-ttu-id="39ab7-152">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="39ab7-152">Partner display name</span></span>|
|<span data-ttu-id="39ab7-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="39ab7-153">isConfigured</span></span>|<span data-ttu-id="39ab7-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="39ab7-154">Boolean</span></span>|<span data-ttu-id="39ab7-155">Указывает, настроен ли партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="39ab7-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="39ab7-156">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="39ab7-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="39ab7-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39ab7-157">DateTimeOffset</span></span>|<span data-ttu-id="39ab7-158">DateTime в UTC, когда будут удалены PartnerDevices.</span><span class="sxs-lookup"><span data-stu-id="39ab7-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="39ab7-159">Это станет obselete в ближайшее время.</span><span class="sxs-lookup"><span data-stu-id="39ab7-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="39ab7-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="39ab7-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="39ab7-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39ab7-161">DateTimeOffset</span></span>|<span data-ttu-id="39ab7-162">DateTime в UTC, когда PartnerDevices будет помечен как NonCompliant.</span><span class="sxs-lookup"><span data-stu-id="39ab7-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="39ab7-163">Это станет obselete в ближайшее время.</span><span class="sxs-lookup"><span data-stu-id="39ab7-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="39ab7-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="39ab7-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="39ab7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39ab7-165">DateTimeOffset</span></span>|<span data-ttu-id="39ab7-166">Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства</span><span class="sxs-lookup"><span data-stu-id="39ab7-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="39ab7-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="39ab7-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="39ab7-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39ab7-168">DateTimeOffset</span></span>|<span data-ttu-id="39ab7-169">Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям</span><span class="sxs-lookup"><span data-stu-id="39ab7-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|
|<span data-ttu-id="39ab7-170">groupsRequiringPartnerEnrollment</span><span class="sxs-lookup"><span data-stu-id="39ab7-170">groupsRequiringPartnerEnrollment</span></span>|<span data-ttu-id="39ab7-171">[коллекция deviceManagementPartnerAssignment](../resources/intune-onboarding-devicemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="39ab7-171">[deviceManagementPartnerAssignment](../resources/intune-onboarding-devicemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="39ab7-172">Группы пользователей, которые уточняют, является ли регистрация партнером.</span><span class="sxs-lookup"><span data-stu-id="39ab7-172">User groups that specifies whether enrollment is through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="39ab7-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="39ab7-173">Response</span></span>
<span data-ttu-id="39ab7-174">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="39ab7-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39ab7-175">Пример</span><span class="sxs-lookup"><span data-stu-id="39ab7-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="39ab7-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="39ab7-176">Request</span></span>
<span data-ttu-id="39ab7-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39ab7-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 1140

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00",
  "groupsRequiringPartnerEnrollment": [
    {
      "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="39ab7-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="39ab7-178">Response</span></span>
<span data-ttu-id="39ab7-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39ab7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1189

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00",
  "groupsRequiringPartnerEnrollment": [
    {
      "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




