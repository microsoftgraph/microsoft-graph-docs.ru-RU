---
title: Создание Виндовсупдатестате
description: Создание нового объекта Виндовсупдатестате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 72171242c826ac171641658067c10d6fa607ad43
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123794"
---
# <a name="create-windowsupdatestate"></a><span data-ttu-id="468e6-103">Создание Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="468e6-103">Create windowsUpdateState</span></span>

<span data-ttu-id="468e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="468e6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="468e6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="468e6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="468e6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="468e6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="468e6-107">Создание нового объекта [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="468e6-107">Create a new [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="468e6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="468e6-108">Prerequisites</span></span>
<span data-ttu-id="468e6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="468e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="468e6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="468e6-111">Permission type</span></span>|<span data-ttu-id="468e6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="468e6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="468e6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="468e6-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="468e6-114">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="468e6-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="468e6-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="468e6-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="468e6-116">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="468e6-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="468e6-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="468e6-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="468e6-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="468e6-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="468e6-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="468e6-119">Not supported.</span></span>|
|<span data-ttu-id="468e6-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="468e6-120">Application</span></span>||
| <span data-ttu-id="468e6-121">&nbsp; &nbsp; **Конфигурация устройства**</span><span class="sxs-lookup"><span data-stu-id="468e6-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="468e6-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="468e6-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="468e6-123">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="468e6-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="468e6-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="468e6-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="468e6-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="468e6-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="468e6-126">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="468e6-126">Request headers</span></span>
|<span data-ttu-id="468e6-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="468e6-127">Header</span></span>|<span data-ttu-id="468e6-128">Значение</span><span class="sxs-lookup"><span data-stu-id="468e6-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="468e6-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="468e6-129">Authorization</span></span>|<span data-ttu-id="468e6-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="468e6-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="468e6-131">Accept</span><span class="sxs-lookup"><span data-stu-id="468e6-131">Accept</span></span>|<span data-ttu-id="468e6-132">application/json</span><span class="sxs-lookup"><span data-stu-id="468e6-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="468e6-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="468e6-133">Request body</span></span>
<span data-ttu-id="468e6-134">В тексте запроса добавьте представление объекта Виндовсупдатестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="468e6-134">In the request body, supply a JSON representation for the windowsUpdateState object.</span></span>

<span data-ttu-id="468e6-135">В следующей таблице приведены свойства, необходимые при создании Виндовсупдатестате.</span><span class="sxs-lookup"><span data-stu-id="468e6-135">The following table shows the properties that are required when you create the windowsUpdateState.</span></span>

|<span data-ttu-id="468e6-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="468e6-136">Property</span></span>|<span data-ttu-id="468e6-137">Тип</span><span class="sxs-lookup"><span data-stu-id="468e6-137">Type</span></span>|<span data-ttu-id="468e6-138">Описание</span><span class="sxs-lookup"><span data-stu-id="468e6-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="468e6-139">id</span><span class="sxs-lookup"><span data-stu-id="468e6-139">id</span></span>|<span data-ttu-id="468e6-140">Строка</span><span class="sxs-lookup"><span data-stu-id="468e6-140">String</span></span>|<span data-ttu-id="468e6-141">Это идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="468e6-141">This is Id of the entity.</span></span>|
|<span data-ttu-id="468e6-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="468e6-142">deviceId</span></span>|<span data-ttu-id="468e6-143">String</span><span class="sxs-lookup"><span data-stu-id="468e6-143">String</span></span>|<span data-ttu-id="468e6-144">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="468e6-144">The id of the device.</span></span>|
|<span data-ttu-id="468e6-145">userId</span><span class="sxs-lookup"><span data-stu-id="468e6-145">userId</span></span>|<span data-ttu-id="468e6-146">String</span><span class="sxs-lookup"><span data-stu-id="468e6-146">String</span></span>|<span data-ttu-id="468e6-147">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="468e6-147">The id of the user.</span></span>|
|<span data-ttu-id="468e6-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="468e6-148">deviceDisplayName</span></span>|<span data-ttu-id="468e6-149">String</span><span class="sxs-lookup"><span data-stu-id="468e6-149">String</span></span>|<span data-ttu-id="468e6-150">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="468e6-150">Device display name.</span></span>|
|<span data-ttu-id="468e6-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="468e6-151">userPrincipalName</span></span>|<span data-ttu-id="468e6-152">Строка</span><span class="sxs-lookup"><span data-stu-id="468e6-152">String</span></span>|<span data-ttu-id="468e6-153">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="468e6-153">User principal name.</span></span>|
|<span data-ttu-id="468e6-154">status</span><span class="sxs-lookup"><span data-stu-id="468e6-154">status</span></span>|[<span data-ttu-id="468e6-155">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="468e6-155">windowsUpdateStatus</span></span>](../resources/intune-shared-windowsupdatestatus.md)|<span data-ttu-id="468e6-156">Состояние Windows удпате.</span><span class="sxs-lookup"><span data-stu-id="468e6-156">Windows udpate status.</span></span> <span data-ttu-id="468e6-157">Возможные значения: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="468e6-157">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="468e6-158">куалитюпдатеверсион</span><span class="sxs-lookup"><span data-stu-id="468e6-158">qualityUpdateVersion</span></span>|<span data-ttu-id="468e6-159">String</span><span class="sxs-lookup"><span data-stu-id="468e6-159">String</span></span>|<span data-ttu-id="468e6-160">Версия устройства для обновления качества.</span><span class="sxs-lookup"><span data-stu-id="468e6-160">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="468e6-161">феатуреупдатеверсион</span><span class="sxs-lookup"><span data-stu-id="468e6-161">featureUpdateVersion</span></span>|<span data-ttu-id="468e6-162">String</span><span class="sxs-lookup"><span data-stu-id="468e6-162">String</span></span>|<span data-ttu-id="468e6-163">Текущая версия обновления компонентов устройства.</span><span class="sxs-lookup"><span data-stu-id="468e6-163">The current feature update version of the device.</span></span>|
|<span data-ttu-id="468e6-164">ластскандатетиме</span><span class="sxs-lookup"><span data-stu-id="468e6-164">lastScanDateTime</span></span>|<span data-ttu-id="468e6-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="468e6-165">DateTimeOffset</span></span>|<span data-ttu-id="468e6-166">Дата и время, когда агент обновления Windows успешно выполнил сканирование.</span><span class="sxs-lookup"><span data-stu-id="468e6-166">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="468e6-167">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="468e6-167">lastSyncDateTime</span></span>|<span data-ttu-id="468e6-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="468e6-168">DateTimeOffset</span></span>|<span data-ttu-id="468e6-169">Дата и время последней синхронизации устройства с Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="468e6-169">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="468e6-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="468e6-170">Response</span></span>
<span data-ttu-id="468e6-171">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="468e6-171">If successful, this method returns a `201 Created` response code and a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="468e6-172">Пример</span><span class="sxs-lookup"><span data-stu-id="468e6-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="468e6-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="468e6-173">Request</span></span>
<span data-ttu-id="468e6-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="468e6-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="468e6-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="468e6-175">Response</span></span>
<span data-ttu-id="468e6-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="468e6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






