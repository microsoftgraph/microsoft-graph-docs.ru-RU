---
title: Обновление mobileThreatDefenseConnector
description: Обновление свойств объекта mobileThreatDefenseConnector.
ms.openlocfilehash: f493a7c79c887d094a7cd5b4d913a78c880b6df0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025020"
---
# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="ff10a-103">Обновление mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="ff10a-103">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="ff10a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ff10a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff10a-105">Обновление свойств объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="ff10a-105">Update the properties of a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ff10a-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ff10a-106">Prerequisites</span></span>
<span data-ttu-id="ff10a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff10a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff10a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff10a-109">Permission type</span></span>|<span data-ttu-id="ff10a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff10a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff10a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff10a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ff10a-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff10a-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ff10a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff10a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff10a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff10a-114">Not supported.</span></span>|
|<span data-ttu-id="ff10a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff10a-115">Application</span></span>|<span data-ttu-id="ff10a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff10a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff10a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff10a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="ff10a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff10a-118">Request headers</span></span>
|<span data-ttu-id="ff10a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff10a-119">Header</span></span>|<span data-ttu-id="ff10a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ff10a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff10a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff10a-121">Authorization</span></span>|<span data-ttu-id="ff10a-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ff10a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff10a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ff10a-123">Accept</span></span>|<span data-ttu-id="ff10a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ff10a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff10a-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ff10a-125">Request body</span></span>
<span data-ttu-id="ff10a-126">В теле запроса добавьте представление объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff10a-126">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="ff10a-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="ff10a-127">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="ff10a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff10a-128">Property</span></span>|<span data-ttu-id="ff10a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ff10a-129">Type</span></span>|<span data-ttu-id="ff10a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ff10a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff10a-131">id</span><span class="sxs-lookup"><span data-stu-id="ff10a-131">id</span></span>|<span data-ttu-id="ff10a-132">String</span><span class="sxs-lookup"><span data-stu-id="ff10a-132">String</span></span>|<span data-ttu-id="ff10a-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ff10a-133">Not yet documented</span></span>|
|<span data-ttu-id="ff10a-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="ff10a-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="ff10a-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff10a-135">DateTimeOffset</span></span>|<span data-ttu-id="ff10a-136">Дата и время последнего подтверждения соединения, полученные от партнера по синхронизации данных</span><span class="sxs-lookup"><span data-stu-id="ff10a-136">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="ff10a-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="ff10a-137">partnerState</span></span>|[<span data-ttu-id="ff10a-138">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="ff10a-138">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="ff10a-139">Состояние партнера синхронизации данных для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="ff10a-139">Data Sync Partner state for this account.</span></span> <span data-ttu-id="ff10a-140">Возможные значения: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="ff10a-140">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="ff10a-141">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="ff10a-141">androidEnabled</span></span>|<span data-ttu-id="ff10a-142">Логическое</span><span class="sxs-lookup"><span data-stu-id="ff10a-142">Boolean</span></span>|<span data-ttu-id="ff10a-143">Для ОС Android следует указать, необходимо ли использовать данные партнера по синхронизации данных в ходе оценки соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="ff10a-143">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="ff10a-144">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="ff10a-144">iosEnabled</span></span>|<span data-ttu-id="ff10a-145">Логическое</span><span class="sxs-lookup"><span data-stu-id="ff10a-145">Boolean</span></span>|<span data-ttu-id="ff10a-146">Для ОС IOS следует указать, использовать ли данные партнера по синхронизации данных в ходе оценок соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="ff10a-146">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="ff10a-147">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="ff10a-147">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="ff10a-148">Логическое</span><span class="sxs-lookup"><span data-stu-id="ff10a-148">Boolean</span></span>|<span data-ttu-id="ff10a-149">Для ОС Android следует указать, получать ли Intune данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям</span><span class="sxs-lookup"><span data-stu-id="ff10a-149">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="ff10a-150">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="ff10a-150">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="ff10a-151">Логическое</span><span class="sxs-lookup"><span data-stu-id="ff10a-151">Boolean</span></span>|<span data-ttu-id="ff10a-152">Для ОС IOS следует указать, получать ли Intune данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям</span><span class="sxs-lookup"><span data-stu-id="ff10a-152">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="ff10a-153">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="ff10a-153">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="ff10a-154">Логическое</span><span class="sxs-lookup"><span data-stu-id="ff10a-154">Boolean</span></span>|<span data-ttu-id="ff10a-155">Получение или задание настроек, следует ли на включенных платформах блокировать устройства, которые не соответствуют минимальным требованиям партнера по синхронизации данных к версии</span><span class="sxs-lookup"><span data-stu-id="ff10a-155">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="ff10a-156">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="ff10a-156">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="ff10a-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ff10a-157">Int32</span></span>|<span data-ttu-id="ff10a-158">Получает или задает количество дней устойчивости к отсутствию отклика для клиента при этой интеграции партнера.</span><span class="sxs-lookup"><span data-stu-id="ff10a-158">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="ff10a-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff10a-159">Response</span></span>
<span data-ttu-id="ff10a-160">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ff10a-160">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff10a-161">Пример</span><span class="sxs-lookup"><span data-stu-id="ff10a-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff10a-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff10a-162">Request</span></span>
<span data-ttu-id="ff10a-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff10a-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ff10a-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff10a-164">Response</span></span>
<span data-ttu-id="ff10a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ff10a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



