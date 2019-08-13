---
title: Обновление объекта deviceManagementPartner
description: Обновление свойств объекта deviceManagementPartner.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 479dc7206de2da5a9172233b6d37b1298824fb25
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352653"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="f0517-103">Обновление объекта deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="f0517-103">Update deviceManagementPartner</span></span>

> <span data-ttu-id="f0517-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0517-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0517-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0517-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0517-106">Обновление свойств объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="f0517-106">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0517-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f0517-107">Prerequisites</span></span>
<span data-ttu-id="f0517-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0517-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0517-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0517-110">Permission type</span></span>|<span data-ttu-id="f0517-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0517-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0517-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0517-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f0517-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0517-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f0517-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0517-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0517-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0517-115">Not supported.</span></span>|
|<span data-ttu-id="f0517-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0517-116">Application</span></span>|<span data-ttu-id="f0517-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0517-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0517-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0517-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="f0517-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0517-119">Request headers</span></span>
|<span data-ttu-id="f0517-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0517-120">Header</span></span>|<span data-ttu-id="f0517-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f0517-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0517-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0517-122">Authorization</span></span>|<span data-ttu-id="f0517-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0517-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0517-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f0517-124">Accept</span></span>|<span data-ttu-id="f0517-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f0517-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0517-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f0517-126">Request body</span></span>
<span data-ttu-id="f0517-127">В теле запроса добавьте представление объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0517-127">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="f0517-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="f0517-128">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="f0517-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0517-129">Property</span></span>|<span data-ttu-id="f0517-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f0517-130">Type</span></span>|<span data-ttu-id="f0517-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f0517-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0517-132">id</span><span class="sxs-lookup"><span data-stu-id="f0517-132">id</span></span>|<span data-ttu-id="f0517-133">String</span><span class="sxs-lookup"><span data-stu-id="f0517-133">String</span></span>|<span data-ttu-id="f0517-134">Идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="f0517-134">Id of the entity</span></span>|
|<span data-ttu-id="f0517-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="f0517-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="f0517-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0517-136">DateTimeOffset</span></span>|<span data-ttu-id="f0517-137">Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".</span><span class="sxs-lookup"><span data-stu-id="f0517-137">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="f0517-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="f0517-138">partnerState</span></span>|[<span data-ttu-id="f0517-139">девицеманажементпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="f0517-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="f0517-140">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="f0517-140">Partner state of this tenant.</span></span> <span data-ttu-id="f0517-141">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="f0517-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="f0517-142">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="f0517-142">partnerAppType</span></span>|[<span data-ttu-id="f0517-143">девицеманажементпартнерапптипе</span><span class="sxs-lookup"><span data-stu-id="f0517-143">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="f0517-144">Тип партнерского приложения.</span><span class="sxs-lookup"><span data-stu-id="f0517-144">Partner App type.</span></span> <span data-ttu-id="f0517-145">Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="f0517-145">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="f0517-146">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="f0517-146">singleTenantAppId</span></span>|<span data-ttu-id="f0517-147">String</span><span class="sxs-lookup"><span data-stu-id="f0517-147">String</span></span>|<span data-ttu-id="f0517-148">Идентификатор одноклиентского приложения партнера</span><span class="sxs-lookup"><span data-stu-id="f0517-148">Partner Single tenant App id</span></span>|
|<span data-ttu-id="f0517-149">displayName</span><span class="sxs-lookup"><span data-stu-id="f0517-149">displayName</span></span>|<span data-ttu-id="f0517-150">Строка</span><span class="sxs-lookup"><span data-stu-id="f0517-150">String</span></span>|<span data-ttu-id="f0517-151">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="f0517-151">Partner display name</span></span>|
|<span data-ttu-id="f0517-152">isConfigured</span><span class="sxs-lookup"><span data-stu-id="f0517-152">isConfigured</span></span>|<span data-ttu-id="f0517-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0517-153">Boolean</span></span>|<span data-ttu-id="f0517-154">Указывает, настроен ли партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="f0517-154">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="f0517-155">вхенпартнердевицесвиллберемовед</span><span class="sxs-lookup"><span data-stu-id="f0517-155">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="f0517-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0517-156">DateTimeOffset</span></span>|<span data-ttu-id="f0517-157">Дата и время в формате UTC, когда партнерские устройства будет удален.</span><span class="sxs-lookup"><span data-stu-id="f0517-157">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="f0517-158">Это скоро станет обселете.</span><span class="sxs-lookup"><span data-stu-id="f0517-158">This will become obselete soon.</span></span>|
|<span data-ttu-id="f0517-159">вхенпартнердевицесвиллбемаркедаснонкомплиант</span><span class="sxs-lookup"><span data-stu-id="f0517-159">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="f0517-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0517-160">DateTimeOffset</span></span>|<span data-ttu-id="f0517-161">Дата и время в формате UTC, когда партнерские устройства будет помечен как несоответствующий.</span><span class="sxs-lookup"><span data-stu-id="f0517-161">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="f0517-162">Это скоро станет обселете.</span><span class="sxs-lookup"><span data-stu-id="f0517-162">This will become obselete soon.</span></span>|
|<span data-ttu-id="f0517-163">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0517-163">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="f0517-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0517-164">DateTimeOffset</span></span>|<span data-ttu-id="f0517-165">Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства</span><span class="sxs-lookup"><span data-stu-id="f0517-165">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="f0517-166">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="f0517-166">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="f0517-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0517-167">DateTimeOffset</span></span>|<span data-ttu-id="f0517-168">Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям</span><span class="sxs-lookup"><span data-stu-id="f0517-168">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="f0517-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0517-169">Response</span></span>
<span data-ttu-id="f0517-170">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f0517-170">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0517-171">Пример</span><span class="sxs-lookup"><span data-stu-id="f0517-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0517-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0517-172">Request</span></span>
<span data-ttu-id="f0517-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0517-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 664

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
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```

### <a name="response"></a><span data-ttu-id="f0517-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0517-174">Response</span></span>
<span data-ttu-id="f0517-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0517-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 713

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
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```






