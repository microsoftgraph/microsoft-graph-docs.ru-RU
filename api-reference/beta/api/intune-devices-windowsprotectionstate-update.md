---
title: Обновление windowsProtectionState
description: Обновление свойств объекта windowsProtectionState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f315188c9a2b666f72af7b6a214a6de6cd6e6e79
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43378176"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="955fb-103">Обновление windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="955fb-103">Update windowsProtectionState</span></span>

<span data-ttu-id="955fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="955fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="955fb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="955fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="955fb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="955fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="955fb-107">Обновление свойств объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="955fb-107">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="955fb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="955fb-108">Prerequisites</span></span>
<span data-ttu-id="955fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="955fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="955fb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="955fb-111">Permission type</span></span>|<span data-ttu-id="955fb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="955fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="955fb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="955fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="955fb-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="955fb-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="955fb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="955fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="955fb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="955fb-116">Not supported.</span></span>|
|<span data-ttu-id="955fb-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="955fb-117">Application</span></span>|<span data-ttu-id="955fb-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="955fb-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="955fb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="955fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="955fb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="955fb-120">Request headers</span></span>
|<span data-ttu-id="955fb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="955fb-121">Header</span></span>|<span data-ttu-id="955fb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="955fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="955fb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="955fb-123">Authorization</span></span>|<span data-ttu-id="955fb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="955fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="955fb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="955fb-125">Accept</span></span>|<span data-ttu-id="955fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="955fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="955fb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="955fb-127">Request body</span></span>
<span data-ttu-id="955fb-128">В тексте запроса добавьте представление объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="955fb-128">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="955fb-129">В следующей таблице приведены свойства, необходимые при создании [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span><span class="sxs-lookup"><span data-stu-id="955fb-129">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="955fb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="955fb-130">Property</span></span>|<span data-ttu-id="955fb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="955fb-131">Type</span></span>|<span data-ttu-id="955fb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="955fb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="955fb-133">id</span><span class="sxs-lookup"><span data-stu-id="955fb-133">id</span></span>|<span data-ttu-id="955fb-134">String</span><span class="sxs-lookup"><span data-stu-id="955fb-134">String</span></span>|<span data-ttu-id="955fb-135">Уникальный идентификатор для объекта состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="955fb-135">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="955fb-136">Это идентификатор устройства для устройства.</span><span class="sxs-lookup"><span data-stu-id="955fb-136">This is device id of the device</span></span>|
|<span data-ttu-id="955fb-137">малварепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="955fb-137">malwareProtectionEnabled</span></span>|<span data-ttu-id="955fb-138">Логическое</span><span class="sxs-lookup"><span data-stu-id="955fb-138">Boolean</span></span>|<span data-ttu-id="955fb-139">Защита от вредоносных программ включена или нет</span><span class="sxs-lookup"><span data-stu-id="955fb-139">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="955fb-140">девицестате</span><span class="sxs-lookup"><span data-stu-id="955fb-140">deviceState</span></span>|[<span data-ttu-id="955fb-141">виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="955fb-141">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="955fb-142">Состояние компьютера (например, очистка или ожидание полного сканирования или Ожидание перезагрузки и т. д.).</span><span class="sxs-lookup"><span data-stu-id="955fb-142">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="955fb-143">Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="955fb-143">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="955fb-144">реалтимепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="955fb-144">realTimeProtectionEnabled</span></span>|<span data-ttu-id="955fb-145">Логическое</span><span class="sxs-lookup"><span data-stu-id="955fb-145">Boolean</span></span>|<span data-ttu-id="955fb-146">Защита в режиме реального времени включена или нет?</span><span class="sxs-lookup"><span data-stu-id="955fb-146">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="955fb-147">нетворкинспектионсистеменаблед</span><span class="sxs-lookup"><span data-stu-id="955fb-147">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="955fb-148">Логическое</span><span class="sxs-lookup"><span data-stu-id="955fb-148">Boolean</span></span>|<span data-ttu-id="955fb-149">Система проверки сети включена или нет?</span><span class="sxs-lookup"><span data-stu-id="955fb-149">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="955fb-150">куиккскановердуе</span><span class="sxs-lookup"><span data-stu-id="955fb-150">quickScanOverdue</span></span>|<span data-ttu-id="955fb-151">Логическое</span><span class="sxs-lookup"><span data-stu-id="955fb-151">Boolean</span></span>|<span data-ttu-id="955fb-152">Быстрая проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="955fb-152">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="955fb-153">фуллскановердуе</span><span class="sxs-lookup"><span data-stu-id="955fb-153">fullScanOverdue</span></span>|<span data-ttu-id="955fb-154">Логическое</span><span class="sxs-lookup"><span data-stu-id="955fb-154">Boolean</span></span>|<span data-ttu-id="955fb-155">Полная проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="955fb-155">Full scan overdue or not?</span></span>|
|<span data-ttu-id="955fb-156">сигнатуреупдатеовердуе</span><span class="sxs-lookup"><span data-stu-id="955fb-156">signatureUpdateOverdue</span></span>|<span data-ttu-id="955fb-157">Логическое</span><span class="sxs-lookup"><span data-stu-id="955fb-157">Boolean</span></span>|<span data-ttu-id="955fb-158">Подпись устарела или нет?</span><span class="sxs-lookup"><span data-stu-id="955fb-158">Signature out of date or not?</span></span>|
|<span data-ttu-id="955fb-159">ребутрекуиред</span><span class="sxs-lookup"><span data-stu-id="955fb-159">rebootRequired</span></span>|<span data-ttu-id="955fb-160">Логическое</span><span class="sxs-lookup"><span data-stu-id="955fb-160">Boolean</span></span>|<span data-ttu-id="955fb-161">Требуется перезагрузка или нет?</span><span class="sxs-lookup"><span data-stu-id="955fb-161">Reboot required or not?</span></span>|
|<span data-ttu-id="955fb-162">фуллсканрекуиред</span><span class="sxs-lookup"><span data-stu-id="955fb-162">fullScanRequired</span></span>|<span data-ttu-id="955fb-163">Логическое</span><span class="sxs-lookup"><span data-stu-id="955fb-163">Boolean</span></span>|<span data-ttu-id="955fb-164">Необходима полная проверка или нет?</span><span class="sxs-lookup"><span data-stu-id="955fb-164">Full scan required or not?</span></span>|
|<span data-ttu-id="955fb-165">енгиневерсион</span><span class="sxs-lookup"><span data-stu-id="955fb-165">engineVersion</span></span>|<span data-ttu-id="955fb-166">String</span><span class="sxs-lookup"><span data-stu-id="955fb-166">String</span></span>|<span data-ttu-id="955fb-167">Текущая версия модуля Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="955fb-167">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="955fb-168">сигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="955fb-168">signatureVersion</span></span>|<span data-ttu-id="955fb-169">String</span><span class="sxs-lookup"><span data-stu-id="955fb-169">String</span></span>|<span data-ttu-id="955fb-170">Текущая версия определений вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="955fb-170">Current malware definitions version</span></span>|
|<span data-ttu-id="955fb-171">антималвареверсион</span><span class="sxs-lookup"><span data-stu-id="955fb-171">antiMalwareVersion</span></span>|<span data-ttu-id="955fb-172">String</span><span class="sxs-lookup"><span data-stu-id="955fb-172">String</span></span>|<span data-ttu-id="955fb-173">Текущая версия защиты от вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="955fb-173">Current anti malware version</span></span>|
|<span data-ttu-id="955fb-174">ласткуиккскандатетиме</span><span class="sxs-lookup"><span data-stu-id="955fb-174">lastQuickScanDateTime</span></span>|<span data-ttu-id="955fb-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="955fb-175">DateTimeOffset</span></span>|<span data-ttu-id="955fb-176">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="955fb-176">Last quick scan datetime</span></span>|
|<span data-ttu-id="955fb-177">ластфуллскандатетиме</span><span class="sxs-lookup"><span data-stu-id="955fb-177">lastFullScanDateTime</span></span>|<span data-ttu-id="955fb-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="955fb-178">DateTimeOffset</span></span>|<span data-ttu-id="955fb-179">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="955fb-179">Last quick scan datetime</span></span>|
|<span data-ttu-id="955fb-180">ласткуиккскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="955fb-180">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="955fb-181">String</span><span class="sxs-lookup"><span data-stu-id="955fb-181">String</span></span>|<span data-ttu-id="955fb-182">Последняя версия подписи быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="955fb-182">Last quick scan signature version</span></span>|
|<span data-ttu-id="955fb-183">ластфуллскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="955fb-183">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="955fb-184">String</span><span class="sxs-lookup"><span data-stu-id="955fb-184">String</span></span>|<span data-ttu-id="955fb-185">Версия последней полной проверки подписи</span><span class="sxs-lookup"><span data-stu-id="955fb-185">Last full scan signature version</span></span>|
|<span data-ttu-id="955fb-186">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="955fb-186">lastReportedDateTime</span></span>|<span data-ttu-id="955fb-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="955fb-187">DateTimeOffset</span></span>|<span data-ttu-id="955fb-188">Последнее состояние работоспособности устройства в отчете о времени</span><span class="sxs-lookup"><span data-stu-id="955fb-188">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="955fb-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="955fb-189">Response</span></span>
<span data-ttu-id="955fb-190">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="955fb-190">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="955fb-191">Пример</span><span class="sxs-lookup"><span data-stu-id="955fb-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="955fb-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="955fb-192">Request</span></span>
<span data-ttu-id="955fb-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="955fb-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
Content-type: application/json
Content-length: 865

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```

### <a name="response"></a><span data-ttu-id="955fb-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="955fb-194">Response</span></span>
<span data-ttu-id="955fb-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="955fb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 914

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "1ac6ea5a-ea5a-1ac6-5aea-c61a5aeac61a",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```



