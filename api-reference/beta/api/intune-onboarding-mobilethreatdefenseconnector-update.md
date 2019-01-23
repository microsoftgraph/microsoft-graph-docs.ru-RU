---
title: Обновление mobileThreatDefenseConnector
description: Обновление свойств объекта mobileThreatDefenseConnector.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c8ed44a29f3e56f602689b58e3f58071998cde21
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411213"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="73991-103">Обновление mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="73991-103">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="73991-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="73991-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="73991-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73991-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73991-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73991-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73991-107">Обновление свойств объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="73991-107">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73991-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="73991-108">Prerequisites</span></span>
<span data-ttu-id="73991-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="73991-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="73991-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73991-111">Permission type</span></span>|<span data-ttu-id="73991-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73991-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73991-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73991-113">Delegated (work or school account)</span></span>|<span data-ttu-id="73991-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73991-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="73991-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73991-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73991-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73991-116">Not supported.</span></span>|
|<span data-ttu-id="73991-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73991-117">Application</span></span>|<span data-ttu-id="73991-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73991-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73991-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73991-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="73991-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73991-120">Request headers</span></span>
|<span data-ttu-id="73991-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73991-121">Header</span></span>|<span data-ttu-id="73991-122">Значение</span><span class="sxs-lookup"><span data-stu-id="73991-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73991-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="73991-123">Authorization</span></span>|<span data-ttu-id="73991-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="73991-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73991-125">Accept</span><span class="sxs-lookup"><span data-stu-id="73991-125">Accept</span></span>|<span data-ttu-id="73991-126">application/json</span><span class="sxs-lookup"><span data-stu-id="73991-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73991-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="73991-127">Request body</span></span>
<span data-ttu-id="73991-128">В теле запроса добавьте представление объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73991-128">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="73991-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="73991-129">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="73991-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="73991-130">Property</span></span>|<span data-ttu-id="73991-131">Тип</span><span class="sxs-lookup"><span data-stu-id="73991-131">Type</span></span>|<span data-ttu-id="73991-132">Описание</span><span class="sxs-lookup"><span data-stu-id="73991-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73991-133">id</span><span class="sxs-lookup"><span data-stu-id="73991-133">id</span></span>|<span data-ttu-id="73991-134">String</span><span class="sxs-lookup"><span data-stu-id="73991-134">String</span></span>|<span data-ttu-id="73991-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="73991-135">Not yet documented</span></span>|
|<span data-ttu-id="73991-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="73991-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="73991-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73991-137">DateTimeOffset</span></span>|<span data-ttu-id="73991-138">Дата и время последнего подтверждения соединения, полученные от партнера по синхронизации данных</span><span class="sxs-lookup"><span data-stu-id="73991-138">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="73991-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="73991-139">partnerState</span></span>|[<span data-ttu-id="73991-140">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="73991-140">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="73991-141">Состояние партнера синхронизации данных для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="73991-141">Data Sync Partner state for this account.</span></span> <span data-ttu-id="73991-142">Возможные значения: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="73991-142">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="73991-143">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="73991-143">androidEnabled</span></span>|<span data-ttu-id="73991-144">Логическое</span><span class="sxs-lookup"><span data-stu-id="73991-144">Boolean</span></span>|<span data-ttu-id="73991-145">Для ОС Android следует указать, необходимо ли использовать данные партнера по синхронизации данных в ходе оценки соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="73991-145">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="73991-146">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="73991-146">iosEnabled</span></span>|<span data-ttu-id="73991-147">Логическое</span><span class="sxs-lookup"><span data-stu-id="73991-147">Boolean</span></span>|<span data-ttu-id="73991-148">Для ОС IOS следует указать, использовать ли данные партнера по синхронизации данных в ходе оценок соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="73991-148">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="73991-149">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="73991-149">windowsEnabled</span></span>|<span data-ttu-id="73991-150">Логический</span><span class="sxs-lookup"><span data-stu-id="73991-150">Boolean</span></span>|<span data-ttu-id="73991-151">Для Windows получить или задать ли данные из партнер синхронизации данных можно использовать во время оценки соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="73991-151">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="73991-152">macEnabled</span><span class="sxs-lookup"><span data-stu-id="73991-152">macEnabled</span></span>|<span data-ttu-id="73991-153">Логический</span><span class="sxs-lookup"><span data-stu-id="73991-153">Boolean</span></span>|<span data-ttu-id="73991-154">Для Mac получить или задать ли данные из партнер синхронизации данных можно использовать во время оценки соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="73991-154">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="73991-155">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="73991-155">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="73991-156">Логическое</span><span class="sxs-lookup"><span data-stu-id="73991-156">Boolean</span></span>|<span data-ttu-id="73991-157">Для ОС Android следует указать, получать ли Intune данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям</span><span class="sxs-lookup"><span data-stu-id="73991-157">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="73991-158">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="73991-158">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="73991-159">Логическое</span><span class="sxs-lookup"><span data-stu-id="73991-159">Boolean</span></span>|<span data-ttu-id="73991-160">Для ОС IOS следует указать, получать ли Intune данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям</span><span class="sxs-lookup"><span data-stu-id="73991-160">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="73991-161">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="73991-161">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="73991-162">Логический</span><span class="sxs-lookup"><span data-stu-id="73991-162">Boolean</span></span>|<span data-ttu-id="73991-163">Для Windows установите ли Intune необходимо получать данные из партнер синхронизации данных до пометки совместимые устройства</span><span class="sxs-lookup"><span data-stu-id="73991-163">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="73991-164">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="73991-164">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="73991-165">Логический</span><span class="sxs-lookup"><span data-stu-id="73991-165">Boolean</span></span>|<span data-ttu-id="73991-166">Для Mac получить или задать ли Intune необходимо получать данные из партнер синхронизации данных до пометки совместимые устройства</span><span class="sxs-lookup"><span data-stu-id="73991-166">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="73991-167">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="73991-167">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="73991-168">Логическое</span><span class="sxs-lookup"><span data-stu-id="73991-168">Boolean</span></span>|<span data-ttu-id="73991-169">Получение или задание настроек, следует ли на включенных платформах блокировать устройства, которые не соответствуют минимальным требованиям партнера по синхронизации данных к версии</span><span class="sxs-lookup"><span data-stu-id="73991-169">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="73991-170">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="73991-170">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="73991-171">Int32</span><span class="sxs-lookup"><span data-stu-id="73991-171">Int32</span></span>|<span data-ttu-id="73991-172">Получает или задает количество дней устойчивости к отсутствию отклика для клиента при этой интеграции партнера.</span><span class="sxs-lookup"><span data-stu-id="73991-172">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="73991-173">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="73991-173">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="73991-174">Логический</span><span class="sxs-lookup"><span data-stu-id="73991-174">Boolean</span></span>|<span data-ttu-id="73991-175">Для операций ввода-ВЫВОДА устройств позволяет администратору настроить ли партнер синхронизации данных также может собирать метаданные об установленных приложениях из Intune</span><span class="sxs-lookup"><span data-stu-id="73991-175">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="73991-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="73991-176">Response</span></span>
<span data-ttu-id="73991-177">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="73991-177">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73991-178">Пример</span><span class="sxs-lookup"><span data-stu-id="73991-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="73991-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="73991-179">Request</span></span>
<span data-ttu-id="73991-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73991-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
Content-type: application/json
Content-length: 622

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "windowsEnabled": true,
  "macEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "windowsDeviceBlockedOnMissingPartnerData": true,
  "macDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6,
  "allowPartnerToCollectIOSApplicationMetadata": true
}
```

### <a name="response"></a><span data-ttu-id="73991-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="73991-181">Response</span></span>
<span data-ttu-id="73991-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="73991-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 671

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "windowsEnabled": true,
  "macEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "windowsDeviceBlockedOnMissingPartnerData": true,
  "macDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6,
  "allowPartnerToCollectIOSApplicationMetadata": true
}
```




