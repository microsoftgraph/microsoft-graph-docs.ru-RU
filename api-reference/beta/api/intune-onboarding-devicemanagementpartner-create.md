---
title: Создание объекта deviceManagementPartner
description: Создание объекта deviceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8fc6a768edbfdc51886e4bc55efb428a156e460c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49285571"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="6ce05-103">Создание объекта deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="6ce05-103">Create deviceManagementPartner</span></span>

<span data-ttu-id="6ce05-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ce05-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ce05-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ce05-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ce05-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ce05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ce05-107">Создание объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="6ce05-107">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ce05-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6ce05-108">Prerequisites</span></span>
<span data-ttu-id="6ce05-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ce05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ce05-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ce05-111">Permission type</span></span>|<span data-ttu-id="6ce05-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ce05-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ce05-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ce05-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ce05-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ce05-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6ce05-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ce05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ce05-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ce05-116">Not supported.</span></span>|
|<span data-ttu-id="6ce05-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ce05-117">Application</span></span>|<span data-ttu-id="6ce05-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ce05-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ce05-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ce05-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="6ce05-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6ce05-120">Request headers</span></span>
|<span data-ttu-id="6ce05-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ce05-121">Header</span></span>|<span data-ttu-id="6ce05-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6ce05-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ce05-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ce05-123">Authorization</span></span>|<span data-ttu-id="6ce05-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ce05-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ce05-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6ce05-125">Accept</span></span>|<span data-ttu-id="6ce05-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ce05-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ce05-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ce05-127">Request body</span></span>
<span data-ttu-id="6ce05-128">В теле запроса добавьте представление объекта deviceManagementPartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ce05-128">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="6ce05-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="6ce05-129">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="6ce05-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ce05-130">Property</span></span>|<span data-ttu-id="6ce05-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6ce05-131">Type</span></span>|<span data-ttu-id="6ce05-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6ce05-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ce05-133">id</span><span class="sxs-lookup"><span data-stu-id="6ce05-133">id</span></span>|<span data-ttu-id="6ce05-134">String</span><span class="sxs-lookup"><span data-stu-id="6ce05-134">String</span></span>|<span data-ttu-id="6ce05-135">Идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="6ce05-135">Id of the entity</span></span>|
|<span data-ttu-id="6ce05-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="6ce05-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="6ce05-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ce05-137">DateTimeOffset</span></span>|<span data-ttu-id="6ce05-138">Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".</span><span class="sxs-lookup"><span data-stu-id="6ce05-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="6ce05-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="6ce05-139">partnerState</span></span>|[<span data-ttu-id="6ce05-140">девицеманажементпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="6ce05-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="6ce05-141">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="6ce05-141">Partner state of this tenant.</span></span> <span data-ttu-id="6ce05-142">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="6ce05-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="6ce05-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="6ce05-143">partnerAppType</span></span>|[<span data-ttu-id="6ce05-144">девицеманажементпартнерапптипе</span><span class="sxs-lookup"><span data-stu-id="6ce05-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="6ce05-145">Тип партнерского приложения.</span><span class="sxs-lookup"><span data-stu-id="6ce05-145">Partner App type.</span></span> <span data-ttu-id="6ce05-146">Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="6ce05-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="6ce05-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="6ce05-147">singleTenantAppId</span></span>|<span data-ttu-id="6ce05-148">String</span><span class="sxs-lookup"><span data-stu-id="6ce05-148">String</span></span>|<span data-ttu-id="6ce05-149">Идентификатор одноклиентского приложения партнера</span><span class="sxs-lookup"><span data-stu-id="6ce05-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="6ce05-150">displayName</span><span class="sxs-lookup"><span data-stu-id="6ce05-150">displayName</span></span>|<span data-ttu-id="6ce05-151">String</span><span class="sxs-lookup"><span data-stu-id="6ce05-151">String</span></span>|<span data-ttu-id="6ce05-152">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="6ce05-152">Partner display name</span></span>|
|<span data-ttu-id="6ce05-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="6ce05-153">isConfigured</span></span>|<span data-ttu-id="6ce05-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ce05-154">Boolean</span></span>|<span data-ttu-id="6ce05-155">Указывает, настроен ли партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="6ce05-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="6ce05-156">вхенпартнердевицесвиллберемовед</span><span class="sxs-lookup"><span data-stu-id="6ce05-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="6ce05-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ce05-157">DateTimeOffset</span></span>|<span data-ttu-id="6ce05-158">Дата и время в формате UTC, когда партнерские устройства будет удален.</span><span class="sxs-lookup"><span data-stu-id="6ce05-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="6ce05-159">Это скоро станет обселете.</span><span class="sxs-lookup"><span data-stu-id="6ce05-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="6ce05-160">вхенпартнердевицесвиллбемаркедаснонкомплиант</span><span class="sxs-lookup"><span data-stu-id="6ce05-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="6ce05-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ce05-161">DateTimeOffset</span></span>|<span data-ttu-id="6ce05-162">Дата и время в формате UTC, когда партнерские устройства будет помечен как несоответствующий.</span><span class="sxs-lookup"><span data-stu-id="6ce05-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="6ce05-163">Это скоро станет обселете.</span><span class="sxs-lookup"><span data-stu-id="6ce05-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="6ce05-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ce05-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="6ce05-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ce05-165">DateTimeOffset</span></span>|<span data-ttu-id="6ce05-166">Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства</span><span class="sxs-lookup"><span data-stu-id="6ce05-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="6ce05-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="6ce05-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="6ce05-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ce05-168">DateTimeOffset</span></span>|<span data-ttu-id="6ce05-169">Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям</span><span class="sxs-lookup"><span data-stu-id="6ce05-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|
|<span data-ttu-id="6ce05-170">граупсрекуирингпартнеренроллмент</span><span class="sxs-lookup"><span data-stu-id="6ce05-170">groupsRequiringPartnerEnrollment</span></span>|<span data-ttu-id="6ce05-171">Коллекция [девицеманажементпартнерассигнмент](../resources/intune-onboarding-devicemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6ce05-171">[deviceManagementPartnerAssignment](../resources/intune-onboarding-devicemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="6ce05-172">Группы пользователей, указывающие, осуществляется ли регистрация через партнера.</span><span class="sxs-lookup"><span data-stu-id="6ce05-172">User groups that specifies whether enrollment is through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="6ce05-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ce05-173">Response</span></span>
<span data-ttu-id="6ce05-174">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6ce05-174">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ce05-175">Пример</span><span class="sxs-lookup"><span data-stu-id="6ce05-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ce05-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ce05-176">Request</span></span>
<span data-ttu-id="6ce05-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ce05-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
Content-type: application/json
Content-length: 1072

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
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="6ce05-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ce05-178">Response</span></span>
<span data-ttu-id="6ce05-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ce05-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1121

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
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```




