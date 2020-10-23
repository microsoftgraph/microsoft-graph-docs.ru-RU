---
title: Создание Виндовсупдатестате
description: Создание нового объекта Виндовсупдатестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ccd1614bd128a0a3182194b64e14cc618da7022b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729870"
---
# <a name="create-windowsupdatestate"></a><span data-ttu-id="8fb03-103">Создание Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="8fb03-103">Create windowsUpdateState</span></span>

<span data-ttu-id="8fb03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fb03-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8fb03-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fb03-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fb03-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8fb03-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fb03-107">Создание нового объекта Виндовсупдатестате.</span><span class="sxs-lookup"><span data-stu-id="8fb03-107">Create a new windowsUpdateState object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8fb03-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8fb03-108">Prerequisites</span></span>
<span data-ttu-id="8fb03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fb03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fb03-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8fb03-111">Permission type</span></span>|<span data-ttu-id="8fb03-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8fb03-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fb03-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8fb03-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8fb03-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="8fb03-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8fb03-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fb03-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="8fb03-116">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="8fb03-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="8fb03-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fb03-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8fb03-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8fb03-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fb03-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fb03-119">Not supported.</span></span>|
|<span data-ttu-id="8fb03-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8fb03-120">Application</span></span>||
| <span data-ttu-id="8fb03-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="8fb03-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8fb03-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fb03-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="8fb03-123">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="8fb03-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="8fb03-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fb03-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fb03-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8fb03-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="8fb03-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8fb03-126">Request headers</span></span>
|<span data-ttu-id="8fb03-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8fb03-127">Header</span></span>|<span data-ttu-id="8fb03-128">Значение</span><span class="sxs-lookup"><span data-stu-id="8fb03-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fb03-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8fb03-129">Authorization</span></span>|<span data-ttu-id="8fb03-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8fb03-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fb03-131">Accept</span><span class="sxs-lookup"><span data-stu-id="8fb03-131">Accept</span></span>|<span data-ttu-id="8fb03-132">application/json</span><span class="sxs-lookup"><span data-stu-id="8fb03-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fb03-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8fb03-133">Request body</span></span>
<span data-ttu-id="8fb03-134">В тексте запроса добавьте представление объекта Виндовсупдатестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8fb03-134">In the request body, supply a JSON representation for the windowsUpdateState object.</span></span>

<span data-ttu-id="8fb03-135">В следующей таблице приведены свойства, необходимые при создании Виндовсупдатестате.</span><span class="sxs-lookup"><span data-stu-id="8fb03-135">The following table shows the properties that are required when you create the windowsUpdateState.</span></span>

