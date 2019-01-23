---
title: Обновление объекта deviceManagementPartner
description: Обновление свойств объекта deviceManagementPartner.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 65a90c85a29340643858fe1166f4bbfbf690035b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421727"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="42bb4-103">Обновление объекта deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="42bb4-103">Update deviceManagementPartner</span></span>

> <span data-ttu-id="42bb4-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="42bb4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="42bb4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42bb4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42bb4-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42bb4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42bb4-107">Обновление свойств объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="42bb4-107">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42bb4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="42bb4-108">Prerequisites</span></span>
<span data-ttu-id="42bb4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="42bb4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="42bb4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42bb4-111">Permission type</span></span>|<span data-ttu-id="42bb4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42bb4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42bb4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42bb4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42bb4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42bb4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="42bb4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42bb4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42bb4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42bb4-116">Not supported.</span></span>|
|<span data-ttu-id="42bb4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42bb4-117">Application</span></span>|<span data-ttu-id="42bb4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42bb4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42bb4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42bb4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="42bb4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42bb4-120">Request headers</span></span>
|<span data-ttu-id="42bb4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42bb4-121">Header</span></span>|<span data-ttu-id="42bb4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="42bb4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42bb4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42bb4-123">Authorization</span></span>|<span data-ttu-id="42bb4-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="42bb4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42bb4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="42bb4-125">Accept</span></span>|<span data-ttu-id="42bb4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42bb4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42bb4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42bb4-127">Request body</span></span>
<span data-ttu-id="42bb4-128">В теле запроса добавьте представление объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42bb4-128">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="42bb4-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="42bb4-129">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="42bb4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="42bb4-130">Property</span></span>|<span data-ttu-id="42bb4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="42bb4-131">Type</span></span>|<span data-ttu-id="42bb4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="42bb4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42bb4-133">id</span><span class="sxs-lookup"><span data-stu-id="42bb4-133">id</span></span>|<span data-ttu-id="42bb4-134">String</span><span class="sxs-lookup"><span data-stu-id="42bb4-134">String</span></span>|<span data-ttu-id="42bb4-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="42bb4-135">Not yet documented</span></span>|
|<span data-ttu-id="42bb4-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="42bb4-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="42bb4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42bb4-137">DateTimeOffset</span></span>|<span data-ttu-id="42bb4-138">Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".</span><span class="sxs-lookup"><span data-stu-id="42bb4-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="42bb4-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="42bb4-139">partnerState</span></span>|[<span data-ttu-id="42bb4-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="42bb4-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="42bb4-141">Состояние партнера клиента.</span><span class="sxs-lookup"><span data-stu-id="42bb4-141">Partner state of this tenant.</span></span> <span data-ttu-id="42bb4-142">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="42bb4-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="42bb4-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="42bb4-143">partnerAppType</span></span>|[<span data-ttu-id="42bb4-144">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="42bb4-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="42bb4-145">Партнерские типа приложения.</span><span class="sxs-lookup"><span data-stu-id="42bb4-145">Partner App type.</span></span> <span data-ttu-id="42bb4-146">Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="42bb4-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="42bb4-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="42bb4-147">singleTenantAppId</span></span>|<span data-ttu-id="42bb4-148">String</span><span class="sxs-lookup"><span data-stu-id="42bb4-148">String</span></span>|<span data-ttu-id="42bb4-149">Идентификатор одноклиентского приложения партнера</span><span class="sxs-lookup"><span data-stu-id="42bb4-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="42bb4-150">displayName</span><span class="sxs-lookup"><span data-stu-id="42bb4-150">displayName</span></span>|<span data-ttu-id="42bb4-151">String</span><span class="sxs-lookup"><span data-stu-id="42bb4-151">String</span></span>|<span data-ttu-id="42bb4-152">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="42bb4-152">Partner display name</span></span>|
|<span data-ttu-id="42bb4-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="42bb4-153">isConfigured</span></span>|<span data-ttu-id="42bb4-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="42bb4-154">Boolean</span></span>|<span data-ttu-id="42bb4-155">Указывает, настроен ли партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="42bb4-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="42bb4-156">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="42bb4-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="42bb4-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42bb4-157">DateTimeOffset</span></span>|<span data-ttu-id="42bb4-158">Дата и время в формате UTC, когда PartnerDevices будут удалены.</span><span class="sxs-lookup"><span data-stu-id="42bb4-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="42bb4-159">Это значение станет obselete ближайшее время.</span><span class="sxs-lookup"><span data-stu-id="42bb4-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="42bb4-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="42bb4-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="42bb4-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42bb4-161">DateTimeOffset</span></span>|<span data-ttu-id="42bb4-162">Дата и время в формате UTC, когда PartnerDevices будут помечены как не соответствует.</span><span class="sxs-lookup"><span data-stu-id="42bb4-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="42bb4-163">Это значение станет obselete ближайшее время.</span><span class="sxs-lookup"><span data-stu-id="42bb4-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="42bb4-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="42bb4-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="42bb4-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42bb4-165">DateTimeOffset</span></span>|<span data-ttu-id="42bb4-166">Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства.</span><span class="sxs-lookup"><span data-stu-id="42bb4-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="42bb4-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="42bb4-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="42bb4-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42bb4-168">DateTimeOffset</span></span>|<span data-ttu-id="42bb4-169">Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям.</span><span class="sxs-lookup"><span data-stu-id="42bb4-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="42bb4-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="42bb4-170">Response</span></span>
<span data-ttu-id="42bb4-171">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="42bb4-171">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42bb4-172">Пример</span><span class="sxs-lookup"><span data-stu-id="42bb4-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="42bb4-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="42bb4-173">Request</span></span>
<span data-ttu-id="42bb4-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42bb4-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="42bb4-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="42bb4-175">Response</span></span>
<span data-ttu-id="42bb4-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="42bb4-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




