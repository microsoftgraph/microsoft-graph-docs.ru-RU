---
title: Обновление объекта deviceManagementPartner
description: Обновление свойств объекта deviceManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 83ba5bf2e022b6961182a8f8c1ac17dec79ed959
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843157"
---
# <a name="update-devicemanagementpartner"></a><span data-ttu-id="75756-103">Обновление объекта deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="75756-103">Update deviceManagementPartner</span></span>

> <span data-ttu-id="75756-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="75756-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75756-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75756-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="75756-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="75756-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75756-107">Обновление свойств объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="75756-107">Update the properties of a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="75756-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="75756-108">Prerequisites</span></span>
<span data-ttu-id="75756-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75756-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75756-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75756-111">Permission type</span></span>|<span data-ttu-id="75756-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75756-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75756-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75756-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75756-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75756-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="75756-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75756-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75756-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75756-116">Not supported.</span></span>|
|<span data-ttu-id="75756-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75756-117">Application</span></span>|<span data-ttu-id="75756-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75756-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75756-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75756-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="75756-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75756-120">Request headers</span></span>
|<span data-ttu-id="75756-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75756-121">Header</span></span>|<span data-ttu-id="75756-122">Значение</span><span class="sxs-lookup"><span data-stu-id="75756-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75756-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="75756-123">Authorization</span></span>|<span data-ttu-id="75756-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="75756-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75756-125">Accept</span><span class="sxs-lookup"><span data-stu-id="75756-125">Accept</span></span>|<span data-ttu-id="75756-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75756-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75756-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75756-127">Request body</span></span>
<span data-ttu-id="75756-128">В теле запроса добавьте представление объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75756-128">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="75756-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="75756-129">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>

|<span data-ttu-id="75756-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="75756-130">Property</span></span>|<span data-ttu-id="75756-131">Тип</span><span class="sxs-lookup"><span data-stu-id="75756-131">Type</span></span>|<span data-ttu-id="75756-132">Описание</span><span class="sxs-lookup"><span data-stu-id="75756-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75756-133">id</span><span class="sxs-lookup"><span data-stu-id="75756-133">id</span></span>|<span data-ttu-id="75756-134">Строка</span><span class="sxs-lookup"><span data-stu-id="75756-134">String</span></span>|<span data-ttu-id="75756-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="75756-135">Not yet documented</span></span>|
|<span data-ttu-id="75756-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="75756-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="75756-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75756-137">DateTimeOffset</span></span>|<span data-ttu-id="75756-138">Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".</span><span class="sxs-lookup"><span data-stu-id="75756-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="75756-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="75756-139">partnerState</span></span>|[<span data-ttu-id="75756-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="75756-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="75756-141">Состояние партнера клиента.</span><span class="sxs-lookup"><span data-stu-id="75756-141">Partner state of this tenant.</span></span> <span data-ttu-id="75756-142">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="75756-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="75756-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="75756-143">partnerAppType</span></span>|[<span data-ttu-id="75756-144">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="75756-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="75756-145">Партнерские типа приложения.</span><span class="sxs-lookup"><span data-stu-id="75756-145">Partner App type.</span></span> <span data-ttu-id="75756-146">Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="75756-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="75756-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="75756-147">singleTenantAppId</span></span>|<span data-ttu-id="75756-148">String</span><span class="sxs-lookup"><span data-stu-id="75756-148">String</span></span>|<span data-ttu-id="75756-149">Идентификатор одноклиентского приложения партнера</span><span class="sxs-lookup"><span data-stu-id="75756-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="75756-150">displayName</span><span class="sxs-lookup"><span data-stu-id="75756-150">displayName</span></span>|<span data-ttu-id="75756-151">String</span><span class="sxs-lookup"><span data-stu-id="75756-151">String</span></span>|<span data-ttu-id="75756-152">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="75756-152">Partner display name</span></span>|
|<span data-ttu-id="75756-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="75756-153">isConfigured</span></span>|<span data-ttu-id="75756-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="75756-154">Boolean</span></span>|<span data-ttu-id="75756-155">Указывает, настроен ли партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="75756-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="75756-156">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="75756-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="75756-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75756-157">DateTimeOffset</span></span>|<span data-ttu-id="75756-158">Дата и время в формате UTC, когда PartnerDevices будут удалены.</span><span class="sxs-lookup"><span data-stu-id="75756-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="75756-159">Это значение станет obselete ближайшее время.</span><span class="sxs-lookup"><span data-stu-id="75756-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="75756-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="75756-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="75756-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75756-161">DateTimeOffset</span></span>|<span data-ttu-id="75756-162">Дата и время в формате UTC, когда PartnerDevices будут помечены как не соответствует.</span><span class="sxs-lookup"><span data-stu-id="75756-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="75756-163">Это значение станет obselete ближайшее время.</span><span class="sxs-lookup"><span data-stu-id="75756-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="75756-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="75756-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="75756-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75756-165">DateTimeOffset</span></span>|<span data-ttu-id="75756-166">Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства.</span><span class="sxs-lookup"><span data-stu-id="75756-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="75756-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="75756-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="75756-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75756-168">DateTimeOffset</span></span>|<span data-ttu-id="75756-169">Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям.</span><span class="sxs-lookup"><span data-stu-id="75756-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="75756-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="75756-170">Response</span></span>
<span data-ttu-id="75756-171">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="75756-171">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75756-172">Пример</span><span class="sxs-lookup"><span data-stu-id="75756-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="75756-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="75756-173">Request</span></span>
<span data-ttu-id="75756-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75756-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 602

{
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

### <a name="response"></a><span data-ttu-id="75756-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="75756-175">Response</span></span>
<span data-ttu-id="75756-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="75756-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





