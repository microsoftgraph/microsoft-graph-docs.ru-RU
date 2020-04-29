---
title: Создание объекта deviceManagementPartner
description: Создание объекта deviceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 73df635a4af3acbb55be7ecd1163555ac4f701bc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473206"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="ae03a-103">Создание объекта deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="ae03a-103">Create deviceManagementPartner</span></span>

<span data-ttu-id="ae03a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae03a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae03a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae03a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae03a-106">Создание объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="ae03a-106">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae03a-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ae03a-107">Prerequisites</span></span>
<span data-ttu-id="ae03a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae03a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae03a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae03a-110">Permission type</span></span>|<span data-ttu-id="ae03a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae03a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae03a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae03a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae03a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae03a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ae03a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae03a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae03a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae03a-115">Not supported.</span></span>|
|<span data-ttu-id="ae03a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae03a-116">Application</span></span>|<span data-ttu-id="ae03a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae03a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae03a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae03a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="ae03a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ae03a-119">Request headers</span></span>
|<span data-ttu-id="ae03a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ae03a-120">Header</span></span>|<span data-ttu-id="ae03a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ae03a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae03a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae03a-122">Authorization</span></span>|<span data-ttu-id="ae03a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae03a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae03a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ae03a-124">Accept</span></span>|<span data-ttu-id="ae03a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ae03a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae03a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ae03a-126">Request body</span></span>
<span data-ttu-id="ae03a-127">В теле запроса добавьте представление объекта deviceManagementPartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae03a-127">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="ae03a-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="ae03a-128">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="ae03a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae03a-129">Property</span></span>|<span data-ttu-id="ae03a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ae03a-130">Type</span></span>|<span data-ttu-id="ae03a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ae03a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae03a-132">id</span><span class="sxs-lookup"><span data-stu-id="ae03a-132">id</span></span>|<span data-ttu-id="ae03a-133">String</span><span class="sxs-lookup"><span data-stu-id="ae03a-133">String</span></span>|<span data-ttu-id="ae03a-134">Идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="ae03a-134">Id of the entity</span></span>|
|<span data-ttu-id="ae03a-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="ae03a-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="ae03a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae03a-136">DateTimeOffset</span></span>|<span data-ttu-id="ae03a-137">Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".</span><span class="sxs-lookup"><span data-stu-id="ae03a-137">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="ae03a-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="ae03a-138">partnerState</span></span>|[<span data-ttu-id="ae03a-139">девицеманажементпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="ae03a-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="ae03a-140">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="ae03a-140">Partner state of this tenant.</span></span> <span data-ttu-id="ae03a-141">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="ae03a-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="ae03a-142">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="ae03a-142">partnerAppType</span></span>|[<span data-ttu-id="ae03a-143">девицеманажементпартнерапптипе</span><span class="sxs-lookup"><span data-stu-id="ae03a-143">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="ae03a-144">Тип партнерского приложения.</span><span class="sxs-lookup"><span data-stu-id="ae03a-144">Partner App type.</span></span> <span data-ttu-id="ae03a-145">Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="ae03a-145">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="ae03a-146">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="ae03a-146">singleTenantAppId</span></span>|<span data-ttu-id="ae03a-147">String</span><span class="sxs-lookup"><span data-stu-id="ae03a-147">String</span></span>|<span data-ttu-id="ae03a-148">Идентификатор одноклиентского приложения партнера</span><span class="sxs-lookup"><span data-stu-id="ae03a-148">Partner Single tenant App id</span></span>|
|<span data-ttu-id="ae03a-149">displayName</span><span class="sxs-lookup"><span data-stu-id="ae03a-149">displayName</span></span>|<span data-ttu-id="ae03a-150">Строка</span><span class="sxs-lookup"><span data-stu-id="ae03a-150">String</span></span>|<span data-ttu-id="ae03a-151">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="ae03a-151">Partner display name</span></span>|
|<span data-ttu-id="ae03a-152">isConfigured</span><span class="sxs-lookup"><span data-stu-id="ae03a-152">isConfigured</span></span>|<span data-ttu-id="ae03a-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae03a-153">Boolean</span></span>|<span data-ttu-id="ae03a-154">Указывает, настроен ли партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="ae03a-154">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="ae03a-155">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae03a-155">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="ae03a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae03a-156">DateTimeOffset</span></span>|<span data-ttu-id="ae03a-157">Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства</span><span class="sxs-lookup"><span data-stu-id="ae03a-157">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="ae03a-158">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="ae03a-158">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="ae03a-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae03a-159">DateTimeOffset</span></span>|<span data-ttu-id="ae03a-160">Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям</span><span class="sxs-lookup"><span data-stu-id="ae03a-160">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="ae03a-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae03a-161">Response</span></span>
<span data-ttu-id="ae03a-162">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ae03a-162">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae03a-163">Пример</span><span class="sxs-lookup"><span data-stu-id="ae03a-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae03a-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae03a-164">Request</span></span>
<span data-ttu-id="ae03a-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae03a-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners
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

### <a name="response"></a><span data-ttu-id="ae03a-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae03a-166">Response</span></span>
<span data-ttu-id="ae03a-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae03a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






