---
title: Обновление mobileThreatDefenseConnector
description: Обновление свойств объекта mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d420b41c4de711a501420ed0ec05b4f65f03a149
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776089"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="8d19e-103">Обновление mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="8d19e-103">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="8d19e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d19e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d19e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d19e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d19e-106">Обновление свойств объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="8d19e-106">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d19e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8d19e-107">Prerequisites</span></span>
<span data-ttu-id="8d19e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d19e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d19e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d19e-110">Permission type</span></span>|<span data-ttu-id="8d19e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d19e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d19e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d19e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d19e-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d19e-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8d19e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d19e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d19e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d19e-115">Not supported.</span></span>|
|<span data-ttu-id="8d19e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d19e-116">Application</span></span>|<span data-ttu-id="8d19e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d19e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d19e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d19e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="8d19e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d19e-119">Request headers</span></span>
|<span data-ttu-id="8d19e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d19e-120">Header</span></span>|<span data-ttu-id="8d19e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8d19e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d19e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d19e-122">Authorization</span></span>|<span data-ttu-id="8d19e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d19e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d19e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8d19e-124">Accept</span></span>|<span data-ttu-id="8d19e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8d19e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d19e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d19e-126">Request body</span></span>
<span data-ttu-id="8d19e-127">В теле запроса добавьте представление объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d19e-127">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="8d19e-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="8d19e-128">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="8d19e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d19e-129">Property</span></span>|<span data-ttu-id="8d19e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8d19e-130">Type</span></span>|<span data-ttu-id="8d19e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8d19e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d19e-132">id</span><span class="sxs-lookup"><span data-stu-id="8d19e-132">id</span></span>|<span data-ttu-id="8d19e-133">String</span><span class="sxs-lookup"><span data-stu-id="8d19e-133">String</span></span>|<span data-ttu-id="8d19e-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8d19e-134">Not yet documented</span></span>|
|<span data-ttu-id="8d19e-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="8d19e-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="8d19e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d19e-136">DateTimeOffset</span></span>|<span data-ttu-id="8d19e-137">Дата и время последнего подтверждения соединения, полученные от партнера по синхронизации данных</span><span class="sxs-lookup"><span data-stu-id="8d19e-137">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="8d19e-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="8d19e-138">partnerState</span></span>|[<span data-ttu-id="8d19e-139">Мобилесреатпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="8d19e-139">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="8d19e-140">Состояние партнера по синхронизации данных для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="8d19e-140">Data Sync Partner state for this account.</span></span> <span data-ttu-id="8d19e-141">Возможные значения: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="8d19e-141">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="8d19e-142">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="8d19e-142">androidEnabled</span></span>|<span data-ttu-id="8d19e-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d19e-143">Boolean</span></span>|<span data-ttu-id="8d19e-144">Для ОС Android следует указать в настройках, необходимо ли использовать данные партнера по синхронизации данных в ходе оценки соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="8d19e-144">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="8d19e-145">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="8d19e-145">iosEnabled</span></span>|<span data-ttu-id="8d19e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d19e-146">Boolean</span></span>|<span data-ttu-id="8d19e-147">Для ОС IOS следует получить или задать настройки, необходимо ли использовать данные партнера по синхронизации данных в ходе оценок соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="8d19e-147">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="8d19e-148">Виндовсенаблед</span><span class="sxs-lookup"><span data-stu-id="8d19e-148">windowsEnabled</span></span>|<span data-ttu-id="8d19e-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d19e-149">Boolean</span></span>|<span data-ttu-id="8d19e-150">В Windows вы можете получить или задать, следует ли использовать данные партнера по синхронизации данных в ходе оценок соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="8d19e-150">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="8d19e-151">Маценаблед</span><span class="sxs-lookup"><span data-stu-id="8d19e-151">macEnabled</span></span>|<span data-ttu-id="8d19e-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d19e-152">Boolean</span></span>|<span data-ttu-id="8d19e-153">В случае Mac получает или задает значение, указывающее, следует ли использовать данные партнера по синхронизации данных в ходе оценок соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="8d19e-153">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="8d19e-154">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="8d19e-154">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="8d19e-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d19e-155">Boolean</span></span>|<span data-ttu-id="8d19e-156">Для ОС Android следует указать, необходимо ли Intune получать данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям</span><span class="sxs-lookup"><span data-stu-id="8d19e-156">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="8d19e-157">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="8d19e-157">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="8d19e-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d19e-158">Boolean</span></span>|<span data-ttu-id="8d19e-159">Для ОС IOS следует указать, необходимо ли Intune получать данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям</span><span class="sxs-lookup"><span data-stu-id="8d19e-159">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="8d19e-160">Виндовсдевицеблоккедонмиссингпартнердата</span><span class="sxs-lookup"><span data-stu-id="8d19e-160">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="8d19e-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d19e-161">Boolean</span></span>|<span data-ttu-id="8d19e-162">В Windows укажите, должны ли Intune получать данные от партнера по синхронизации данных, прежде чем помечать соответствующие устройства</span><span class="sxs-lookup"><span data-stu-id="8d19e-162">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="8d19e-163">Макдевицеблоккедонмиссингпартнердата</span><span class="sxs-lookup"><span data-stu-id="8d19e-163">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="8d19e-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d19e-164">Boolean</span></span>|<span data-ttu-id="8d19e-165">В случае Mac получает или задает значение, указывающее, должны ли Intune получать данные от партнера по синхронизации данных, прежде чем помечать соответствующие устройства</span><span class="sxs-lookup"><span data-stu-id="8d19e-165">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="8d19e-166">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="8d19e-166">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="8d19e-167">Логическое</span><span class="sxs-lookup"><span data-stu-id="8d19e-167">Boolean</span></span>|<span data-ttu-id="8d19e-168">Получение или задание настроек, следует ли блокировать устройства на включенных платформах, которые не соответствуют минимальным требованиям к версии партнера по синхронизации данных</span><span class="sxs-lookup"><span data-stu-id="8d19e-168">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="8d19e-169">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="8d19e-169">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="8d19e-170">Int32</span><span class="sxs-lookup"><span data-stu-id="8d19e-170">Int32</span></span>|<span data-ttu-id="8d19e-171">Получает или задает количество дней устойчивости к отсутствию отклика для клиента при этой интеграции партнера.</span><span class="sxs-lookup"><span data-stu-id="8d19e-171">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="8d19e-172">Алловпартнертоколлектиосаппликатионметадата</span><span class="sxs-lookup"><span data-stu-id="8d19e-172">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="8d19e-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d19e-173">Boolean</span></span>|<span data-ttu-id="8d19e-174">Для устройств с IOS позволяет администратору настроить, может ли партнер по синхронизации данных собирать метаданные об установленных приложениях из Intune</span><span class="sxs-lookup"><span data-stu-id="8d19e-174">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="8d19e-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d19e-175">Response</span></span>
<span data-ttu-id="8d19e-176">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8d19e-176">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d19e-177">Пример</span><span class="sxs-lookup"><span data-stu-id="8d19e-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d19e-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d19e-178">Request</span></span>
<span data-ttu-id="8d19e-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d19e-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8d19e-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d19e-180">Response</span></span>
<span data-ttu-id="8d19e-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d19e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





