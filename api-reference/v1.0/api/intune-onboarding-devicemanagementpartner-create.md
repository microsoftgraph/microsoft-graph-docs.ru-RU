---
title: Создание объекта deviceManagementPartner
description: Создание объекта deviceManagementPartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6c9087653c68f52cf0926acb205acb6afc6b83d8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075093"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="7b273-103">Создание объекта deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="7b273-103">Create deviceManagementPartner</span></span>

<span data-ttu-id="7b273-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b273-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b273-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b273-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b273-106">Создание объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="7b273-106">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b273-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7b273-107">Prerequisites</span></span>
<span data-ttu-id="7b273-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b273-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b273-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b273-110">Permission type</span></span>|<span data-ttu-id="7b273-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b273-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b273-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b273-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7b273-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b273-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7b273-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b273-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b273-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b273-115">Not supported.</span></span>|
|<span data-ttu-id="7b273-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b273-116">Application</span></span>|<span data-ttu-id="7b273-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b273-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b273-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b273-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="7b273-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7b273-119">Request headers</span></span>
|<span data-ttu-id="7b273-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b273-120">Header</span></span>|<span data-ttu-id="7b273-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7b273-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b273-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b273-122">Authorization</span></span>|<span data-ttu-id="7b273-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b273-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b273-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7b273-124">Accept</span></span>|<span data-ttu-id="7b273-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7b273-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b273-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b273-126">Request body</span></span>
<span data-ttu-id="7b273-127">В теле запроса добавьте представление объекта deviceManagementPartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b273-127">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="7b273-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="7b273-128">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="7b273-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b273-129">Property</span></span>|<span data-ttu-id="7b273-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7b273-130">Type</span></span>|<span data-ttu-id="7b273-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7b273-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b273-132">id</span><span class="sxs-lookup"><span data-stu-id="7b273-132">id</span></span>|<span data-ttu-id="7b273-133">Строка</span><span class="sxs-lookup"><span data-stu-id="7b273-133">String</span></span>|<span data-ttu-id="7b273-134">Идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="7b273-134">Id of the entity</span></span>|
|<span data-ttu-id="7b273-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="7b273-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="7b273-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b273-136">DateTimeOffset</span></span>|<span data-ttu-id="7b273-137">Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".</span><span class="sxs-lookup"><span data-stu-id="7b273-137">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="7b273-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="7b273-138">partnerState</span></span>|[<span data-ttu-id="7b273-139">девицеманажементпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="7b273-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="7b273-140">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="7b273-140">Partner state of this tenant.</span></span> <span data-ttu-id="7b273-141">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="7b273-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="7b273-142">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="7b273-142">partnerAppType</span></span>|[<span data-ttu-id="7b273-143">девицеманажементпартнерапптипе</span><span class="sxs-lookup"><span data-stu-id="7b273-143">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="7b273-144">Тип партнерского приложения.</span><span class="sxs-lookup"><span data-stu-id="7b273-144">Partner App type.</span></span> <span data-ttu-id="7b273-145">Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="7b273-145">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="7b273-146">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="7b273-146">singleTenantAppId</span></span>|<span data-ttu-id="7b273-147">String</span><span class="sxs-lookup"><span data-stu-id="7b273-147">String</span></span>|<span data-ttu-id="7b273-148">Идентификатор одноклиентского приложения партнера</span><span class="sxs-lookup"><span data-stu-id="7b273-148">Partner Single tenant App id</span></span>|
|<span data-ttu-id="7b273-149">displayName</span><span class="sxs-lookup"><span data-stu-id="7b273-149">displayName</span></span>|<span data-ttu-id="7b273-150">Строка</span><span class="sxs-lookup"><span data-stu-id="7b273-150">String</span></span>|<span data-ttu-id="7b273-151">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="7b273-151">Partner display name</span></span>|
|<span data-ttu-id="7b273-152">isConfigured</span><span class="sxs-lookup"><span data-stu-id="7b273-152">isConfigured</span></span>|<span data-ttu-id="7b273-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b273-153">Boolean</span></span>|<span data-ttu-id="7b273-154">Указывает, настроен ли партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="7b273-154">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="7b273-155">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b273-155">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="7b273-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b273-156">DateTimeOffset</span></span>|<span data-ttu-id="7b273-157">Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства</span><span class="sxs-lookup"><span data-stu-id="7b273-157">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="7b273-158">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="7b273-158">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="7b273-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b273-159">DateTimeOffset</span></span>|<span data-ttu-id="7b273-160">Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям</span><span class="sxs-lookup"><span data-stu-id="7b273-160">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="7b273-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b273-161">Response</span></span>
<span data-ttu-id="7b273-162">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7b273-162">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b273-163">Пример</span><span class="sxs-lookup"><span data-stu-id="7b273-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b273-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b273-164">Request</span></span>
<span data-ttu-id="7b273-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b273-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7b273-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b273-166">Response</span></span>
<span data-ttu-id="7b273-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b273-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









