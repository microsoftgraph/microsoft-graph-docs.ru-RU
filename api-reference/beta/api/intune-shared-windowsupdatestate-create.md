---
title: Создание Виндовсупдатестате
description: Создание нового объекта Виндовсупдатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 32f3bd844ad028a894eeacdf0cc5a052053fa124
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201142"
---
# <a name="create-windowsupdatestate"></a><span data-ttu-id="bcf09-103">Создание Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="bcf09-103">Create windowsUpdateState</span></span>

> <span data-ttu-id="bcf09-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcf09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcf09-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bcf09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcf09-106">Создание нового объекта [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="bcf09-106">Create a new [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bcf09-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bcf09-107">Prerequisites</span></span>
<span data-ttu-id="bcf09-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcf09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcf09-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcf09-110">Permission type</span></span>|<span data-ttu-id="bcf09-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcf09-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcf09-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcf09-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bcf09-113">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="bcf09-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="bcf09-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcf09-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="bcf09-115">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="bcf09-115">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="bcf09-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcf09-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bcf09-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcf09-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcf09-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcf09-118">Not supported.</span></span>|
|<span data-ttu-id="bcf09-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcf09-119">Application</span></span>||
| <span data-ttu-id="bcf09-120">&nbsp; &nbsp; **Настройка устройства**</span><span class="sxs-lookup"><span data-stu-id="bcf09-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="bcf09-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcf09-121">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="bcf09-122">&nbsp;&nbsp; **Обновление программного обеспечения**</span><span class="sxs-lookup"><span data-stu-id="bcf09-122">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="bcf09-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcf09-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcf09-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcf09-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="bcf09-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcf09-125">Request headers</span></span>
|<span data-ttu-id="bcf09-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bcf09-126">Header</span></span>|<span data-ttu-id="bcf09-127">Значение</span><span class="sxs-lookup"><span data-stu-id="bcf09-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcf09-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bcf09-128">Authorization</span></span>|<span data-ttu-id="bcf09-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcf09-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcf09-130">Accept</span><span class="sxs-lookup"><span data-stu-id="bcf09-130">Accept</span></span>|<span data-ttu-id="bcf09-131">application/json</span><span class="sxs-lookup"><span data-stu-id="bcf09-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcf09-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bcf09-132">Request body</span></span>
<span data-ttu-id="bcf09-133">В тексте запроса добавьте представление объекта Виндовсупдатестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bcf09-133">In the request body, supply a JSON representation for the windowsUpdateState object.</span></span>

<span data-ttu-id="bcf09-134">В следующей таблице приведены свойства, необходимые при создании Виндовсупдатестате.</span><span class="sxs-lookup"><span data-stu-id="bcf09-134">The following table shows the properties that are required when you create the windowsUpdateState.</span></span>

|<span data-ttu-id="bcf09-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="bcf09-135">Property</span></span>|<span data-ttu-id="bcf09-136">Тип</span><span class="sxs-lookup"><span data-stu-id="bcf09-136">Type</span></span>|<span data-ttu-id="bcf09-137">Описание</span><span class="sxs-lookup"><span data-stu-id="bcf09-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcf09-138">id</span><span class="sxs-lookup"><span data-stu-id="bcf09-138">id</span></span>|<span data-ttu-id="bcf09-139">Строка</span><span class="sxs-lookup"><span data-stu-id="bcf09-139">String</span></span>|<span data-ttu-id="bcf09-140">Это идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="bcf09-140">This is Id of the entity.</span></span>|
|<span data-ttu-id="bcf09-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="bcf09-141">deviceId</span></span>|<span data-ttu-id="bcf09-142">String.</span><span class="sxs-lookup"><span data-stu-id="bcf09-142">String</span></span>|<span data-ttu-id="bcf09-143">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="bcf09-143">The id of the device.</span></span>|
|<span data-ttu-id="bcf09-144">userId</span><span class="sxs-lookup"><span data-stu-id="bcf09-144">userId</span></span>|<span data-ttu-id="bcf09-145">String</span><span class="sxs-lookup"><span data-stu-id="bcf09-145">String</span></span>|<span data-ttu-id="bcf09-146">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="bcf09-146">The id of the user.</span></span>|
|<span data-ttu-id="bcf09-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="bcf09-147">deviceDisplayName</span></span>|<span data-ttu-id="bcf09-148">String</span><span class="sxs-lookup"><span data-stu-id="bcf09-148">String</span></span>|<span data-ttu-id="bcf09-149">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="bcf09-149">Device display name.</span></span>|
|<span data-ttu-id="bcf09-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bcf09-150">userPrincipalName</span></span>|<span data-ttu-id="bcf09-151">Строка</span><span class="sxs-lookup"><span data-stu-id="bcf09-151">String</span></span>|<span data-ttu-id="bcf09-152">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="bcf09-152">User principal name.</span></span>|
|<span data-ttu-id="bcf09-153">status</span><span class="sxs-lookup"><span data-stu-id="bcf09-153">status</span></span>|[<span data-ttu-id="bcf09-154">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="bcf09-154">windowsUpdateStatus</span></span>](../resources/intune-shared-windowsupdatestatus.md)|<span data-ttu-id="bcf09-155">Состояние Windows удпате.</span><span class="sxs-lookup"><span data-stu-id="bcf09-155">Windows udpate status.</span></span> <span data-ttu-id="bcf09-156">Возможные значения: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="bcf09-156">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="bcf09-157">куалитюпдатеверсион</span><span class="sxs-lookup"><span data-stu-id="bcf09-157">qualityUpdateVersion</span></span>|<span data-ttu-id="bcf09-158">String.</span><span class="sxs-lookup"><span data-stu-id="bcf09-158">String</span></span>|<span data-ttu-id="bcf09-159">Версия устройства для обновления качества.</span><span class="sxs-lookup"><span data-stu-id="bcf09-159">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="bcf09-160">феатуреупдатеверсион</span><span class="sxs-lookup"><span data-stu-id="bcf09-160">featureUpdateVersion</span></span>|<span data-ttu-id="bcf09-161">String.</span><span class="sxs-lookup"><span data-stu-id="bcf09-161">String</span></span>|<span data-ttu-id="bcf09-162">Текущая версия обновления компонентов устройства.</span><span class="sxs-lookup"><span data-stu-id="bcf09-162">The current feature update version of the device.</span></span>|
|<span data-ttu-id="bcf09-163">ластскандатетиме</span><span class="sxs-lookup"><span data-stu-id="bcf09-163">lastScanDateTime</span></span>|<span data-ttu-id="bcf09-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcf09-164">DateTimeOffset</span></span>|<span data-ttu-id="bcf09-165">Дата и время, когда агент обновления Windows успешно выполнил сканирование.</span><span class="sxs-lookup"><span data-stu-id="bcf09-165">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="bcf09-166">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="bcf09-166">lastSyncDateTime</span></span>|<span data-ttu-id="bcf09-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcf09-167">DateTimeOffset</span></span>|<span data-ttu-id="bcf09-168">Дата и время последней синхронизации устройства с Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="bcf09-168">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="bcf09-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcf09-169">Response</span></span>
<span data-ttu-id="bcf09-170">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсупдатестате](../resources/intune-shared-windowsupdatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bcf09-170">If successful, this method returns a `201 Created` response code and a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcf09-171">Пример</span><span class="sxs-lookup"><span data-stu-id="bcf09-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="bcf09-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcf09-172">Request</span></span>
<span data-ttu-id="bcf09-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcf09-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bcf09-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcf09-174">Response</span></span>
<span data-ttu-id="bcf09-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bcf09-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




