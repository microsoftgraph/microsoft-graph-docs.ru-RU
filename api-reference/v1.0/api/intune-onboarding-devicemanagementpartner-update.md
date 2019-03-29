---
title: Обновление объекта deviceManagementPartner
description: Обновление свойств объекта deviceManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb90210e753becbee984cc9c809e3cbdee089bee
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968408"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="c4f88-103">Обновление объекта deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="c4f88-103">Update deviceManagementPartner</span></span>

> <span data-ttu-id="c4f88-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4f88-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4f88-105">Обновление свойств объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="c4f88-105">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4f88-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c4f88-106">Prerequisites</span></span>
<span data-ttu-id="c4f88-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4f88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4f88-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4f88-109">Permission type</span></span>|<span data-ttu-id="c4f88-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4f88-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4f88-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4f88-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c4f88-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4f88-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c4f88-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4f88-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4f88-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4f88-114">Not supported.</span></span>|
|<span data-ttu-id="c4f88-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4f88-115">Application</span></span>|<span data-ttu-id="c4f88-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4f88-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4f88-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4f88-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="c4f88-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4f88-118">Request headers</span></span>
|<span data-ttu-id="c4f88-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4f88-119">Header</span></span>|<span data-ttu-id="c4f88-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c4f88-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4f88-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4f88-121">Authorization</span></span>|<span data-ttu-id="c4f88-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4f88-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4f88-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c4f88-123">Accept</span></span>|<span data-ttu-id="c4f88-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c4f88-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4f88-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4f88-125">Request body</span></span>
<span data-ttu-id="c4f88-126">В теле запроса добавьте представление объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4f88-126">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="c4f88-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="c4f88-127">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="c4f88-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4f88-128">Property</span></span>|<span data-ttu-id="c4f88-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c4f88-129">Type</span></span>|<span data-ttu-id="c4f88-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c4f88-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4f88-131">id</span><span class="sxs-lookup"><span data-stu-id="c4f88-131">id</span></span>|<span data-ttu-id="c4f88-132">String</span><span class="sxs-lookup"><span data-stu-id="c4f88-132">String</span></span>|<span data-ttu-id="c4f88-133">Идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="c4f88-133">Id of the entity</span></span>|
|<span data-ttu-id="c4f88-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="c4f88-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="c4f88-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4f88-135">DateTimeOffset</span></span>|<span data-ttu-id="c4f88-136">Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".</span><span class="sxs-lookup"><span data-stu-id="c4f88-136">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="c4f88-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="c4f88-137">partnerState</span></span>|[<span data-ttu-id="c4f88-138">Девицеманажементпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="c4f88-138">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="c4f88-139">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="c4f88-139">Partner state of this tenant.</span></span> <span data-ttu-id="c4f88-140">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="c4f88-140">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="c4f88-141">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="c4f88-141">partnerAppType</span></span>|[<span data-ttu-id="c4f88-142">Девицеманажементпартнерапптипе</span><span class="sxs-lookup"><span data-stu-id="c4f88-142">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="c4f88-143">Тип партнерского приложения.</span><span class="sxs-lookup"><span data-stu-id="c4f88-143">Partner App type.</span></span> <span data-ttu-id="c4f88-144">Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="c4f88-144">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="c4f88-145">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="c4f88-145">singleTenantAppId</span></span>|<span data-ttu-id="c4f88-146">String</span><span class="sxs-lookup"><span data-stu-id="c4f88-146">String</span></span>|<span data-ttu-id="c4f88-147">Идентификатор одноклиентского приложения партнера</span><span class="sxs-lookup"><span data-stu-id="c4f88-147">Partner Single tenant App id</span></span>|
|<span data-ttu-id="c4f88-148">displayName</span><span class="sxs-lookup"><span data-stu-id="c4f88-148">displayName</span></span>|<span data-ttu-id="c4f88-149">String</span><span class="sxs-lookup"><span data-stu-id="c4f88-149">String</span></span>|<span data-ttu-id="c4f88-150">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="c4f88-150">Partner display name</span></span>|
|<span data-ttu-id="c4f88-151">isConfigured</span><span class="sxs-lookup"><span data-stu-id="c4f88-151">isConfigured</span></span>|<span data-ttu-id="c4f88-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4f88-152">Boolean</span></span>|<span data-ttu-id="c4f88-153">Указывает, настроен ли партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="c4f88-153">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="c4f88-154">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4f88-154">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="c4f88-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4f88-155">DateTimeOffset</span></span>|<span data-ttu-id="c4f88-156">Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства</span><span class="sxs-lookup"><span data-stu-id="c4f88-156">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="c4f88-157">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="c4f88-157">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="c4f88-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4f88-158">DateTimeOffset</span></span>|<span data-ttu-id="c4f88-159">Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям</span><span class="sxs-lookup"><span data-stu-id="c4f88-159">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="c4f88-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4f88-160">Response</span></span>
<span data-ttu-id="c4f88-161">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c4f88-161">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4f88-162">Пример</span><span class="sxs-lookup"><span data-stu-id="c4f88-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4f88-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4f88-163">Request</span></span>
<span data-ttu-id="c4f88-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4f88-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c4f88-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4f88-165">Response</span></span>
<span data-ttu-id="c4f88-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4f88-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



