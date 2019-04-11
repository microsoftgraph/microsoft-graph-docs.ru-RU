---
title: Обновление windowsProtectionState
description: Обновление свойств объекта windowsProtectionState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b53e93f09be2b091ffe3e6a30cd109feb55c8d8a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797405"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="5a1c6-103">Обновление windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="5a1c6-103">Update windowsProtectionState</span></span>

> <span data-ttu-id="5a1c6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a1c6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a1c6-106">Обновление свойств объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="5a1c6-106">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a1c6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5a1c6-107">Prerequisites</span></span>
<span data-ttu-id="5a1c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a1c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a1c6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a1c6-110">Permission type</span></span>|<span data-ttu-id="5a1c6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a1c6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a1c6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a1c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5a1c6-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a1c6-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5a1c6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a1c6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a1c6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-115">Not supported.</span></span>|
|<span data-ttu-id="5a1c6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a1c6-116">Application</span></span>|<span data-ttu-id="5a1c6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a1c6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a1c6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="5a1c6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a1c6-119">Request headers</span></span>
|<span data-ttu-id="5a1c6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a1c6-120">Header</span></span>|<span data-ttu-id="5a1c6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5a1c6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a1c6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a1c6-122">Authorization</span></span>|<span data-ttu-id="5a1c6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a1c6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5a1c6-124">Accept</span></span>|<span data-ttu-id="5a1c6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5a1c6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a1c6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a1c6-126">Request body</span></span>
<span data-ttu-id="5a1c6-127">В тексте запроса добавьте представление объекта [WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-127">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="5a1c6-128">В следующей таблице приведены свойства, необходимые при создании [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span><span class="sxs-lookup"><span data-stu-id="5a1c6-128">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="5a1c6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a1c6-129">Property</span></span>|<span data-ttu-id="5a1c6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5a1c6-130">Type</span></span>|<span data-ttu-id="5a1c6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5a1c6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a1c6-132">id</span><span class="sxs-lookup"><span data-stu-id="5a1c6-132">id</span></span>|<span data-ttu-id="5a1c6-133">String</span><span class="sxs-lookup"><span data-stu-id="5a1c6-133">String</span></span>|<span data-ttu-id="5a1c6-134">Уникальный идентификатор для объекта состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-134">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="5a1c6-135">Это идентификатор устройства для устройства.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-135">This is device id of the device</span></span>|
|<span data-ttu-id="5a1c6-136">Малварепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="5a1c6-136">malwareProtectionEnabled</span></span>|<span data-ttu-id="5a1c6-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a1c6-137">Boolean</span></span>|<span data-ttu-id="5a1c6-138">Защита от вредоносных программ включена или нет</span><span class="sxs-lookup"><span data-stu-id="5a1c6-138">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="5a1c6-139">Девицестате</span><span class="sxs-lookup"><span data-stu-id="5a1c6-139">deviceState</span></span>|[<span data-ttu-id="5a1c6-140">Виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="5a1c6-140">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="5a1c6-141">Состояние компьютера (например, очистка или ожидание полного сканирования или Ожидание перезагрузки и т. д.).</span><span class="sxs-lookup"><span data-stu-id="5a1c6-141">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="5a1c6-142">Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-142">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="5a1c6-143">Реалтимепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="5a1c6-143">realTimeProtectionEnabled</span></span>|<span data-ttu-id="5a1c6-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a1c6-144">Boolean</span></span>|<span data-ttu-id="5a1c6-145">Защита в режиме реального времени включена или нет?</span><span class="sxs-lookup"><span data-stu-id="5a1c6-145">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="5a1c6-146">Нетворкинспектионсистеменаблед</span><span class="sxs-lookup"><span data-stu-id="5a1c6-146">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="5a1c6-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a1c6-147">Boolean</span></span>|<span data-ttu-id="5a1c6-148">Система проверки сети включена или нет?</span><span class="sxs-lookup"><span data-stu-id="5a1c6-148">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="5a1c6-149">Куиккскановердуе</span><span class="sxs-lookup"><span data-stu-id="5a1c6-149">quickScanOverdue</span></span>|<span data-ttu-id="5a1c6-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a1c6-150">Boolean</span></span>|<span data-ttu-id="5a1c6-151">Быстрая проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="5a1c6-151">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="5a1c6-152">Фуллскановердуе</span><span class="sxs-lookup"><span data-stu-id="5a1c6-152">fullScanOverdue</span></span>|<span data-ttu-id="5a1c6-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a1c6-153">Boolean</span></span>|<span data-ttu-id="5a1c6-154">Полная проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="5a1c6-154">Full scan overdue or not?</span></span>|
|<span data-ttu-id="5a1c6-155">Сигнатуреупдатеовердуе</span><span class="sxs-lookup"><span data-stu-id="5a1c6-155">signatureUpdateOverdue</span></span>|<span data-ttu-id="5a1c6-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a1c6-156">Boolean</span></span>|<span data-ttu-id="5a1c6-157">Подпись устарела или нет?</span><span class="sxs-lookup"><span data-stu-id="5a1c6-157">Signature out of date or not?</span></span>|
|<span data-ttu-id="5a1c6-158">Ребутрекуиред</span><span class="sxs-lookup"><span data-stu-id="5a1c6-158">rebootRequired</span></span>|<span data-ttu-id="5a1c6-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a1c6-159">Boolean</span></span>|<span data-ttu-id="5a1c6-160">Требуется переЗагрузка или нет?</span><span class="sxs-lookup"><span data-stu-id="5a1c6-160">Reboot required or not?</span></span>|
|<span data-ttu-id="5a1c6-161">Фуллсканрекуиред</span><span class="sxs-lookup"><span data-stu-id="5a1c6-161">fullScanRequired</span></span>|<span data-ttu-id="5a1c6-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a1c6-162">Boolean</span></span>|<span data-ttu-id="5a1c6-163">Необходима полная проверка или нет?</span><span class="sxs-lookup"><span data-stu-id="5a1c6-163">Full scan required or not?</span></span>|
|<span data-ttu-id="5a1c6-164">Енгиневерсион</span><span class="sxs-lookup"><span data-stu-id="5a1c6-164">engineVersion</span></span>|<span data-ttu-id="5a1c6-165">String</span><span class="sxs-lookup"><span data-stu-id="5a1c6-165">String</span></span>|<span data-ttu-id="5a1c6-166">Текущая версия модуля Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="5a1c6-166">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="5a1c6-167">Сигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="5a1c6-167">signatureVersion</span></span>|<span data-ttu-id="5a1c6-168">String</span><span class="sxs-lookup"><span data-stu-id="5a1c6-168">String</span></span>|<span data-ttu-id="5a1c6-169">Текущая версия определений вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="5a1c6-169">Current malware definitions version</span></span>|
|<span data-ttu-id="5a1c6-170">Антималвареверсион</span><span class="sxs-lookup"><span data-stu-id="5a1c6-170">antiMalwareVersion</span></span>|<span data-ttu-id="5a1c6-171">String</span><span class="sxs-lookup"><span data-stu-id="5a1c6-171">String</span></span>|<span data-ttu-id="5a1c6-172">Текущая версия защиты от вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="5a1c6-172">Current anti malware version</span></span>|
|<span data-ttu-id="5a1c6-173">Ласткуиккскандатетиме</span><span class="sxs-lookup"><span data-stu-id="5a1c6-173">lastQuickScanDateTime</span></span>|<span data-ttu-id="5a1c6-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a1c6-174">DateTimeOffset</span></span>|<span data-ttu-id="5a1c6-175">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="5a1c6-175">Last quick scan datetime</span></span>|
|<span data-ttu-id="5a1c6-176">Ластфуллскандатетиме</span><span class="sxs-lookup"><span data-stu-id="5a1c6-176">lastFullScanDateTime</span></span>|<span data-ttu-id="5a1c6-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a1c6-177">DateTimeOffset</span></span>|<span data-ttu-id="5a1c6-178">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="5a1c6-178">Last quick scan datetime</span></span>|
|<span data-ttu-id="5a1c6-179">Ласткуиккскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="5a1c6-179">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="5a1c6-180">String</span><span class="sxs-lookup"><span data-stu-id="5a1c6-180">String</span></span>|<span data-ttu-id="5a1c6-181">Последняя версия подписи быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="5a1c6-181">Last quick scan signature version</span></span>|
|<span data-ttu-id="5a1c6-182">Ластфуллскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="5a1c6-182">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="5a1c6-183">String</span><span class="sxs-lookup"><span data-stu-id="5a1c6-183">String</span></span>|<span data-ttu-id="5a1c6-184">Версия последней полной проверки подписи</span><span class="sxs-lookup"><span data-stu-id="5a1c6-184">Last full scan signature version</span></span>|
|<span data-ttu-id="5a1c6-185">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a1c6-185">lastReportedDateTime</span></span>|<span data-ttu-id="5a1c6-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a1c6-186">DateTimeOffset</span></span>|<span data-ttu-id="5a1c6-187">Последнее состояние работоспособности устройства в отчете о времени</span><span class="sxs-lookup"><span data-stu-id="5a1c6-187">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="5a1c6-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a1c6-188">Response</span></span>
<span data-ttu-id="5a1c6-189">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-189">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a1c6-190">Пример</span><span class="sxs-lookup"><span data-stu-id="5a1c6-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a1c6-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a1c6-191">Request</span></span>
<span data-ttu-id="5a1c6-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5a1c6-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a1c6-193">Response</span></span>
<span data-ttu-id="5a1c6-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a1c6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





