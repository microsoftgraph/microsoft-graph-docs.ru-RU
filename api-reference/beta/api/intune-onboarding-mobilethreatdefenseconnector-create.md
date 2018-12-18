---
title: Создание объекта mobileThreatDefenseConnector
description: Создание объекта mobileThreatDefenseConnector.
author: tfitzmac
ms.openlocfilehash: e77b4684f2f330441b8d9ec1f7b14e8e788835a9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330984"
---
# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="2527d-103">Создание объекта mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="2527d-103">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="2527d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2527d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2527d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2527d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2527d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2527d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2527d-107">Создание объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="2527d-107">Create a new [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2527d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2527d-108">Prerequisites</span></span>
<span data-ttu-id="2527d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2527d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2527d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2527d-111">Permission type</span></span>|<span data-ttu-id="2527d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2527d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2527d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2527d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2527d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2527d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2527d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2527d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2527d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2527d-116">Not supported.</span></span>|
|<span data-ttu-id="2527d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2527d-117">Application</span></span>|<span data-ttu-id="2527d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2527d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2527d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2527d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="2527d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2527d-120">Request headers</span></span>
|<span data-ttu-id="2527d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2527d-121">Header</span></span>|<span data-ttu-id="2527d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2527d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2527d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2527d-123">Authorization</span></span>|<span data-ttu-id="2527d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2527d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2527d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2527d-125">Accept</span></span>|<span data-ttu-id="2527d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2527d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2527d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2527d-127">Request body</span></span>
<span data-ttu-id="2527d-128">В тексте запроса добавьте представление объекта mobileThreatDefenseConnector в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2527d-128">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="2527d-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="2527d-129">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="2527d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2527d-130">Property</span></span>|<span data-ttu-id="2527d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2527d-131">Type</span></span>|<span data-ttu-id="2527d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2527d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2527d-133">id</span><span class="sxs-lookup"><span data-stu-id="2527d-133">id</span></span>|<span data-ttu-id="2527d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2527d-134">String</span></span>|<span data-ttu-id="2527d-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2527d-135">Not yet documented</span></span>|
|<span data-ttu-id="2527d-136">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="2527d-136">lastHeartbeatDateTime</span></span>|<span data-ttu-id="2527d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2527d-137">DateTimeOffset</span></span>|<span data-ttu-id="2527d-138">Дата и время последнего подтверждения соединения, полученные от партнера по синхронизации данных</span><span class="sxs-lookup"><span data-stu-id="2527d-138">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="2527d-139">partnerState</span><span class="sxs-lookup"><span data-stu-id="2527d-139">partnerState</span></span>|[<span data-ttu-id="2527d-140">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="2527d-140">mobileThreatPartnerTenantState</span></span>](../resources/intune-onboarding-mobilethreatpartnertenantstate.md)|<span data-ttu-id="2527d-141">Состояние партнера синхронизации данных для этой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="2527d-141">Data Sync Partner state for this account.</span></span> <span data-ttu-id="2527d-142">Возможные значения: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="2527d-142">Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="2527d-143">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="2527d-143">androidEnabled</span></span>|<span data-ttu-id="2527d-144">Логическое</span><span class="sxs-lookup"><span data-stu-id="2527d-144">Boolean</span></span>|<span data-ttu-id="2527d-145">Для ОС Android следует указать, необходимо ли использовать данные партнера по синхронизации данных в ходе оценки соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="2527d-145">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="2527d-146">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="2527d-146">iosEnabled</span></span>|<span data-ttu-id="2527d-147">Логическое</span><span class="sxs-lookup"><span data-stu-id="2527d-147">Boolean</span></span>|<span data-ttu-id="2527d-148">Для ОС IOS следует указать, использовать ли данные партнера по синхронизации данных в ходе оценок соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="2527d-148">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="2527d-149">windowsEnabled</span><span class="sxs-lookup"><span data-stu-id="2527d-149">windowsEnabled</span></span>|<span data-ttu-id="2527d-150">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2527d-150">Boolean</span></span>|<span data-ttu-id="2527d-151">Для Windows получить или задать ли данные из партнер синхронизации данных можно использовать во время оценки соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="2527d-151">For Windows, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="2527d-152">macEnabled</span><span class="sxs-lookup"><span data-stu-id="2527d-152">macEnabled</span></span>|<span data-ttu-id="2527d-153">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2527d-153">Boolean</span></span>|<span data-ttu-id="2527d-154">Для Mac получить или задать ли данные из партнер синхронизации данных можно использовать во время оценки соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="2527d-154">For Mac, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="2527d-155">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="2527d-155">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="2527d-156">Логическое</span><span class="sxs-lookup"><span data-stu-id="2527d-156">Boolean</span></span>|<span data-ttu-id="2527d-157">Для ОС Android следует указать, получать ли Intune данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям</span><span class="sxs-lookup"><span data-stu-id="2527d-157">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="2527d-158">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="2527d-158">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="2527d-159">Логическое</span><span class="sxs-lookup"><span data-stu-id="2527d-159">Boolean</span></span>|<span data-ttu-id="2527d-160">Для ОС IOS следует указать, получать ли Intune данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям</span><span class="sxs-lookup"><span data-stu-id="2527d-160">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="2527d-161">windowsDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="2527d-161">windowsDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="2527d-162">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2527d-162">Boolean</span></span>|<span data-ttu-id="2527d-163">Для Windows установите ли Intune необходимо получать данные из партнер синхронизации данных до пометки совместимые устройства</span><span class="sxs-lookup"><span data-stu-id="2527d-163">For Windows, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="2527d-164">macDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="2527d-164">macDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="2527d-165">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2527d-165">Boolean</span></span>|<span data-ttu-id="2527d-166">Для Mac получить или задать ли Intune необходимо получать данные из партнер синхронизации данных до пометки совместимые устройства</span><span class="sxs-lookup"><span data-stu-id="2527d-166">For Mac, get or set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="2527d-167">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="2527d-167">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="2527d-168">Логическое</span><span class="sxs-lookup"><span data-stu-id="2527d-168">Boolean</span></span>|<span data-ttu-id="2527d-169">Получение или задание настроек, следует ли на включенных платформах блокировать устройства, которые не соответствуют минимальным требованиям партнера по синхронизации данных к версии</span><span class="sxs-lookup"><span data-stu-id="2527d-169">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="2527d-170">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="2527d-170">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="2527d-171">Int32</span><span class="sxs-lookup"><span data-stu-id="2527d-171">Int32</span></span>|<span data-ttu-id="2527d-172">Получает или задает количество дней устойчивости к отсутствию отклика для клиента при этой интеграции партнера.</span><span class="sxs-lookup"><span data-stu-id="2527d-172">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|
|<span data-ttu-id="2527d-173">allowPartnerToCollectIOSApplicationMetadata</span><span class="sxs-lookup"><span data-stu-id="2527d-173">allowPartnerToCollectIOSApplicationMetadata</span></span>|<span data-ttu-id="2527d-174">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2527d-174">Boolean</span></span>|<span data-ttu-id="2527d-175">Для операций ввода-ВЫВОДА устройств позволяет администратору настроить ли партнер синхронизации данных также может собирать метаданные об установленных приложениях из Intune</span><span class="sxs-lookup"><span data-stu-id="2527d-175">For IOS devices, allows the admin to configure whether the data sync partner may also collect metadata about installed applications from Intune</span></span>|



## <a name="response"></a><span data-ttu-id="2527d-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="2527d-176">Response</span></span>
<span data-ttu-id="2527d-177">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2527d-177">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2527d-178">Пример</span><span class="sxs-lookup"><span data-stu-id="2527d-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="2527d-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="2527d-179">Request</span></span>
<span data-ttu-id="2527d-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2527d-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors
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

### <a name="response"></a><span data-ttu-id="2527d-181">Ответ</span><span class="sxs-lookup"><span data-stu-id="2527d-181">Response</span></span>
<span data-ttu-id="2527d-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2527d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





