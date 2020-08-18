---
title: Обновление windowsProtectionState
description: Обновление свойств объекта windowsProtectionState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 593ba645ef109742c295c3f45bb2c2e4d3af3be6
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790555"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="85b18-103">Обновление windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="85b18-103">Update windowsProtectionState</span></span>

<span data-ttu-id="85b18-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85b18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85b18-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85b18-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85b18-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85b18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85b18-107">Обновление свойств объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="85b18-107">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85b18-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="85b18-108">Prerequisites</span></span>
<span data-ttu-id="85b18-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85b18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85b18-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85b18-111">Permission type</span></span>|<span data-ttu-id="85b18-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85b18-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85b18-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85b18-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85b18-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85b18-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="85b18-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85b18-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85b18-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85b18-116">Not supported.</span></span>|
|<span data-ttu-id="85b18-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="85b18-117">Application</span></span>|<span data-ttu-id="85b18-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85b18-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85b18-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85b18-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="85b18-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="85b18-120">Request headers</span></span>
|<span data-ttu-id="85b18-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85b18-121">Header</span></span>|<span data-ttu-id="85b18-122">Значение</span><span class="sxs-lookup"><span data-stu-id="85b18-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85b18-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85b18-123">Authorization</span></span>|<span data-ttu-id="85b18-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85b18-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85b18-125">Accept</span><span class="sxs-lookup"><span data-stu-id="85b18-125">Accept</span></span>|<span data-ttu-id="85b18-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85b18-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85b18-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85b18-127">Request body</span></span>
<span data-ttu-id="85b18-128">В тексте запроса добавьте представление объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85b18-128">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="85b18-129">В следующей таблице приведены свойства, необходимые при создании [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span><span class="sxs-lookup"><span data-stu-id="85b18-129">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="85b18-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="85b18-130">Property</span></span>|<span data-ttu-id="85b18-131">Тип</span><span class="sxs-lookup"><span data-stu-id="85b18-131">Type</span></span>|<span data-ttu-id="85b18-132">Описание</span><span class="sxs-lookup"><span data-stu-id="85b18-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85b18-133">id</span><span class="sxs-lookup"><span data-stu-id="85b18-133">id</span></span>|<span data-ttu-id="85b18-134">String</span><span class="sxs-lookup"><span data-stu-id="85b18-134">String</span></span>|<span data-ttu-id="85b18-135">Уникальный идентификатор для объекта состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="85b18-135">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="85b18-136">Это идентификатор устройства для устройства.</span><span class="sxs-lookup"><span data-stu-id="85b18-136">This is device id of the device</span></span>|
|<span data-ttu-id="85b18-137">малварепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="85b18-137">malwareProtectionEnabled</span></span>|<span data-ttu-id="85b18-138">Логический</span><span class="sxs-lookup"><span data-stu-id="85b18-138">Boolean</span></span>|<span data-ttu-id="85b18-139">Защита от вредоносных программ включена или нет</span><span class="sxs-lookup"><span data-stu-id="85b18-139">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="85b18-140">девицестате</span><span class="sxs-lookup"><span data-stu-id="85b18-140">deviceState</span></span>|[<span data-ttu-id="85b18-141">виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="85b18-141">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="85b18-142">Состояние компьютера (например, очистка или ожидание полного сканирования или Ожидание перезагрузки и т. д.).</span><span class="sxs-lookup"><span data-stu-id="85b18-142">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="85b18-143">Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="85b18-143">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="85b18-144">реалтимепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="85b18-144">realTimeProtectionEnabled</span></span>|<span data-ttu-id="85b18-145">Логический</span><span class="sxs-lookup"><span data-stu-id="85b18-145">Boolean</span></span>|<span data-ttu-id="85b18-146">Защита в режиме реального времени включена или нет?</span><span class="sxs-lookup"><span data-stu-id="85b18-146">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="85b18-147">нетворкинспектионсистеменаблед</span><span class="sxs-lookup"><span data-stu-id="85b18-147">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="85b18-148">Логический</span><span class="sxs-lookup"><span data-stu-id="85b18-148">Boolean</span></span>|<span data-ttu-id="85b18-149">Система проверки сети включена или нет?</span><span class="sxs-lookup"><span data-stu-id="85b18-149">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="85b18-150">куиккскановердуе</span><span class="sxs-lookup"><span data-stu-id="85b18-150">quickScanOverdue</span></span>|<span data-ttu-id="85b18-151">Логический</span><span class="sxs-lookup"><span data-stu-id="85b18-151">Boolean</span></span>|<span data-ttu-id="85b18-152">Быстрая проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="85b18-152">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="85b18-153">фуллскановердуе</span><span class="sxs-lookup"><span data-stu-id="85b18-153">fullScanOverdue</span></span>|<span data-ttu-id="85b18-154">Логический</span><span class="sxs-lookup"><span data-stu-id="85b18-154">Boolean</span></span>|<span data-ttu-id="85b18-155">Полная проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="85b18-155">Full scan overdue or not?</span></span>|
|<span data-ttu-id="85b18-156">сигнатуреупдатеовердуе</span><span class="sxs-lookup"><span data-stu-id="85b18-156">signatureUpdateOverdue</span></span>|<span data-ttu-id="85b18-157">Логический</span><span class="sxs-lookup"><span data-stu-id="85b18-157">Boolean</span></span>|<span data-ttu-id="85b18-158">Подпись устарела или нет?</span><span class="sxs-lookup"><span data-stu-id="85b18-158">Signature out of date or not?</span></span>|
|<span data-ttu-id="85b18-159">ребутрекуиред</span><span class="sxs-lookup"><span data-stu-id="85b18-159">rebootRequired</span></span>|<span data-ttu-id="85b18-160">Логический</span><span class="sxs-lookup"><span data-stu-id="85b18-160">Boolean</span></span>|<span data-ttu-id="85b18-161">Требуется перезагрузка или нет?</span><span class="sxs-lookup"><span data-stu-id="85b18-161">Reboot required or not?</span></span>|
|<span data-ttu-id="85b18-162">фуллсканрекуиред</span><span class="sxs-lookup"><span data-stu-id="85b18-162">fullScanRequired</span></span>|<span data-ttu-id="85b18-163">Логический</span><span class="sxs-lookup"><span data-stu-id="85b18-163">Boolean</span></span>|<span data-ttu-id="85b18-164">Необходима полная проверка или нет?</span><span class="sxs-lookup"><span data-stu-id="85b18-164">Full scan required or not?</span></span>|
|<span data-ttu-id="85b18-165">енгиневерсион</span><span class="sxs-lookup"><span data-stu-id="85b18-165">engineVersion</span></span>|<span data-ttu-id="85b18-166">String</span><span class="sxs-lookup"><span data-stu-id="85b18-166">String</span></span>|<span data-ttu-id="85b18-167">Текущая версия модуля Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="85b18-167">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="85b18-168">сигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="85b18-168">signatureVersion</span></span>|<span data-ttu-id="85b18-169">String</span><span class="sxs-lookup"><span data-stu-id="85b18-169">String</span></span>|<span data-ttu-id="85b18-170">Текущая версия определений вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="85b18-170">Current malware definitions version</span></span>|
|<span data-ttu-id="85b18-171">антималвареверсион</span><span class="sxs-lookup"><span data-stu-id="85b18-171">antiMalwareVersion</span></span>|<span data-ttu-id="85b18-172">String</span><span class="sxs-lookup"><span data-stu-id="85b18-172">String</span></span>|<span data-ttu-id="85b18-173">Текущая версия защиты от вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="85b18-173">Current anti malware version</span></span>|
|<span data-ttu-id="85b18-174">ласткуиккскандатетиме</span><span class="sxs-lookup"><span data-stu-id="85b18-174">lastQuickScanDateTime</span></span>|<span data-ttu-id="85b18-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85b18-175">DateTimeOffset</span></span>|<span data-ttu-id="85b18-176">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="85b18-176">Last quick scan datetime</span></span>|
|<span data-ttu-id="85b18-177">ластфуллскандатетиме</span><span class="sxs-lookup"><span data-stu-id="85b18-177">lastFullScanDateTime</span></span>|<span data-ttu-id="85b18-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85b18-178">DateTimeOffset</span></span>|<span data-ttu-id="85b18-179">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="85b18-179">Last quick scan datetime</span></span>|
|<span data-ttu-id="85b18-180">ласткуиккскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="85b18-180">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="85b18-181">String</span><span class="sxs-lookup"><span data-stu-id="85b18-181">String</span></span>|<span data-ttu-id="85b18-182">Последняя версия подписи быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="85b18-182">Last quick scan signature version</span></span>|
|<span data-ttu-id="85b18-183">ластфуллскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="85b18-183">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="85b18-184">String</span><span class="sxs-lookup"><span data-stu-id="85b18-184">String</span></span>|<span data-ttu-id="85b18-185">Версия последней полной проверки подписи</span><span class="sxs-lookup"><span data-stu-id="85b18-185">Last full scan signature version</span></span>|
|<span data-ttu-id="85b18-186">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="85b18-186">lastReportedDateTime</span></span>|<span data-ttu-id="85b18-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85b18-187">DateTimeOffset</span></span>|<span data-ttu-id="85b18-188">Последнее состояние работоспособности устройства в отчете о времени</span><span class="sxs-lookup"><span data-stu-id="85b18-188">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="85b18-189">Ответ</span><span class="sxs-lookup"><span data-stu-id="85b18-189">Response</span></span>
<span data-ttu-id="85b18-190">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85b18-190">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85b18-191">Пример</span><span class="sxs-lookup"><span data-stu-id="85b18-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="85b18-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="85b18-192">Request</span></span>
<span data-ttu-id="85b18-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85b18-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
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

### <a name="response"></a><span data-ttu-id="85b18-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="85b18-194">Response</span></span>
<span data-ttu-id="85b18-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85b18-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



