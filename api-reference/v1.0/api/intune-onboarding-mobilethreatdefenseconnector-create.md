---
title: Создание объекта mobileThreatDefenseConnector
description: Создание объекта mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04fe51cc57e1671ab323b454ee4b796f04e62b1a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252247"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="4d097-103">Создание объекта mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="4d097-103">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="4d097-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d097-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d097-105">Создание объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="4d097-105">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d097-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4d097-106">Prerequisites</span></span>
<span data-ttu-id="4d097-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4d097-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4d097-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d097-109">Permission type</span></span>|<span data-ttu-id="4d097-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d097-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d097-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d097-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4d097-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d097-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4d097-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d097-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d097-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d097-114">Not supported.</span></span>|
|<span data-ttu-id="4d097-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4d097-115">Application</span></span>|<span data-ttu-id="4d097-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d097-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d097-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d097-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="4d097-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4d097-118">Request headers</span></span>
|<span data-ttu-id="4d097-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d097-119">Header</span></span>|<span data-ttu-id="4d097-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4d097-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d097-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d097-121">Authorization</span></span>|<span data-ttu-id="4d097-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4d097-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d097-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4d097-123">Accept</span></span>|<span data-ttu-id="4d097-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4d097-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d097-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d097-125">Request body</span></span>
<span data-ttu-id="4d097-126">В тексте запроса добавьте представление объекта mobileThreatDefenseConnector в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d097-126">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="4d097-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="4d097-127">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="4d097-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d097-128">Property</span></span>|<span data-ttu-id="4d097-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4d097-129">Type</span></span>|<span data-ttu-id="4d097-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4d097-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d097-131">id</span><span class="sxs-lookup"><span data-stu-id="4d097-131">id</span></span>|<span data-ttu-id="4d097-132">String</span><span class="sxs-lookup"><span data-stu-id="4d097-132">String</span></span>|<span data-ttu-id="4d097-133">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4d097-133">Not yet documented</span></span>|
|<span data-ttu-id="4d097-134">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="4d097-134">lastHeartbeatDateTime</span></span>|<span data-ttu-id="4d097-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d097-135">DateTimeOffset</span></span>|<span data-ttu-id="4d097-136">Дата и время последнего подтверждения соединения, полученные от партнера по синхронизации данных</span><span class="sxs-lookup"><span data-stu-id="4d097-136">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="4d097-137">partnerState</span><span class="sxs-lookup"><span data-stu-id="4d097-137">partnerState</span></span>|[<span data-ttu-id="4d097-138">Мобилесреатпартнертенантстате</span><span class="sxs-lookup"><span data-stu-id="4d097-138">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="4d097-139">Состояние партнера по синхронизации данных для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="4d097-139">Data Sync Partner state for this account.</span></span> <span data-ttu-id="4d097-140">Возможные значения: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="4d097-140">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="4d097-141">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="4d097-141">androidEnabled</span></span>|<span data-ttu-id="4d097-142">Логический</span><span class="sxs-lookup"><span data-stu-id="4d097-142">Boolean</span></span>|<span data-ttu-id="4d097-143">Для ОС Android следует указать, необходимо ли использовать данные партнера по синхронизации данных в ходе оценки соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="4d097-143">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="4d097-144">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="4d097-144">iosEnabled</span></span>|<span data-ttu-id="4d097-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d097-145">Boolean</span></span>|<span data-ttu-id="4d097-146">Для ОС IOS следует указать, использовать ли данные партнера по синхронизации данных в ходе оценок соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="4d097-146">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="4d097-147">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="4d097-147">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="4d097-148">Логический</span><span class="sxs-lookup"><span data-stu-id="4d097-148">Boolean</span></span>|<span data-ttu-id="4d097-149">Для ОС Android следует указать, получать ли Intune данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям</span><span class="sxs-lookup"><span data-stu-id="4d097-149">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="4d097-150">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="4d097-150">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="4d097-151">Логический</span><span class="sxs-lookup"><span data-stu-id="4d097-151">Boolean</span></span>|<span data-ttu-id="4d097-152">Для ОС IOS следует указать, получать ли Intune данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям</span><span class="sxs-lookup"><span data-stu-id="4d097-152">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="4d097-153">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="4d097-153">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="4d097-154">Логическое</span><span class="sxs-lookup"><span data-stu-id="4d097-154">Boolean</span></span>|<span data-ttu-id="4d097-155">Получение или задание настроек, следует ли на включенных платформах блокировать устройства, которые не соответствуют минимальным требованиям партнера по синхронизации данных к версии</span><span class="sxs-lookup"><span data-stu-id="4d097-155">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="4d097-156">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="4d097-156">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="4d097-157">Int32</span><span class="sxs-lookup"><span data-stu-id="4d097-157">Int32</span></span>|<span data-ttu-id="4d097-158">Получает или задает количество дней устойчивости к отсутствию отклика для клиента при этой интеграции партнера.</span><span class="sxs-lookup"><span data-stu-id="4d097-158">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="4d097-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d097-159">Response</span></span>
<span data-ttu-id="4d097-160">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4d097-160">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d097-161">Пример</span><span class="sxs-lookup"><span data-stu-id="4d097-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d097-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d097-162">Request</span></span>
<span data-ttu-id="4d097-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d097-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
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

### <a name="response"></a><span data-ttu-id="4d097-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="4d097-164">Response</span></span>
<span data-ttu-id="4d097-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4d097-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



