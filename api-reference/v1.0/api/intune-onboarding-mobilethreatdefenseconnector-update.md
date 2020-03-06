---
title: Обновление mobileThreatDefenseConnector
description: Обновление свойств объекта mobileThreatDefenseConnector.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d652e77b62c6020dd83ba9d2088c3bdd26b09a06
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512449"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="15cca-103">Обновление mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="15cca-103">Update mobileThreatDefenseConnector</span></span>

<span data-ttu-id="15cca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15cca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15cca-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15cca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15cca-106">Обновление свойств объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="15cca-106">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15cca-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="15cca-107">Prerequisites</span></span>
<span data-ttu-id="15cca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15cca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15cca-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15cca-110">Permission type</span></span>|<span data-ttu-id="15cca-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="15cca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15cca-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15cca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="15cca-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15cca-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="15cca-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15cca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15cca-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15cca-115">Not supported.</span></span>|
|<span data-ttu-id="15cca-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15cca-116">Application</span></span>|<span data-ttu-id="15cca-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15cca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15cca-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15cca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="15cca-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="15cca-119">Request headers</span></span>
|<span data-ttu-id="15cca-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15cca-120">Header</span></span>|<span data-ttu-id="15cca-121">Значение</span><span class="sxs-lookup"><span data-stu-id="15cca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15cca-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="15cca-122">Authorization</span></span>|<span data-ttu-id="15cca-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15cca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15cca-124">Accept</span><span class="sxs-lookup"><span data-stu-id="15cca-124">Accept</span></span>|<span data-ttu-id="15cca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="15cca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15cca-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15cca-126">Request body</span></span>
<span data-ttu-id="15cca-127">В теле запроса добавьте представление объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15cca-127">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="15cca-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="15cca-128">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="15cca-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="15cca-129">Property</span></span>|<span data-ttu-id="15cca-130">Тип</span><span class="sxs-lookup"><span data-stu-id="15cca-130">Type</span></span>|<span data-ttu-id="15cca-131">Описание</span><span class="sxs-lookup"><span data-stu-id="15cca-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15cca-132">id</span><span class="sxs-lookup"><span data-stu-id="15cca-132">id</span></span>|<span data-ttu-id="15cca-133">Строка</span><span class="sxs-lookup"><span data-stu-id="15cca-133">String</span></span>|<span data-ttu-id="15cca-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="15cca-134">Not yet documented</span></span>|
|<span data-ttu-id="15cca-135">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="15cca-135">lastHeartbeatDateTime</span></span>|<span data-ttu-id="15cca-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15cca-136">DateTimeOffset</span></span>|<span data-ttu-id="15cca-137">Дата и время последнего подтверждения соединения, полученные от партнера по синхронизации данных</span><span class="sxs-lookup"><span data-stu-id="15cca-137">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="15cca-138">partnerState</span><span class="sxs-lookup"><span data-stu-id="15cca-138">partnerState</span></span>|[<span data-ttu-id="15cca-139">мобилесреатпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="15cca-139">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="15cca-140">Состояние партнера по синхронизации данных для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="15cca-140">Data Sync Partner state for this account.</span></span> <span data-ttu-id="15cca-141">Возможные значения: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="15cca-141">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="15cca-142">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="15cca-142">androidEnabled</span></span>|<span data-ttu-id="15cca-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="15cca-143">Boolean</span></span>|<span data-ttu-id="15cca-144">Для ОС Android следует указать в настройках, необходимо ли использовать данные партнера по синхронизации данных в ходе оценки соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="15cca-144">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="15cca-145">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="15cca-145">iosEnabled</span></span>|<span data-ttu-id="15cca-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="15cca-146">Boolean</span></span>|<span data-ttu-id="15cca-147">Для ОС IOS следует получить или задать настройки, необходимо ли использовать данные партнера по синхронизации данных в ходе оценок соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="15cca-147">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="15cca-148">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="15cca-148">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="15cca-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="15cca-149">Boolean</span></span>|<span data-ttu-id="15cca-150">Для ОС Android следует указать, необходимо ли Intune получать данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям</span><span class="sxs-lookup"><span data-stu-id="15cca-150">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="15cca-151">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="15cca-151">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="15cca-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="15cca-152">Boolean</span></span>|<span data-ttu-id="15cca-153">Для ОС IOS следует указать, необходимо ли Intune получать данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям</span><span class="sxs-lookup"><span data-stu-id="15cca-153">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="15cca-154">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="15cca-154">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="15cca-155">Логическое</span><span class="sxs-lookup"><span data-stu-id="15cca-155">Boolean</span></span>|<span data-ttu-id="15cca-156">Получение или задание настроек, следует ли блокировать устройства на включенных платформах, которые не соответствуют минимальным требованиям к версии партнера по синхронизации данных</span><span class="sxs-lookup"><span data-stu-id="15cca-156">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="15cca-157">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="15cca-157">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="15cca-158">Int32</span><span class="sxs-lookup"><span data-stu-id="15cca-158">Int32</span></span>|<span data-ttu-id="15cca-159">Получает или задает количество дней устойчивости к отсутствию отклика для клиента при этой интеграции партнера.</span><span class="sxs-lookup"><span data-stu-id="15cca-159">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="15cca-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="15cca-160">Response</span></span>
<span data-ttu-id="15cca-161">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="15cca-161">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15cca-162">Пример</span><span class="sxs-lookup"><span data-stu-id="15cca-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="15cca-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="15cca-163">Request</span></span>
<span data-ttu-id="15cca-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15cca-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
Content-type: application/json
Content-length: 414

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```

### <a name="response"></a><span data-ttu-id="15cca-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="15cca-165">Response</span></span>
<span data-ttu-id="15cca-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15cca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 463

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```




