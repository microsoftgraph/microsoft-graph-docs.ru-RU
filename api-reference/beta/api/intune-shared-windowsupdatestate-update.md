---
title: Обновление Виндовсупдатестате
description: Обновление свойств объекта Виндовсупдатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4778c4a45b473e7eea8176e05dfbe5525cc04aee
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085411"
---
# <a name="update-windowsupdatestate"></a><span data-ttu-id="7a19e-103">Обновление Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="7a19e-103">Update windowsUpdateState</span></span>

> <span data-ttu-id="7a19e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a19e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a19e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a19e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a19e-106">Обновление свойств объекта [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="7a19e-106">Update the properties of a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a19e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7a19e-107">Prerequisites</span></span>
<span data-ttu-id="7a19e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a19e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a19e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a19e-110">Permission type</span></span>|<span data-ttu-id="7a19e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a19e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a19e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a19e-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7a19e-113">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="7a19e-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="7a19e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a19e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="7a19e-115">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="7a19e-115">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="7a19e-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a19e-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7a19e-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a19e-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a19e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a19e-118">Not supported.</span></span>|
|<span data-ttu-id="7a19e-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a19e-119">Application</span></span>||
| <span data-ttu-id="7a19e-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="7a19e-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="7a19e-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a19e-121">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="7a19e-122">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="7a19e-122">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="7a19e-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a19e-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a19e-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a19e-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="7a19e-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7a19e-125">Request headers</span></span>
|<span data-ttu-id="7a19e-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a19e-126">Header</span></span>|<span data-ttu-id="7a19e-127">Значение</span><span class="sxs-lookup"><span data-stu-id="7a19e-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a19e-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7a19e-128">Authorization</span></span>|<span data-ttu-id="7a19e-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a19e-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a19e-130">Accept</span><span class="sxs-lookup"><span data-stu-id="7a19e-130">Accept</span></span>|<span data-ttu-id="7a19e-131">application/json</span><span class="sxs-lookup"><span data-stu-id="7a19e-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a19e-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a19e-132">Request body</span></span>
<span data-ttu-id="7a19e-133">В тексте запроса добавьте представление объекта [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a19e-133">In the request body, supply a JSON representation for the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

<span data-ttu-id="7a19e-134">В следующей таблице приведены свойства, необходимые при создании [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="7a19e-134">The following table shows the properties that are required when you create the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

|<span data-ttu-id="7a19e-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a19e-135">Property</span></span>|<span data-ttu-id="7a19e-136">Тип</span><span class="sxs-lookup"><span data-stu-id="7a19e-136">Type</span></span>|<span data-ttu-id="7a19e-137">Описание</span><span class="sxs-lookup"><span data-stu-id="7a19e-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a19e-138">id</span><span class="sxs-lookup"><span data-stu-id="7a19e-138">id</span></span>|<span data-ttu-id="7a19e-139">Строка</span><span class="sxs-lookup"><span data-stu-id="7a19e-139">String</span></span>|<span data-ttu-id="7a19e-140">Это идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="7a19e-140">This is Id of the entity.</span></span>|
|<span data-ttu-id="7a19e-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="7a19e-141">deviceId</span></span>|<span data-ttu-id="7a19e-142">String</span><span class="sxs-lookup"><span data-stu-id="7a19e-142">String</span></span>|<span data-ttu-id="7a19e-143">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="7a19e-143">The id of the device.</span></span>|
|<span data-ttu-id="7a19e-144">userId</span><span class="sxs-lookup"><span data-stu-id="7a19e-144">userId</span></span>|<span data-ttu-id="7a19e-145">String</span><span class="sxs-lookup"><span data-stu-id="7a19e-145">String</span></span>|<span data-ttu-id="7a19e-146">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="7a19e-146">The id of the user.</span></span>|
|<span data-ttu-id="7a19e-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="7a19e-147">deviceDisplayName</span></span>|<span data-ttu-id="7a19e-148">String</span><span class="sxs-lookup"><span data-stu-id="7a19e-148">String</span></span>|<span data-ttu-id="7a19e-149">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="7a19e-149">Device display name.</span></span>|
|<span data-ttu-id="7a19e-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7a19e-150">userPrincipalName</span></span>|<span data-ttu-id="7a19e-151">Строка</span><span class="sxs-lookup"><span data-stu-id="7a19e-151">String</span></span>|<span data-ttu-id="7a19e-152">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="7a19e-152">User principal name.</span></span>|
|<span data-ttu-id="7a19e-153">status</span><span class="sxs-lookup"><span data-stu-id="7a19e-153">status</span></span>|[<span data-ttu-id="7a19e-154">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="7a19e-154">windowsUpdateStatus</span></span>](../resources/intune-shared-windowsupdatestatus.md)|<span data-ttu-id="7a19e-155">Состояние Windows удпате.</span><span class="sxs-lookup"><span data-stu-id="7a19e-155">Windows udpate status.</span></span> <span data-ttu-id="7a19e-156">Возможные значения: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="7a19e-156">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="7a19e-157">куалитюпдатеверсион</span><span class="sxs-lookup"><span data-stu-id="7a19e-157">qualityUpdateVersion</span></span>|<span data-ttu-id="7a19e-158">String</span><span class="sxs-lookup"><span data-stu-id="7a19e-158">String</span></span>|<span data-ttu-id="7a19e-159">Версия устройства для обновления качества.</span><span class="sxs-lookup"><span data-stu-id="7a19e-159">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="7a19e-160">феатуреупдатеверсион</span><span class="sxs-lookup"><span data-stu-id="7a19e-160">featureUpdateVersion</span></span>|<span data-ttu-id="7a19e-161">String</span><span class="sxs-lookup"><span data-stu-id="7a19e-161">String</span></span>|<span data-ttu-id="7a19e-162">Текущая версия обновления компонентов устройства.</span><span class="sxs-lookup"><span data-stu-id="7a19e-162">The current feature update version of the device.</span></span>|
|<span data-ttu-id="7a19e-163">ластскандатетиме</span><span class="sxs-lookup"><span data-stu-id="7a19e-163">lastScanDateTime</span></span>|<span data-ttu-id="7a19e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a19e-164">DateTimeOffset</span></span>|<span data-ttu-id="7a19e-165">Дата и время, когда агент обновления Windows успешно выполнил сканирование.</span><span class="sxs-lookup"><span data-stu-id="7a19e-165">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="7a19e-166">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7a19e-166">lastSyncDateTime</span></span>|<span data-ttu-id="7a19e-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a19e-167">DateTimeOffset</span></span>|<span data-ttu-id="7a19e-168">Дата и время последней синхронизации устройства с Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="7a19e-168">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="7a19e-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a19e-169">Response</span></span>
<span data-ttu-id="7a19e-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7a19e-170">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a19e-171">Пример</span><span class="sxs-lookup"><span data-stu-id="7a19e-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a19e-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a19e-172">Request</span></span>
<span data-ttu-id="7a19e-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a19e-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
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

### <a name="response"></a><span data-ttu-id="7a19e-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a19e-174">Response</span></span>
<span data-ttu-id="7a19e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7a19e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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









