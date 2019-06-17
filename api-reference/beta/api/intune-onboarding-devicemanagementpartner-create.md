---
title: Создание объекта deviceManagementPartner
description: Создание объекта deviceManagementPartner.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d8cf972806c246c033bef95f26bff7d55a5d9c44
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34980994"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="569f9-103">Создание объекта deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="569f9-103">Create deviceManagementPartner</span></span>

> <span data-ttu-id="569f9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="569f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="569f9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="569f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="569f9-106">Создание объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="569f9-106">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="569f9-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="569f9-107">Prerequisites</span></span>
<span data-ttu-id="569f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="569f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="569f9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="569f9-110">Permission type</span></span>|<span data-ttu-id="569f9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="569f9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="569f9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="569f9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="569f9-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="569f9-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="569f9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="569f9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="569f9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="569f9-115">Not supported.</span></span>|
|<span data-ttu-id="569f9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="569f9-116">Application</span></span>|<span data-ttu-id="569f9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="569f9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="569f9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="569f9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="569f9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="569f9-119">Request headers</span></span>
|<span data-ttu-id="569f9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="569f9-120">Header</span></span>|<span data-ttu-id="569f9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="569f9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="569f9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="569f9-122">Authorization</span></span>|<span data-ttu-id="569f9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="569f9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="569f9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="569f9-124">Accept</span></span>|<span data-ttu-id="569f9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="569f9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="569f9-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="569f9-126">Request body</span></span>
<span data-ttu-id="569f9-127">В теле запроса добавьте представление объекта deviceManagementPartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="569f9-127">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="569f9-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="569f9-128">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="569f9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="569f9-129">Property</span></span>|<span data-ttu-id="569f9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="569f9-130">Type</span></span>|<span data-ttu-id="569f9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="569f9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="569f9-132">id</span><span class="sxs-lookup"><span data-stu-id="569f9-132">id</span></span>|<span data-ttu-id="569f9-133">String</span><span class="sxs-lookup"><span data-stu-id="569f9-133">String</span></span>|<span data-ttu-id="569f9-134">Идентификатор объекта</span><span class="sxs-lookup"><span data-stu-id="569f9-134">Id of the entity</span></span>|
|<span data-ttu-id="569f9-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="569f9-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="569f9-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="569f9-136">DateTimeOffset</span></span>|<span data-ttu-id="569f9-137">Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".</span><span class="sxs-lookup"><span data-stu-id="569f9-137">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="569f9-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="569f9-138">partnerState</span></span>|[<span data-ttu-id="569f9-139">Девицеманажементпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="569f9-139">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="569f9-140">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="569f9-140">Partner state of this tenant.</span></span> <span data-ttu-id="569f9-141">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="569f9-141">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="569f9-142">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="569f9-142">partnerAppType</span></span>|[<span data-ttu-id="569f9-143">Девицеманажементпартнерапптипе</span><span class="sxs-lookup"><span data-stu-id="569f9-143">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="569f9-144">Тип партнерского приложения.</span><span class="sxs-lookup"><span data-stu-id="569f9-144">Partner App type.</span></span> <span data-ttu-id="569f9-145">Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="569f9-145">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="569f9-146">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="569f9-146">singleTenantAppId</span></span>|<span data-ttu-id="569f9-147">String</span><span class="sxs-lookup"><span data-stu-id="569f9-147">String</span></span>|<span data-ttu-id="569f9-148">Идентификатор одноклиентского приложения партнера</span><span class="sxs-lookup"><span data-stu-id="569f9-148">Partner Single tenant App id</span></span>|
|<span data-ttu-id="569f9-149">displayName</span><span class="sxs-lookup"><span data-stu-id="569f9-149">displayName</span></span>|<span data-ttu-id="569f9-150">Строка</span><span class="sxs-lookup"><span data-stu-id="569f9-150">String</span></span>|<span data-ttu-id="569f9-151">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="569f9-151">Partner display name</span></span>|
|<span data-ttu-id="569f9-152">isConfigured</span><span class="sxs-lookup"><span data-stu-id="569f9-152">isConfigured</span></span>|<span data-ttu-id="569f9-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="569f9-153">Boolean</span></span>|<span data-ttu-id="569f9-154">Указывает, настроен ли партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="569f9-154">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="569f9-155">Вхенпартнердевицесвиллберемовед</span><span class="sxs-lookup"><span data-stu-id="569f9-155">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="569f9-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="569f9-156">DateTimeOffset</span></span>|<span data-ttu-id="569f9-157">Дата и время в формате UTC, когда партнерские устройства будет удален.</span><span class="sxs-lookup"><span data-stu-id="569f9-157">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="569f9-158">Это скоро станет обселете.</span><span class="sxs-lookup"><span data-stu-id="569f9-158">This will become obselete soon.</span></span>|
|<span data-ttu-id="569f9-159">Вхенпартнердевицесвиллбемаркедаснонкомплиант</span><span class="sxs-lookup"><span data-stu-id="569f9-159">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="569f9-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="569f9-160">DateTimeOffset</span></span>|<span data-ttu-id="569f9-161">Дата и время в формате UTC, когда партнерские устройства будет помечен как несоответствующий.</span><span class="sxs-lookup"><span data-stu-id="569f9-161">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="569f9-162">Это скоро станет обселете.</span><span class="sxs-lookup"><span data-stu-id="569f9-162">This will become obselete soon.</span></span>|
|<span data-ttu-id="569f9-163">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="569f9-163">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="569f9-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="569f9-164">DateTimeOffset</span></span>|<span data-ttu-id="569f9-165">Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства</span><span class="sxs-lookup"><span data-stu-id="569f9-165">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="569f9-166">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="569f9-166">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="569f9-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="569f9-167">DateTimeOffset</span></span>|<span data-ttu-id="569f9-168">Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям</span><span class="sxs-lookup"><span data-stu-id="569f9-168">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="569f9-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="569f9-169">Response</span></span>
<span data-ttu-id="569f9-170">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="569f9-170">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="569f9-171">Пример</span><span class="sxs-lookup"><span data-stu-id="569f9-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="569f9-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="569f9-172">Request</span></span>
<span data-ttu-id="569f9-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="569f9-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
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

### <a name="response"></a><span data-ttu-id="569f9-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="569f9-174">Response</span></span>
<span data-ttu-id="569f9-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="569f9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





