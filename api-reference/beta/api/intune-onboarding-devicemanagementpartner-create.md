---
title: Создание объекта deviceManagementPartner
description: Создание объекта deviceManagementPartner.
author: tfitzmac
ms.openlocfilehash: f8778ff23ed5990e1749bc36122587ef20488417
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333553"
---
# <a name="create-devicemanagementpartner"></a><span data-ttu-id="cecd3-103">Создание объекта deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="cecd3-103">Create deviceManagementPartner</span></span>

> <span data-ttu-id="cecd3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cecd3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cecd3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cecd3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cecd3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cecd3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cecd3-107">Создание объекта [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="cecd3-107">Create a new [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cecd3-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cecd3-108">Prerequisites</span></span>
<span data-ttu-id="cecd3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cecd3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cecd3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cecd3-111">Permission type</span></span>|<span data-ttu-id="cecd3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cecd3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cecd3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cecd3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cecd3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cecd3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cecd3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cecd3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cecd3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cecd3-116">Not supported.</span></span>|
|<span data-ttu-id="cecd3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cecd3-117">Application</span></span>|<span data-ttu-id="cecd3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cecd3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cecd3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cecd3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="cecd3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cecd3-120">Request headers</span></span>
|<span data-ttu-id="cecd3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cecd3-121">Header</span></span>|<span data-ttu-id="cecd3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cecd3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cecd3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cecd3-123">Authorization</span></span>|<span data-ttu-id="cecd3-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cecd3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cecd3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cecd3-125">Accept</span></span>|<span data-ttu-id="cecd3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cecd3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cecd3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cecd3-127">Request body</span></span>
<span data-ttu-id="cecd3-128">В теле запроса добавьте представление объекта deviceManagementPartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cecd3-128">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="cecd3-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="cecd3-129">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="cecd3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cecd3-130">Property</span></span>|<span data-ttu-id="cecd3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cecd3-131">Type</span></span>|<span data-ttu-id="cecd3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cecd3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cecd3-133">id</span><span class="sxs-lookup"><span data-stu-id="cecd3-133">id</span></span>|<span data-ttu-id="cecd3-134">Строка</span><span class="sxs-lookup"><span data-stu-id="cecd3-134">String</span></span>|<span data-ttu-id="cecd3-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cecd3-135">Not yet documented</span></span>|
|<span data-ttu-id="cecd3-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="cecd3-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="cecd3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cecd3-137">DateTimeOffset</span></span>|<span data-ttu-id="cecd3-138">Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".</span><span class="sxs-lookup"><span data-stu-id="cecd3-138">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="cecd3-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="cecd3-139">partnerState</span></span>|[<span data-ttu-id="cecd3-140">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="cecd3-140">deviceManagementPartnerTenantState</span></span>](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|<span data-ttu-id="cecd3-141">Состояние партнера клиента.</span><span class="sxs-lookup"><span data-stu-id="cecd3-141">Partner state of this tenant.</span></span> <span data-ttu-id="cecd3-142">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="cecd3-142">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="cecd3-143">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="cecd3-143">partnerAppType</span></span>|[<span data-ttu-id="cecd3-144">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="cecd3-144">deviceManagementPartnerAppType</span></span>](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|<span data-ttu-id="cecd3-145">Партнерские типа приложения.</span><span class="sxs-lookup"><span data-stu-id="cecd3-145">Partner App type.</span></span> <span data-ttu-id="cecd3-146">Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="cecd3-146">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="cecd3-147">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="cecd3-147">singleTenantAppId</span></span>|<span data-ttu-id="cecd3-148">String</span><span class="sxs-lookup"><span data-stu-id="cecd3-148">String</span></span>|<span data-ttu-id="cecd3-149">Идентификатор одноклиентского приложения партнера</span><span class="sxs-lookup"><span data-stu-id="cecd3-149">Partner Single tenant App id</span></span>|
|<span data-ttu-id="cecd3-150">displayName</span><span class="sxs-lookup"><span data-stu-id="cecd3-150">displayName</span></span>|<span data-ttu-id="cecd3-151">String</span><span class="sxs-lookup"><span data-stu-id="cecd3-151">String</span></span>|<span data-ttu-id="cecd3-152">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="cecd3-152">Partner display name</span></span>|
|<span data-ttu-id="cecd3-153">isConfigured</span><span class="sxs-lookup"><span data-stu-id="cecd3-153">isConfigured</span></span>|<span data-ttu-id="cecd3-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="cecd3-154">Boolean</span></span>|<span data-ttu-id="cecd3-155">Указывает, настроен ли партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="cecd3-155">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="cecd3-156">whenPartnerDevicesWillBeRemoved</span><span class="sxs-lookup"><span data-stu-id="cecd3-156">whenPartnerDevicesWillBeRemoved</span></span>|<span data-ttu-id="cecd3-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cecd3-157">DateTimeOffset</span></span>|<span data-ttu-id="cecd3-158">Дата и время в формате UTC, когда PartnerDevices будут удалены.</span><span class="sxs-lookup"><span data-stu-id="cecd3-158">DateTime in UTC when PartnerDevices will be removed.</span></span> <span data-ttu-id="cecd3-159">Это значение станет obselete ближайшее время.</span><span class="sxs-lookup"><span data-stu-id="cecd3-159">This will become obselete soon.</span></span>|
|<span data-ttu-id="cecd3-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span><span class="sxs-lookup"><span data-stu-id="cecd3-160">whenPartnerDevicesWillBeMarkedAsNonCompliant</span></span>|<span data-ttu-id="cecd3-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cecd3-161">DateTimeOffset</span></span>|<span data-ttu-id="cecd3-162">Дата и время в формате UTC, когда PartnerDevices будут помечены как не соответствует.</span><span class="sxs-lookup"><span data-stu-id="cecd3-162">DateTime in UTC when PartnerDevices will be marked as NonCompliant.</span></span> <span data-ttu-id="cecd3-163">Это значение станет obselete ближайшее время.</span><span class="sxs-lookup"><span data-stu-id="cecd3-163">This will become obselete soon.</span></span>|
|<span data-ttu-id="cecd3-164">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="cecd3-164">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="cecd3-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cecd3-165">DateTimeOffset</span></span>|<span data-ttu-id="cecd3-166">Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства.</span><span class="sxs-lookup"><span data-stu-id="cecd3-166">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="cecd3-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="cecd3-167">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="cecd3-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cecd3-168">DateTimeOffset</span></span>|<span data-ttu-id="cecd3-169">Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям.</span><span class="sxs-lookup"><span data-stu-id="cecd3-169">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="cecd3-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="cecd3-170">Response</span></span>
<span data-ttu-id="cecd3-171">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cecd3-171">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cecd3-172">Пример</span><span class="sxs-lookup"><span data-stu-id="cecd3-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="cecd3-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="cecd3-173">Request</span></span>
<span data-ttu-id="cecd3-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cecd3-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cecd3-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="cecd3-175">Response</span></span>
<span data-ttu-id="cecd3-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cecd3-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





