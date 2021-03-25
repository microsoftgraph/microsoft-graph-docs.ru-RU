---
title: Обновление mobileThreatDefenseConnector
description: Обновление свойств объекта mobileThreatDefenseConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8de03a90555c5d80e10bf0c64bb408c12130cba8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156879"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="31516-103">Обновление mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="31516-103">Update mobileThreatDefenseConnector</span></span>

<span data-ttu-id="31516-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31516-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31516-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31516-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31516-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31516-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31516-107">Обновление свойств объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="31516-107">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31516-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="31516-108">Prerequisites</span></span>
<span data-ttu-id="31516-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31516-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31516-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31516-111">Permission type</span></span>|<span data-ttu-id="31516-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31516-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31516-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31516-113">Delegated (work or school account)</span></span>|<span data-ttu-id="31516-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31516-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="31516-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31516-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31516-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31516-116">Not supported.</span></span>|
|<span data-ttu-id="31516-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="31516-117">Application</span></span>|<span data-ttu-id="31516-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31516-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="31516-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31516-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="31516-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="31516-120">Request headers</span></span>
|<span data-ttu-id="31516-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="31516-121">Header</span></span>|<span data-ttu-id="31516-122">Значение</span><span class="sxs-lookup"><span data-stu-id="31516-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31516-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="31516-123">Authorization</span></span>|<span data-ttu-id="31516-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31516-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31516-125">Accept</span><span class="sxs-lookup"><span data-stu-id="31516-125">Accept</span></span>|<span data-ttu-id="31516-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31516-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31516-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31516-127">Request body</span></span>
<span data-ttu-id="31516-128">В теле запроса добавьте представление объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31516-128">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="31516-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="31516-129">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="31516-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="31516-130">Property</span></span>|<span data-ttu-id="31516-131">Тип</span><span class="sxs-lookup"><span data-stu-id="31516-131">Type</span></span>|<span data-ttu-id="31516-132">Описание</span><span class="sxs-lookup"><span data-stu-id="31516-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31516-133">id</span><span class="sxs-lookup"><span data-stu-id="31516-133">id</span></span>|<span data-ttu-id="31516-134">Строка</span><span class="sxs-lookup"><span data-stu-id="31516-134">String</span></span>|<span data-ttu-id="31516-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="31516-135">Not yet documented</span></span>|
|<span data-ttu-id="31516-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="31516-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="31516-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31516-137">DateTimeOffset</span></span>|<span data-ttu-id="31516-138">Дата и время последнего подтверждения соединения, полученные от партнера по синхронизации данных</span><span class="sxs-lookup"><span data-stu-id="31516-138">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="31516-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="31516-139">partnerState</span></span>|[<span data-ttu-id="31516-140">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="31516-140">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="31516-141">Состояние Партнера синхронизации данных для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="31516-141">Data Sync Partner state for this account.</span></span> <span data-ttu-id="31516-142">Возможные значения: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="31516-142">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="31516-143">AndroidMobileApplicationManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="31516-143">androidMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="31516-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="31516-144">Boolean</span></span>|<span data-ttu-id="31516-145">Для Android установите, следует ли использовать данные партнера синхронизации данных во время оценок управления мобильными приложениями (MAM).</span><span class="sxs-lookup"><span data-stu-id="31516-145">For Android, set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="31516-146">Для оценки управления мобильными приложениями (MAM) может быть включен только один партнер на платформе.</span><span class="sxs-lookup"><span data-stu-id="31516-146">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="31516-147">iosMobileApplicationManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="31516-147">iosMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="31516-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="31516-148">Boolean</span></span>|<span data-ttu-id="31516-149">Для IOS получите или установите, следует ли использовать данные партнера синхронизации данных во время оценок управления мобильными приложениями (MAM).</span><span class="sxs-lookup"><span data-stu-id="31516-149">For IOS, get or set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="31516-150">Для оценки управления мобильными приложениями (MAM) может быть включен только один партнер на платформе.</span><span class="sxs-lookup"><span data-stu-id="31516-150">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="31516-151">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="31516-151">androidEnabled</span></span>|<span data-ttu-id="31516-152">Логическое</span><span class="sxs-lookup"><span data-stu-id="31516-152">Boolean</span></span>|<span data-ttu-id="31516-153">Для ОС Android следует указать в настройках, необходимо ли использовать данные партнера по синхронизации данных в ходе оценки соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="31516-153">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="31516-154">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="31516-154">iosEnabled</span></span>|<span data-ttu-id="31516-155">Логическое</span><span class="sxs-lookup"><span data-stu-id="31516-155">Boolean</span></span>|<span data-ttu-id="31516-156">Для ОС IOS следует получить или задать настройки, необходимо ли использовать данные партнера по синхронизации данных в ходе оценок соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="31516-156">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="31516-157">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="31516-157">windowsEnabled</span></span>|<span data-ttu-id="31516-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="31516-158">Boolean</span></span>|<span data-ttu-id="31516-159">Для Windows получите или установите, следует ли использовать данные партнера синхронизации данных во время оценки соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="31516-159">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="31516-160">macEnabled</span><span class="sxs-lookup"><span data-stu-id="31516-160">macEnabled</span></span>|<span data-ttu-id="31516-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="31516-161">Boolean</span></span>|<span data-ttu-id="31516-162">Для Mac получите или установите, следует ли использовать данные партнера синхронизации данных во время оценки соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="31516-162">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="31516-163">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="31516-163">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="31516-164">Логическое</span><span class="sxs-lookup"><span data-stu-id="31516-164">Boolean</span></span>|<span data-ttu-id="31516-165">Для ОС Android следует указать, необходимо ли Intune получать данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям</span><span class="sxs-lookup"><span data-stu-id="31516-165">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="31516-166">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="31516-166">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="31516-167">Логическое</span><span class="sxs-lookup"><span data-stu-id="31516-167">Boolean</span></span>|<span data-ttu-id="31516-168">Для ОС IOS следует указать, необходимо ли Intune получать данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям</span><span class="sxs-lookup"><span data-stu-id="31516-168">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="31516-169">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="31516-169">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="31516-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="31516-170">Boolean</span></span>|<span data-ttu-id="31516-171">Для Windows установите, должен ли Intune получать данные от партнера синхронизации данных до маркировки устройства, удовлетворяемой требованиям.</span><span class="sxs-lookup"><span data-stu-id="31516-171">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="31516-172">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="31516-172">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="31516-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="31516-173">Boolean</span></span>|<span data-ttu-id="31516-174">Для Mac получите или установите, должен ли Intune получать данные от партнера по синхронизации данных до маркировки устройства, удовлетворяемой требованиям.</span><span class="sxs-lookup"><span data-stu-id="31516-174">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="31516-175">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="31516-175">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="31516-176">Логическое</span><span class="sxs-lookup"><span data-stu-id="31516-176">Boolean</span></span>|<span data-ttu-id="31516-177">Получение или задание настроек, следует ли блокировать устройства на включенных платформах, которые не соответствуют минимальным требованиям к версии партнера по синхронизации данных</span><span class="sxs-lookup"><span data-stu-id="31516-177">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="31516-178">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="31516-178">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="31516-179">Int32</span><span class="sxs-lookup"><span data-stu-id="31516-179">Int32</span></span>|<span data-ttu-id="31516-180">Получает или задает количество дней устойчивости к отсутствию отклика для клиента при этой интеграции партнера.</span><span class="sxs-lookup"><span data-stu-id="31516-180">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="31516-181">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="31516-181">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="31516-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="31516-182">Boolean</span></span>|<span data-ttu-id="31516-183">Для устройств IOS администратор может настроить, может ли партнер синхронизации данных также собирать метаданные об установленных приложениях из Intune.</span><span class="sxs-lookup"><span data-stu-id="31516-183">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="31516-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="31516-184">Response</span></span>
<span data-ttu-id="31516-185">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="31516-185">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31516-186">Пример</span><span class="sxs-lookup"><span data-stu-id="31516-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="31516-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="31516-187">Request</span></span>
<span data-ttu-id="31516-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31516-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
Content-type: application/json
Content-length: 726

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidMobileApplicationManagementEnabled": true,
  "iosMobileApplicationManagementEnabled": true,
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

### <a name="response"></a><span data-ttu-id="31516-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="31516-189">Response</span></span>
<span data-ttu-id="31516-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31516-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 775

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidMobileApplicationManagementEnabled": true,
  "iosMobileApplicationManagementEnabled": true,
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




