---
title: Обновление Виндовсупдатестате
description: Обновление свойств объекта Виндовсупдатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 47021216905227509d2c97c38cbfa464764e79af
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939313"
---
# <a name="update-windowsupdatestate"></a><span data-ttu-id="44ea2-103">Обновление Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="44ea2-103">Update windowsUpdateState</span></span>

> <span data-ttu-id="44ea2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44ea2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44ea2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44ea2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44ea2-106">Обновление свойств объекта [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="44ea2-106">Update the properties of a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44ea2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="44ea2-107">Prerequisites</span></span>
<span data-ttu-id="44ea2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44ea2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44ea2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44ea2-110">Permission type</span></span>|<span data-ttu-id="44ea2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="44ea2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44ea2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44ea2-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="44ea2-113">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="44ea2-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="44ea2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44ea2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="44ea2-115">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="44ea2-115">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="44ea2-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44ea2-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44ea2-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44ea2-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44ea2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44ea2-118">Not supported.</span></span>|
|<span data-ttu-id="44ea2-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44ea2-119">Application</span></span>||
| <span data-ttu-id="44ea2-120">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="44ea2-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="44ea2-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44ea2-121">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="44ea2-122">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="44ea2-122">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="44ea2-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44ea2-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44ea2-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44ea2-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="44ea2-125">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="44ea2-125">Request headers</span></span>
|<span data-ttu-id="44ea2-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44ea2-126">Header</span></span>|<span data-ttu-id="44ea2-127">Значение</span><span class="sxs-lookup"><span data-stu-id="44ea2-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44ea2-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44ea2-128">Authorization</span></span>|<span data-ttu-id="44ea2-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44ea2-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44ea2-130">Accept</span><span class="sxs-lookup"><span data-stu-id="44ea2-130">Accept</span></span>|<span data-ttu-id="44ea2-131">application/json</span><span class="sxs-lookup"><span data-stu-id="44ea2-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44ea2-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="44ea2-132">Request body</span></span>
<span data-ttu-id="44ea2-133">В тексте запроса добавьте представление объекта [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44ea2-133">In the request body, supply a JSON representation for the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

<span data-ttu-id="44ea2-134">В следующей таблице приведены свойства, необходимые при создании [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="44ea2-134">The following table shows the properties that are required when you create the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

|<span data-ttu-id="44ea2-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="44ea2-135">Property</span></span>|<span data-ttu-id="44ea2-136">Тип</span><span class="sxs-lookup"><span data-stu-id="44ea2-136">Type</span></span>|<span data-ttu-id="44ea2-137">Описание</span><span class="sxs-lookup"><span data-stu-id="44ea2-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44ea2-138">id</span><span class="sxs-lookup"><span data-stu-id="44ea2-138">id</span></span>|<span data-ttu-id="44ea2-139">Строка</span><span class="sxs-lookup"><span data-stu-id="44ea2-139">String</span></span>|<span data-ttu-id="44ea2-140">Это идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="44ea2-140">This is Id of the entity.</span></span>|
|<span data-ttu-id="44ea2-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="44ea2-141">deviceId</span></span>|<span data-ttu-id="44ea2-142">Строка</span><span class="sxs-lookup"><span data-stu-id="44ea2-142">String</span></span>|<span data-ttu-id="44ea2-143">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="44ea2-143">The id of the device.</span></span>|
|<span data-ttu-id="44ea2-144">userId</span><span class="sxs-lookup"><span data-stu-id="44ea2-144">userId</span></span>|<span data-ttu-id="44ea2-145">String</span><span class="sxs-lookup"><span data-stu-id="44ea2-145">String</span></span>|<span data-ttu-id="44ea2-146">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="44ea2-146">The id of the user.</span></span>|
|<span data-ttu-id="44ea2-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="44ea2-147">deviceDisplayName</span></span>|<span data-ttu-id="44ea2-148">String</span><span class="sxs-lookup"><span data-stu-id="44ea2-148">String</span></span>|<span data-ttu-id="44ea2-149">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="44ea2-149">Device display name.</span></span>|
|<span data-ttu-id="44ea2-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="44ea2-150">userPrincipalName</span></span>|<span data-ttu-id="44ea2-151">Строка</span><span class="sxs-lookup"><span data-stu-id="44ea2-151">String</span></span>|<span data-ttu-id="44ea2-152">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="44ea2-152">User principal name.</span></span>|
|<span data-ttu-id="44ea2-153">status</span><span class="sxs-lookup"><span data-stu-id="44ea2-153">status</span></span>|[<span data-ttu-id="44ea2-154">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="44ea2-154">windowsUpdateStatus</span></span>](../resources/intune-shared-windowsupdatestatus.md)|<span data-ttu-id="44ea2-155">Состояние Windows удпате.</span><span class="sxs-lookup"><span data-stu-id="44ea2-155">Windows udpate status.</span></span> <span data-ttu-id="44ea2-156">Возможные значения: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="44ea2-156">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="44ea2-157">куалитюпдатеверсион</span><span class="sxs-lookup"><span data-stu-id="44ea2-157">qualityUpdateVersion</span></span>|<span data-ttu-id="44ea2-158">Строка</span><span class="sxs-lookup"><span data-stu-id="44ea2-158">String</span></span>|<span data-ttu-id="44ea2-159">Версия устройства для обновления качества.</span><span class="sxs-lookup"><span data-stu-id="44ea2-159">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="44ea2-160">феатуреупдатеверсион</span><span class="sxs-lookup"><span data-stu-id="44ea2-160">featureUpdateVersion</span></span>|<span data-ttu-id="44ea2-161">Строка</span><span class="sxs-lookup"><span data-stu-id="44ea2-161">String</span></span>|<span data-ttu-id="44ea2-162">Текущая версия обновления компонентов устройства.</span><span class="sxs-lookup"><span data-stu-id="44ea2-162">The current feature update version of the device.</span></span>|
|<span data-ttu-id="44ea2-163">ластскандатетиме</span><span class="sxs-lookup"><span data-stu-id="44ea2-163">lastScanDateTime</span></span>|<span data-ttu-id="44ea2-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44ea2-164">DateTimeOffset</span></span>|<span data-ttu-id="44ea2-165">Дата и время, когда агент обновления Windows успешно выполнил сканирование.</span><span class="sxs-lookup"><span data-stu-id="44ea2-165">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="44ea2-166">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="44ea2-166">lastSyncDateTime</span></span>|<span data-ttu-id="44ea2-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44ea2-167">DateTimeOffset</span></span>|<span data-ttu-id="44ea2-168">Дата и время последней синхронизации устройства с Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="44ea2-168">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="44ea2-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="44ea2-169">Response</span></span>
<span data-ttu-id="44ea2-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44ea2-170">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44ea2-171">Пример</span><span class="sxs-lookup"><span data-stu-id="44ea2-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="44ea2-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="44ea2-172">Request</span></span>
<span data-ttu-id="44ea2-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44ea2-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="44ea2-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="44ea2-174">Response</span></span>
<span data-ttu-id="44ea2-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44ea2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








