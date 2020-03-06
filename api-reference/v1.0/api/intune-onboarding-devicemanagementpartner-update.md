---
title: Обновление объекта deviceManagementPartner
description: Обновление свойств объекта deviceManagementPartner.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9158b5dd73f657e5c17326867af89f58772691d4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512512"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="b18ec-103">Обновление объекта deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="b18ec-103">Update deviceManagementPartner</span></span>

<span data-ttu-id="b18ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b18ec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b18ec-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b18ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b18ec-106">Обновление свойств объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="b18ec-106">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b18ec-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b18ec-107">Prerequisites</span></span>
<span data-ttu-id="b18ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b18ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b18ec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b18ec-110">Permission type</span></span>|<span data-ttu-id="b18ec-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b18ec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b18ec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b18ec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b18ec-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b18ec-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b18ec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b18ec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b18ec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b18ec-115">Not supported.</span></span>|
|<span data-ttu-id="b18ec-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b18ec-116">Application</span></span>|<span data-ttu-id="b18ec-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b18ec-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b18ec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b18ec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="b18ec-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b18ec-119">Request headers</span></span>
|<span data-ttu-id="b18ec-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b18ec-120">Header</span></span>|<span data-ttu-id="b18ec-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b18ec-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b18ec-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b18ec-122">Authorization</span></span>|<span data-ttu-id="b18ec-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b18ec-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b18ec-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b18ec-124">Accept</span></span>|<span data-ttu-id="b18ec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b18ec-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b18ec-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b18ec-126">Request body</span></span>
<span data-ttu-id="b18ec-127">В теле запроса добавьте представление объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b18ec-127">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="b18ec-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="b18ec-128">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="b18ec-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b18ec-129">Property</span></span>|<span data-ttu-id="b18ec-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b18ec-130">Type</span></span>|<span data-ttu-id="b18ec-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b18ec-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b18ec-132">id</span><span class="sxs-lookup"><span data-stu-id="b18ec-132">id</span></span>|<span data-ttu-id="b18ec-133">String</span><span class="sxs-lookup"><span data-stu-id="b18ec-133">String</span></span>|<span data-ttu-id="b18ec-134">Идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="b18ec-134">Id of the entity</span></span>|
|<span data-ttu-id="b18ec-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="b18ec-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="b18ec-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b18ec-136">DateTimeOffset</span></span>|<span data-ttu-id="b18ec-137">Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".</span><span class="sxs-lookup"><span data-stu-id="b18ec-137">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="b18ec-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="b18ec-138">partnerState</span></span>|[<span data-ttu-id="b18ec-139">девицеманажементпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="b18ec-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="b18ec-140">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="b18ec-140">Partner state of this tenant.</span></span> <span data-ttu-id="b18ec-141">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="b18ec-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="b18ec-142">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="b18ec-142">partnerAppType</span></span>|[<span data-ttu-id="b18ec-143">девицеманажементпартнерапптипе</span><span class="sxs-lookup"><span data-stu-id="b18ec-143">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="b18ec-144">Тип партнерского приложения.</span><span class="sxs-lookup"><span data-stu-id="b18ec-144">Partner App type.</span></span> <span data-ttu-id="b18ec-145">Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="b18ec-145">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="b18ec-146">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="b18ec-146">singleTenantAppId</span></span>|<span data-ttu-id="b18ec-147">String</span><span class="sxs-lookup"><span data-stu-id="b18ec-147">String</span></span>|<span data-ttu-id="b18ec-148">Идентификатор одноклиентского приложения партнера</span><span class="sxs-lookup"><span data-stu-id="b18ec-148">Partner Single tenant App id</span></span>|
|<span data-ttu-id="b18ec-149">displayName</span><span class="sxs-lookup"><span data-stu-id="b18ec-149">displayName</span></span>|<span data-ttu-id="b18ec-150">Строка</span><span class="sxs-lookup"><span data-stu-id="b18ec-150">String</span></span>|<span data-ttu-id="b18ec-151">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="b18ec-151">Partner display name</span></span>|
|<span data-ttu-id="b18ec-152">isConfigured</span><span class="sxs-lookup"><span data-stu-id="b18ec-152">isConfigured</span></span>|<span data-ttu-id="b18ec-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="b18ec-153">Boolean</span></span>|<span data-ttu-id="b18ec-154">Указывает, настроен ли партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="b18ec-154">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="b18ec-155">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="b18ec-155">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="b18ec-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b18ec-156">DateTimeOffset</span></span>|<span data-ttu-id="b18ec-157">Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства</span><span class="sxs-lookup"><span data-stu-id="b18ec-157">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="b18ec-158">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="b18ec-158">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="b18ec-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b18ec-159">DateTimeOffset</span></span>|<span data-ttu-id="b18ec-160">Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям</span><span class="sxs-lookup"><span data-stu-id="b18ec-160">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="b18ec-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="b18ec-161">Response</span></span>
<span data-ttu-id="b18ec-162">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b18ec-162">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b18ec-163">Пример</span><span class="sxs-lookup"><span data-stu-id="b18ec-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="b18ec-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="b18ec-164">Request</span></span>
<span data-ttu-id="b18ec-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b18ec-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 502

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```

### <a name="response"></a><span data-ttu-id="b18ec-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="b18ec-166">Response</span></span>
<span data-ttu-id="b18ec-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b18ec-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 551

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```