|<span data-ttu-id="8fb03-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="8fb03-136">Property</span></span>|<span data-ttu-id="8fb03-137">Тип</span><span class="sxs-lookup"><span data-stu-id="8fb03-137">Type</span></span>|<span data-ttu-id="8fb03-138">Описание</span><span class="sxs-lookup"><span data-stu-id="8fb03-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fb03-139">id</span><span class="sxs-lookup"><span data-stu-id="8fb03-139">id</span></span>|<span data-ttu-id="8fb03-140">Строка</span><span class="sxs-lookup"><span data-stu-id="8fb03-140">String</span></span>|<span data-ttu-id="8fb03-141">Это идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="8fb03-141">This is Id of the entity.</span></span>|
|<span data-ttu-id="8fb03-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="8fb03-142">deviceId</span></span>|<span data-ttu-id="8fb03-143">String</span><span class="sxs-lookup"><span data-stu-id="8fb03-143">String</span></span>|<span data-ttu-id="8fb03-144">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="8fb03-144">The id of the device.</span></span>|
|<span data-ttu-id="8fb03-145">userId</span><span class="sxs-lookup"><span data-stu-id="8fb03-145">userId</span></span>|<span data-ttu-id="8fb03-146">String</span><span class="sxs-lookup"><span data-stu-id="8fb03-146">String</span></span>|<span data-ttu-id="8fb03-147">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="8fb03-147">The id of the user.</span></span>|
|<span data-ttu-id="8fb03-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8fb03-148">deviceDisplayName</span></span>|<span data-ttu-id="8fb03-149">String</span><span class="sxs-lookup"><span data-stu-id="8fb03-149">String</span></span>|<span data-ttu-id="8fb03-150">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="8fb03-150">Device display name.</span></span>|
|<span data-ttu-id="8fb03-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8fb03-151">userPrincipalName</span></span>|<span data-ttu-id="8fb03-152">String</span><span class="sxs-lookup"><span data-stu-id="8fb03-152">String</span></span>|<span data-ttu-id="8fb03-153">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="8fb03-153">User principal name.</span></span>|
|<span data-ttu-id="8fb03-154">status</span><span class="sxs-lookup"><span data-stu-id="8fb03-154">status</span></span>|[<span data-ttu-id="8fb03-155">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="8fb03-155">windowsUpdateStatus</span></span>](../resources/intune-deviceconfig-windowsupdatestatus.md)|<span data-ttu-id="8fb03-156">Состояние Windows удпате.</span><span class="sxs-lookup"><span data-stu-id="8fb03-156">Windows udpate status.</span></span> <span data-ttu-id="8fb03-157">Возможные значения: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="8fb03-157">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="8fb03-158">куалитюпдатеверсион</span><span class="sxs-lookup"><span data-stu-id="8fb03-158">qualityUpdateVersion</span></span>|<span data-ttu-id="8fb03-159">Строка</span><span class="sxs-lookup"><span data-stu-id="8fb03-159">String</span></span>|<span data-ttu-id="8fb03-160">Версия устройства для обновления качества.</span><span class="sxs-lookup"><span data-stu-id="8fb03-160">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="8fb03-161">феатуреупдатеверсион</span><span class="sxs-lookup"><span data-stu-id="8fb03-161">featureUpdateVersion</span></span>|<span data-ttu-id="8fb03-162">Строка</span><span class="sxs-lookup"><span data-stu-id="8fb03-162">String</span></span>|<span data-ttu-id="8fb03-163">Текущая версия обновления компонентов устройства.</span><span class="sxs-lookup"><span data-stu-id="8fb03-163">The current feature update version of the device.</span></span>|
|<span data-ttu-id="8fb03-164">ластскандатетиме</span><span class="sxs-lookup"><span data-stu-id="8fb03-164">lastScanDateTime</span></span>|<span data-ttu-id="8fb03-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fb03-165">DateTimeOffset</span></span>|<span data-ttu-id="8fb03-166">Дата и время, когда агент обновления Windows успешно выполнил сканирование.</span><span class="sxs-lookup"><span data-stu-id="8fb03-166">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="8fb03-167">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8fb03-167">lastSyncDateTime</span></span>|<span data-ttu-id="8fb03-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fb03-168">DateTimeOffset</span></span>|<span data-ttu-id="8fb03-169">Дата и время последней синхронизации устройства с Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="8fb03-169">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="8fb03-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="8fb03-170">Response</span></span>
<span data-ttu-id="8fb03-171">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8fb03-171">If successful, this method returns a `201 Created` response code and a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fb03-172">Пример</span><span class="sxs-lookup"><span data-stu-id="8fb03-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="8fb03-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="8fb03-173">Request</span></span>
<span data-ttu-id="8fb03-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8fb03-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
Content-type: application/json
Content-length: 504

{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "status": "pendingInstallation",
  "qualityUpdateVersion": "Quality Update Version value",
  "featureUpdateVersion": "Feature Update Version value",
  "lastScanDateTime": "2016-12-31T23:59:18.0955018-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```

### <a name="response"></a><span data-ttu-id="8fb03-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fb03-175">Response</span></span>
<span data-ttu-id="8fb03-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8fb03-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 553

{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "id": "3d92af00-af00-3d92-00af-923d00af923d",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "status": "pendingInstallation",
  "qualityUpdateVersion": "Quality Update Version value",
  "featureUpdateVersion": "Feature Update Version value",
  "lastScanDateTime": "2016-12-31T23:59:18.0955018-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```








