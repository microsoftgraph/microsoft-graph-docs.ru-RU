---
title: Создание Виндовсупдатестате
description: Создание нового объекта Виндовсупдатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4b6ad2081039a6bc6cf21259e2e6ffb4418637cd
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42159887"
---
# <a name="create-windowsupdatestate"></a><span data-ttu-id="c32de-103">Создание Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="c32de-103">Create windowsUpdateState</span></span>

> <span data-ttu-id="c32de-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c32de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c32de-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c32de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c32de-106">Создание нового объекта [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="c32de-106">Create a new [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c32de-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c32de-107">Prerequisites</span></span>
<span data-ttu-id="c32de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c32de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c32de-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c32de-110">Permission type</span></span>|<span data-ttu-id="c32de-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c32de-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c32de-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c32de-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c32de-113">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="c32de-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c32de-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c32de-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="c32de-115">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="c32de-115">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="c32de-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c32de-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c32de-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c32de-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c32de-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c32de-118">Not supported.</span></span>|
|<span data-ttu-id="c32de-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c32de-119">Application</span></span>||
| <span data-ttu-id="c32de-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="c32de-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c32de-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c32de-121">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="c32de-122">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="c32de-122">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="c32de-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c32de-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c32de-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c32de-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="c32de-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c32de-125">Request headers</span></span>
|<span data-ttu-id="c32de-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c32de-126">Header</span></span>|<span data-ttu-id="c32de-127">Значение</span><span class="sxs-lookup"><span data-stu-id="c32de-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c32de-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="c32de-128">Authorization</span></span>|<span data-ttu-id="c32de-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c32de-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c32de-130">Accept</span><span class="sxs-lookup"><span data-stu-id="c32de-130">Accept</span></span>|<span data-ttu-id="c32de-131">application/json</span><span class="sxs-lookup"><span data-stu-id="c32de-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c32de-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c32de-132">Request body</span></span>
<span data-ttu-id="c32de-133">В тексте запроса добавьте представление объекта Виндовсупдатестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c32de-133">In the request body, supply a JSON representation for the windowsUpdateState object.</span></span>

<span data-ttu-id="c32de-134">В следующей таблице приведены свойства, необходимые при создании Виндовсупдатестате.</span><span class="sxs-lookup"><span data-stu-id="c32de-134">The following table shows the properties that are required when you create the windowsUpdateState.</span></span>

|<span data-ttu-id="c32de-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="c32de-135">Property</span></span>|<span data-ttu-id="c32de-136">Тип</span><span class="sxs-lookup"><span data-stu-id="c32de-136">Type</span></span>|<span data-ttu-id="c32de-137">Описание</span><span class="sxs-lookup"><span data-stu-id="c32de-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c32de-138">id</span><span class="sxs-lookup"><span data-stu-id="c32de-138">id</span></span>|<span data-ttu-id="c32de-139">Строка</span><span class="sxs-lookup"><span data-stu-id="c32de-139">String</span></span>|<span data-ttu-id="c32de-140">Это идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="c32de-140">This is Id of the entity.</span></span>|
|<span data-ttu-id="c32de-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="c32de-141">deviceId</span></span>|<span data-ttu-id="c32de-142">String</span><span class="sxs-lookup"><span data-stu-id="c32de-142">String</span></span>|<span data-ttu-id="c32de-143">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="c32de-143">The id of the device.</span></span>|
|<span data-ttu-id="c32de-144">userId</span><span class="sxs-lookup"><span data-stu-id="c32de-144">userId</span></span>|<span data-ttu-id="c32de-145">String</span><span class="sxs-lookup"><span data-stu-id="c32de-145">String</span></span>|<span data-ttu-id="c32de-146">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="c32de-146">The id of the user.</span></span>|
|<span data-ttu-id="c32de-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="c32de-147">deviceDisplayName</span></span>|<span data-ttu-id="c32de-148">String</span><span class="sxs-lookup"><span data-stu-id="c32de-148">String</span></span>|<span data-ttu-id="c32de-149">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="c32de-149">Device display name.</span></span>|
|<span data-ttu-id="c32de-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c32de-150">userPrincipalName</span></span>|<span data-ttu-id="c32de-151">Строка</span><span class="sxs-lookup"><span data-stu-id="c32de-151">String</span></span>|<span data-ttu-id="c32de-152">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="c32de-152">User principal name.</span></span>|
|<span data-ttu-id="c32de-153">status</span><span class="sxs-lookup"><span data-stu-id="c32de-153">status</span></span>|[<span data-ttu-id="c32de-154">windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="c32de-154">windowsUpdateState</span></span>](../resources/intune-shared-windowsupdatestate.md)|<span data-ttu-id="c32de-155">Состояние Windows удпате.</span><span class="sxs-lookup"><span data-stu-id="c32de-155">Windows udpate status.</span></span> <span data-ttu-id="c32de-156">Возможные значения: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="c32de-156">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="c32de-157">куалитюпдатеверсион</span><span class="sxs-lookup"><span data-stu-id="c32de-157">qualityUpdateVersion</span></span>|<span data-ttu-id="c32de-158">String</span><span class="sxs-lookup"><span data-stu-id="c32de-158">String</span></span>|<span data-ttu-id="c32de-159">Версия устройства для обновления качества.</span><span class="sxs-lookup"><span data-stu-id="c32de-159">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="c32de-160">феатуреупдатеверсион</span><span class="sxs-lookup"><span data-stu-id="c32de-160">featureUpdateVersion</span></span>|<span data-ttu-id="c32de-161">String</span><span class="sxs-lookup"><span data-stu-id="c32de-161">String</span></span>|<span data-ttu-id="c32de-162">Текущая версия обновления компонентов устройства.</span><span class="sxs-lookup"><span data-stu-id="c32de-162">The current feature update version of the device.</span></span>|
|<span data-ttu-id="c32de-163">ластскандатетиме</span><span class="sxs-lookup"><span data-stu-id="c32de-163">lastScanDateTime</span></span>|<span data-ttu-id="c32de-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c32de-164">DateTimeOffset</span></span>|<span data-ttu-id="c32de-165">Дата и время, когда агент обновления Windows успешно выполнил сканирование.</span><span class="sxs-lookup"><span data-stu-id="c32de-165">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="c32de-166">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c32de-166">lastSyncDateTime</span></span>|<span data-ttu-id="c32de-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c32de-167">DateTimeOffset</span></span>|<span data-ttu-id="c32de-168">Дата и время последней синхронизации устройства с Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="c32de-168">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="c32de-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="c32de-169">Response</span></span>
<span data-ttu-id="c32de-170">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c32de-170">If successful, this method returns a `201 Created` response code and a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c32de-171">Пример</span><span class="sxs-lookup"><span data-stu-id="c32de-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="c32de-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="c32de-172">Request</span></span>
<span data-ttu-id="c32de-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c32de-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c32de-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="c32de-174">Response</span></span>
<span data-ttu-id="c32de-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c32de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








