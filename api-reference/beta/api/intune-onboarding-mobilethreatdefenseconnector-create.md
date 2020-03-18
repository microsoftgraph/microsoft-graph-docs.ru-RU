---
title: Создание объекта mobileThreatDefenseConnector
description: Создание объекта mobileThreatDefenseConnector.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bb1904038341c02d1b17696ce0b2016876f8be5d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42802813"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="6f3f1-103">Создание объекта mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="6f3f1-103">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="6f3f1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f3f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f3f1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6f3f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f3f1-106">Создание объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="6f3f1-106">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f3f1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6f3f1-107">Prerequisites</span></span>
<span data-ttu-id="6f3f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f3f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f3f1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f3f1-110">Permission type</span></span>|<span data-ttu-id="6f3f1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f3f1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f3f1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f3f1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6f3f1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f3f1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6f3f1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f3f1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f3f1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f3f1-115">Not supported.</span></span>|
|<span data-ttu-id="6f3f1-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6f3f1-116">Application</span></span>|<span data-ttu-id="6f3f1-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f3f1-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f3f1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f3f1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="6f3f1-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6f3f1-119">Request headers</span></span>
|<span data-ttu-id="6f3f1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f3f1-120">Header</span></span>|<span data-ttu-id="6f3f1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6f3f1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f3f1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f3f1-122">Authorization</span></span>|<span data-ttu-id="6f3f1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f3f1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f3f1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6f3f1-124">Accept</span></span>|<span data-ttu-id="6f3f1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6f3f1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f3f1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f3f1-126">Request body</span></span>
<span data-ttu-id="6f3f1-127">В тексте запроса добавьте представление объекта mobileThreatDefenseConnector в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f3f1-127">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="6f3f1-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="6f3f1-128">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="6f3f1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f3f1-129">Property</span></span>|<span data-ttu-id="6f3f1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6f3f1-130">Type</span></span>|<span data-ttu-id="6f3f1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6f3f1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f3f1-132">id</span><span class="sxs-lookup"><span data-stu-id="6f3f1-132">id</span></span>|<span data-ttu-id="6f3f1-133">String</span><span class="sxs-lookup"><span data-stu-id="6f3f1-133">String</span></span>|<span data-ttu-id="6f3f1-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="6f3f1-134">Not yet documented</span></span>|
|<span data-ttu-id="6f3f1-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="6f3f1-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="6f3f1-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f3f1-136">DateTimeOffset</span></span>|<span data-ttu-id="6f3f1-137">Дата и время последнего подтверждения соединения, полученные от партнера по синхронизации данных</span><span class="sxs-lookup"><span data-stu-id="6f3f1-137">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="6f3f1-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="6f3f1-138">partnerState</span></span>|[<span data-ttu-id="6f3f1-139">мобилесреатпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="6f3f1-139">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="6f3f1-140">Состояние партнера по синхронизации данных для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="6f3f1-140">Data Sync Partner state for this account.</span></span> <span data-ttu-id="6f3f1-141">Возможные значения: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="6f3f1-141">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="6f3f1-142">андроидмобилеаппликатионманажементенаблед</span><span class="sxs-lookup"><span data-stu-id="6f3f1-142">androidMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="6f3f1-143">Логический</span><span class="sxs-lookup"><span data-stu-id="6f3f1-143">Boolean</span></span>|<span data-ttu-id="6f3f1-144">Для Android укажите, следует ли использовать данные партнера по синхронизации данных во время оценок управления мобильными приложениями (MAM).</span><span class="sxs-lookup"><span data-stu-id="6f3f1-144">For Android, set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="6f3f1-145">Для оценки управления мобильными приложениями (MAM) можно включить только один партнер на платформу.</span><span class="sxs-lookup"><span data-stu-id="6f3f1-145">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="6f3f1-146">иосмобилеаппликатионманажементенаблед</span><span class="sxs-lookup"><span data-stu-id="6f3f1-146">iosMobileApplicationManagementEnabled</span></span>|<span data-ttu-id="6f3f1-147">Логический</span><span class="sxs-lookup"><span data-stu-id="6f3f1-147">Boolean</span></span>|<span data-ttu-id="6f3f1-148">Для IOS необходимо получить или указать, следует ли использовать данные партнера по синхронизации данных во время оценок управления мобильными приложениями (MAM).</span><span class="sxs-lookup"><span data-stu-id="6f3f1-148">For IOS, get or set whether data from the data sync partner should be used during Mobile Application Management (MAM) evaluations.</span></span> <span data-ttu-id="6f3f1-149">Для оценки управления мобильными приложениями (MAM) можно включить только один партнер на платформу.</span><span class="sxs-lookup"><span data-stu-id="6f3f1-149">Only one partner per platform may be enabled for Mobile Application Management (MAM) evaluation.</span></span>|
|<span data-ttu-id="6f3f1-150">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="6f3f1-150">androidEnabled</span></span>|<span data-ttu-id="6f3f1-151">Логический</span><span class="sxs-lookup"><span data-stu-id="6f3f1-151">Boolean</span></span>|<span data-ttu-id="6f3f1-152">Для ОС Android следует указать в настройках, необходимо ли использовать данные партнера по синхронизации данных в ходе оценки соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="6f3f1-152">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="6f3f1-153">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="6f3f1-153">iosEnabled</span></span>|<span data-ttu-id="6f3f1-154">Логический</span><span class="sxs-lookup"><span data-stu-id="6f3f1-154">Boolean</span></span>|<span data-ttu-id="6f3f1-155">Для ОС IOS следует получить или задать настройки, необходимо ли использовать данные партнера по синхронизации данных в ходе оценок соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="6f3f1-155">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="6f3f1-156">виндовсенаблед</span><span class="sxs-lookup"><span data-stu-id="6f3f1-156">windowsEnabled</span></span>|<span data-ttu-id="6f3f1-157">Логический</span><span class="sxs-lookup"><span data-stu-id="6f3f1-157">Boolean</span></span>|<span data-ttu-id="6f3f1-158">В Windows вы можете получить или задать, следует ли использовать данные партнера по синхронизации данных в ходе оценок соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="6f3f1-158">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="6f3f1-159">маценаблед</span><span class="sxs-lookup"><span data-stu-id="6f3f1-159">macEnabled</span></span>|<span data-ttu-id="6f3f1-160">Логический</span><span class="sxs-lookup"><span data-stu-id="6f3f1-160">Boolean</span></span>|<span data-ttu-id="6f3f1-161">В случае Mac получает или задает значение, указывающее, следует ли использовать данные партнера по синхронизации данных в ходе оценок соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="6f3f1-161">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="6f3f1-162">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="6f3f1-162">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="6f3f1-163">Логический</span><span class="sxs-lookup"><span data-stu-id="6f3f1-163">Boolean</span></span>|<span data-ttu-id="6f3f1-164">Для ОС Android следует указать, необходимо ли Intune получать данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям</span><span class="sxs-lookup"><span data-stu-id="6f3f1-164">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="6f3f1-165">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="6f3f1-165">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="6f3f1-166">Логический</span><span class="sxs-lookup"><span data-stu-id="6f3f1-166">Boolean</span></span>|<span data-ttu-id="6f3f1-167">Для ОС IOS следует указать, необходимо ли Intune получать данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям</span><span class="sxs-lookup"><span data-stu-id="6f3f1-167">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="6f3f1-168">виндовсдевицеблоккедонмиссингпартнердата</span><span class="sxs-lookup"><span data-stu-id="6f3f1-168">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="6f3f1-169">Логический</span><span class="sxs-lookup"><span data-stu-id="6f3f1-169">Boolean</span></span>|<span data-ttu-id="6f3f1-170">В Windows укажите, должны ли Intune получать данные от партнера по синхронизации данных, прежде чем помечать соответствующие устройства</span><span class="sxs-lookup"><span data-stu-id="6f3f1-170">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="6f3f1-171">макдевицеблоккедонмиссингпартнердата</span><span class="sxs-lookup"><span data-stu-id="6f3f1-171">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="6f3f1-172">Логический</span><span class="sxs-lookup"><span data-stu-id="6f3f1-172">Boolean</span></span>|<span data-ttu-id="6f3f1-173">В случае Mac получает или задает значение, указывающее, должны ли Intune получать данные от партнера по синхронизации данных, прежде чем помечать соответствующие устройства</span><span class="sxs-lookup"><span data-stu-id="6f3f1-173">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="6f3f1-174">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="6f3f1-174">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="6f3f1-175">Логическое</span><span class="sxs-lookup"><span data-stu-id="6f3f1-175">Boolean</span></span>|<span data-ttu-id="6f3f1-176">Получение или задание настроек, следует ли блокировать устройства на включенных платформах, которые не соответствуют минимальным требованиям к версии партнера по синхронизации данных</span><span class="sxs-lookup"><span data-stu-id="6f3f1-176">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="6f3f1-177">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="6f3f1-177">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="6f3f1-178">Int32</span><span class="sxs-lookup"><span data-stu-id="6f3f1-178">Int32</span></span>|<span data-ttu-id="6f3f1-179">Получает или задает количество дней устойчивости к отсутствию отклика для клиента при этой интеграции партнера.</span><span class="sxs-lookup"><span data-stu-id="6f3f1-179">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="6f3f1-180">алловпартнертоколлектиосаппликатионметадата</span><span class="sxs-lookup"><span data-stu-id="6f3f1-180">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="6f3f1-181">Логический</span><span class="sxs-lookup"><span data-stu-id="6f3f1-181">Boolean</span></span>|<span data-ttu-id="6f3f1-182">Для устройств с IOS позволяет администратору настроить, может ли партнер по синхронизации данных собирать метаданные об установленных приложениях из Intune</span><span class="sxs-lookup"><span data-stu-id="6f3f1-182">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="6f3f1-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f3f1-183">Response</span></span>
<span data-ttu-id="6f3f1-184">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6f3f1-184">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f3f1-185">Пример</span><span class="sxs-lookup"><span data-stu-id="6f3f1-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f3f1-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f3f1-186">Request</span></span>
<span data-ttu-id="6f3f1-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f3f1-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors
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

### <a name="response"></a><span data-ttu-id="6f3f1-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f3f1-188">Response</span></span>
<span data-ttu-id="6f3f1-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f3f1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




