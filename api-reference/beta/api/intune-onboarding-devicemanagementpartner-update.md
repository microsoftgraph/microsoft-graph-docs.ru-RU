---
title: Обновление объекта deviceManagementPartner
description: Обновление свойств объекта deviceManagementPartner.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 200897b4f4060b1e94f6a72c61c267202c609c19
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462049"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="e1914-103">Обновление объекта deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="e1914-103">Update deviceManagementPartner</span></span>

<span data-ttu-id="e1914-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e1914-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1914-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1914-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1914-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e1914-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1914-107">Обновление свойств объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="e1914-107">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1914-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e1914-108">Prerequisites</span></span>
<span data-ttu-id="e1914-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1914-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1914-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1914-111">Permission type</span></span>|<span data-ttu-id="e1914-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1914-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1914-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1914-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1914-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1914-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e1914-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1914-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1914-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1914-116">Not supported.</span></span>|
|<span data-ttu-id="e1914-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1914-117">Application</span></span>|<span data-ttu-id="e1914-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1914-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1914-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1914-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="e1914-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e1914-120">Request headers</span></span>
|<span data-ttu-id="e1914-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e1914-121">Header</span></span>|<span data-ttu-id="e1914-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e1914-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1914-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1914-123">Authorization</span></span>|<span data-ttu-id="e1914-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1914-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1914-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e1914-125">Accept</span></span>|<span data-ttu-id="e1914-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1914-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1914-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1914-127">Request body</span></span>
<span data-ttu-id="e1914-128">В теле запроса добавьте представление объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1914-128">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="e1914-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="e1914-129">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="e1914-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1914-130">Property</span></span>|<span data-ttu-id="e1914-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e1914-131">Type</span></span>|<span data-ttu-id="e1914-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e1914-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1914-133">id</span><span class="sxs-lookup"><span data-stu-id="e1914-133">id</span></span>|<span data-ttu-id="e1914-134">String</span><span class="sxs-lookup"><span data-stu-id="e1914-134">String</span></span>|<span data-ttu-id="e1914-135">Идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="e1914-135">Id of the entity</span></span>|
|<span data-ttu-id="e1914-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="e1914-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="e1914-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1914-137">DateTimeOffset</span></span>|<span data-ttu-id="e1914-138">Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".</span><span class="sxs-lookup"><span data-stu-id="e1914-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="e1914-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="e1914-139">partnerState</span></span>|[<span data-ttu-id="e1914-140">девицеманажементпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="e1914-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="e1914-141">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="e1914-141">Partner state of this tenant.</span></span> <span data-ttu-id="e1914-142">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="e1914-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="e1914-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="e1914-143">partnerAppType</span></span>|[<span data-ttu-id="e1914-144">девицеманажементпартнерапптипе</span><span class="sxs-lookup"><span data-stu-id="e1914-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="e1914-145">Тип партнерского приложения.</span><span class="sxs-lookup"><span data-stu-id="e1914-145">Partner App type.</span></span> <span data-ttu-id="e1914-146">Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="e1914-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="e1914-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="e1914-147">singleTenantAppId</span></span>|<span data-ttu-id="e1914-148">String</span><span class="sxs-lookup"><span data-stu-id="e1914-148">String</span></span>|<span data-ttu-id="e1914-149">Идентификатор одноклиентского приложения партнера</span><span class="sxs-lookup"><span data-stu-id="e1914-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="e1914-150">displayName</span><span class="sxs-lookup"><span data-stu-id="e1914-150">displayName</span></span>|<span data-ttu-id="e1914-151">Строка</span><span class="sxs-lookup"><span data-stu-id="e1914-151">String</span></span>|<span data-ttu-id="e1914-152">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="e1914-152">Partner display name</span></span>|
|<span data-ttu-id="e1914-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="e1914-153">isConfigured</span></span>|<span data-ttu-id="e1914-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1914-154">Boolean</span></span>|<span data-ttu-id="e1914-155">Указывает, настроен ли партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="e1914-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="e1914-156">вхенпартнердевицесвиллберемовед</span><span class="sxs-lookup"><span data-stu-id="e1914-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="e1914-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1914-157">DateTimeOffset</span></span>|<span data-ttu-id="e1914-158">Дата и время в формате UTC, когда партнерские устройства будет удален.</span><span class="sxs-lookup"><span data-stu-id="e1914-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="e1914-159">Это скоро станет обселете.</span><span class="sxs-lookup"><span data-stu-id="e1914-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="e1914-160">вхенпартнердевицесвиллбемаркедаснонкомплиант</span><span class="sxs-lookup"><span data-stu-id="e1914-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="e1914-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1914-161">DateTimeOffset</span></span>|<span data-ttu-id="e1914-162">Дата и время в формате UTC, когда партнерские устройства будет помечен как несоответствующий.</span><span class="sxs-lookup"><span data-stu-id="e1914-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="e1914-163">Это скоро станет обселете.</span><span class="sxs-lookup"><span data-stu-id="e1914-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="e1914-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1914-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="e1914-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1914-165">DateTimeOffset</span></span>|<span data-ttu-id="e1914-166">Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства</span><span class="sxs-lookup"><span data-stu-id="e1914-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="e1914-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="e1914-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="e1914-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1914-168">DateTimeOffset</span></span>|<span data-ttu-id="e1914-169">Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям</span><span class="sxs-lookup"><span data-stu-id="e1914-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|
|<span data-ttu-id="e1914-170">граупсрекуирингпартнеренроллмент</span><span class="sxs-lookup"><span data-stu-id="e1914-170">groupsRequiringPartnerEnrollment</span></span>|<span data-ttu-id="e1914-171">Коллекция [девицеманажементпартнерассигнмент](../resources/intune-onboarding-devicemanagementpartnerassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e1914-171">[deviceManagementPartnerAssignment](../resources/intune-onboarding-devicemanagementpartnerassignment.md) collection</span></span>|<span data-ttu-id="e1914-172">Группы пользователей, указывающие, осуществляется ли регистрация через партнера.</span><span class="sxs-lookup"><span data-stu-id="e1914-172">User groups that specifies whether enrollment is through partner.</span></span>|



## <a name="response"></a><span data-ttu-id="e1914-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1914-173">Response</span></span>
<span data-ttu-id="e1914-174">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e1914-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1914-175">Пример</span><span class="sxs-lookup"><span data-stu-id="e1914-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1914-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1914-176">Request</span></span>
<span data-ttu-id="e1914-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1914-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 897

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
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e1914-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1914-178">Response</span></span>
<span data-ttu-id="e1914-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1914-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 946

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
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
      }
    }
  ]
}
```





