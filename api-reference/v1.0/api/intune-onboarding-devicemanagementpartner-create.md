---
title: Создание объекта deviceManagementPartner
description: Создание объекта deviceManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 34de40589542e74a8f2fec5347c12a3d32637e16
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959994"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="8e0ce-103">Создание объекта deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="8e0ce-103">Create deviceManagementPartner</span></span>

> <span data-ttu-id="8e0ce-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e0ce-105">Создание объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="8e0ce-105">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e0ce-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8e0ce-106">Prerequisites</span></span>
<span data-ttu-id="8e0ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e0ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e0ce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e0ce-109">Permission type</span></span>|<span data-ttu-id="8e0ce-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e0ce-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e0ce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e0ce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8e0ce-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e0ce-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8e0ce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e0ce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e0ce-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-114">Not supported.</span></span>|
|<span data-ttu-id="8e0ce-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e0ce-115">Application</span></span>|<span data-ttu-id="8e0ce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e0ce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e0ce-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="8e0ce-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e0ce-118">Request headers</span></span>
|<span data-ttu-id="8e0ce-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e0ce-119">Header</span></span>|<span data-ttu-id="8e0ce-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8e0ce-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e0ce-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e0ce-121">Authorization</span></span>|<span data-ttu-id="8e0ce-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e0ce-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8e0ce-123">Accept</span></span>|<span data-ttu-id="8e0ce-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8e0ce-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e0ce-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e0ce-125">Request body</span></span>
<span data-ttu-id="8e0ce-126">В теле запроса добавьте представление объекта deviceManagementPartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-126">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="8e0ce-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-127">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="8e0ce-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e0ce-128">Property</span></span>|<span data-ttu-id="8e0ce-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8e0ce-129">Type</span></span>|<span data-ttu-id="8e0ce-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8e0ce-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e0ce-131">id</span><span class="sxs-lookup"><span data-stu-id="8e0ce-131">id</span></span>|<span data-ttu-id="8e0ce-132">String</span><span class="sxs-lookup"><span data-stu-id="8e0ce-132">String</span></span>|<span data-ttu-id="8e0ce-133">Идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="8e0ce-133">Id of the entity</span></span>|
|<span data-ttu-id="8e0ce-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="8e0ce-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="8e0ce-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e0ce-135">DateTimeOffset</span></span>|<span data-ttu-id="8e0ce-136">Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".</span><span class="sxs-lookup"><span data-stu-id="8e0ce-136">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="8e0ce-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="8e0ce-137">partnerState</span></span>|[<span data-ttu-id="8e0ce-138">Девицеманажементпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="8e0ce-138">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="8e0ce-139">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-139">Partner state of this tenant.</span></span> <span data-ttu-id="8e0ce-140">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-140">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="8e0ce-141">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="8e0ce-141">partnerAppType</span></span>|[<span data-ttu-id="8e0ce-142">Девицеманажементпартнерапптипе</span><span class="sxs-lookup"><span data-stu-id="8e0ce-142">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="8e0ce-143">Тип партнерского приложения.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-143">Partner App type.</span></span> <span data-ttu-id="8e0ce-144">Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-144">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="8e0ce-145">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="8e0ce-145">singleTenantAppId</span></span>|<span data-ttu-id="8e0ce-146">String</span><span class="sxs-lookup"><span data-stu-id="8e0ce-146">String</span></span>|<span data-ttu-id="8e0ce-147">Идентификатор одноклиентского приложения партнера</span><span class="sxs-lookup"><span data-stu-id="8e0ce-147">Partner Single tenant App id</span></span>|
|<span data-ttu-id="8e0ce-148">displayName</span><span class="sxs-lookup"><span data-stu-id="8e0ce-148">displayName</span></span>|<span data-ttu-id="8e0ce-149">String</span><span class="sxs-lookup"><span data-stu-id="8e0ce-149">String</span></span>|<span data-ttu-id="8e0ce-150">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="8e0ce-150">Partner display name</span></span>|
|<span data-ttu-id="8e0ce-151">isConfigured</span><span class="sxs-lookup"><span data-stu-id="8e0ce-151">isConfigured</span></span>|<span data-ttu-id="8e0ce-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e0ce-152">Boolean</span></span>|<span data-ttu-id="8e0ce-153">Указывает, настроен ли партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="8e0ce-153">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="8e0ce-154">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e0ce-154">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="8e0ce-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e0ce-155">DateTimeOffset</span></span>|<span data-ttu-id="8e0ce-156">Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства</span><span class="sxs-lookup"><span data-stu-id="8e0ce-156">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="8e0ce-157">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="8e0ce-157">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="8e0ce-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e0ce-158">DateTimeOffset</span></span>|<span data-ttu-id="8e0ce-159">Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям</span><span class="sxs-lookup"><span data-stu-id="8e0ce-159">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="8e0ce-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e0ce-160">Response</span></span>
<span data-ttu-id="8e0ce-161">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-161">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e0ce-162">Пример</span><span class="sxs-lookup"><span data-stu-id="8e0ce-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e0ce-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e0ce-163">Request</span></span>
<span data-ttu-id="8e0ce-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8e0ce-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e0ce-165">Response</span></span>
<span data-ttu-id="8e0ce-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e0ce-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



