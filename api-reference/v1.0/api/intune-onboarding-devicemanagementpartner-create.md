---
title: Создание объекта deviceManagementPartner
description: Создание объекта deviceManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f9b3d09c3c22bf13e887a17ef9eb62c8d3a786de
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866159"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="1b85c-103">Создание объекта deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="1b85c-103">Create deviceManagementPartner</span></span>

> <span data-ttu-id="1b85c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1b85c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b85c-105">Создание объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="1b85c-105">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1b85c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1b85c-106">Prerequisites</span></span>
<span data-ttu-id="1b85c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b85c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b85c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b85c-109">Permission type</span></span>|<span data-ttu-id="1b85c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b85c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b85c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b85c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1b85c-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b85c-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1b85c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b85c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b85c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b85c-114">Not supported.</span></span>|
|<span data-ttu-id="1b85c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b85c-115">Application</span></span>|<span data-ttu-id="1b85c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b85c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b85c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b85c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="1b85c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b85c-118">Request headers</span></span>
|<span data-ttu-id="1b85c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b85c-119">Header</span></span>|<span data-ttu-id="1b85c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1b85c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b85c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b85c-121">Authorization</span></span>|<span data-ttu-id="1b85c-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1b85c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b85c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1b85c-123">Accept</span></span>|<span data-ttu-id="1b85c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1b85c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b85c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1b85c-125">Request body</span></span>
<span data-ttu-id="1b85c-126">В теле запроса добавьте представление объекта deviceManagementPartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b85c-126">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="1b85c-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="1b85c-127">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="1b85c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b85c-128">Property</span></span>|<span data-ttu-id="1b85c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="1b85c-129">Type</span></span>|<span data-ttu-id="1b85c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="1b85c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b85c-131">id</span><span class="sxs-lookup"><span data-stu-id="1b85c-131">id</span></span>|<span data-ttu-id="1b85c-132">Строка</span><span class="sxs-lookup"><span data-stu-id="1b85c-132">String</span></span>|<span data-ttu-id="1b85c-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1b85c-133">Not yet documented</span></span>|
|<span data-ttu-id="1b85c-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="1b85c-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="1b85c-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b85c-135">DateTimeOffset</span></span>|<span data-ttu-id="1b85c-136">Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".</span><span class="sxs-lookup"><span data-stu-id="1b85c-136">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="1b85c-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="1b85c-137">partnerState</span></span>|[<span data-ttu-id="1b85c-138">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="1b85c-138">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="1b85c-139">Состояние партнера клиента.</span><span class="sxs-lookup"><span data-stu-id="1b85c-139">Partner state of this tenant.</span></span> <span data-ttu-id="1b85c-140">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="1b85c-140">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="1b85c-141">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="1b85c-141">partnerAppType</span></span>|[<span data-ttu-id="1b85c-142">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="1b85c-142">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="1b85c-143">Партнерские типа приложения.</span><span class="sxs-lookup"><span data-stu-id="1b85c-143">Partner App type.</span></span> <span data-ttu-id="1b85c-144">Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="1b85c-144">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="1b85c-145">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="1b85c-145">singleTenantAppId</span></span>|<span data-ttu-id="1b85c-146">String</span><span class="sxs-lookup"><span data-stu-id="1b85c-146">String</span></span>|<span data-ttu-id="1b85c-147">Идентификатор одноклиентского приложения партнера</span><span class="sxs-lookup"><span data-stu-id="1b85c-147">Partner Single tenant App id</span></span>|
|<span data-ttu-id="1b85c-148">displayName</span><span class="sxs-lookup"><span data-stu-id="1b85c-148">displayName</span></span>|<span data-ttu-id="1b85c-149">String</span><span class="sxs-lookup"><span data-stu-id="1b85c-149">String</span></span>|<span data-ttu-id="1b85c-150">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="1b85c-150">Partner display name</span></span>|
|<span data-ttu-id="1b85c-151">isConfigured</span><span class="sxs-lookup"><span data-stu-id="1b85c-151">isConfigured</span></span>|<span data-ttu-id="1b85c-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b85c-152">Boolean</span></span>|<span data-ttu-id="1b85c-153">Указывает, настроен ли партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="1b85c-153">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="1b85c-154">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b85c-154">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="1b85c-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b85c-155">DateTimeOffset</span></span>|<span data-ttu-id="1b85c-156">Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства.</span><span class="sxs-lookup"><span data-stu-id="1b85c-156">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="1b85c-157">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="1b85c-157">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="1b85c-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b85c-158">DateTimeOffset</span></span>|<span data-ttu-id="1b85c-159">Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям.</span><span class="sxs-lookup"><span data-stu-id="1b85c-159">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="1b85c-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b85c-160">Response</span></span>
<span data-ttu-id="1b85c-161">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1b85c-161">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b85c-162">Пример</span><span class="sxs-lookup"><span data-stu-id="1b85c-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="1b85c-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b85c-163">Request</span></span>
<span data-ttu-id="1b85c-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b85c-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1b85c-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b85c-165">Response</span></span>
<span data-ttu-id="1b85c-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1b85c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



