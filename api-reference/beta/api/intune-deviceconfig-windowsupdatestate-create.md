---
title: Создание Виндовсупдатестате
description: Создание нового объекта Виндовсупдатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9a5437321741131f2a341c07514e57e50c5ea2be
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313701"
---
# <a name="create-windowsupdatestate"></a><span data-ttu-id="cec3d-103">Создание Виндовсупдатестате</span><span class="sxs-lookup"><span data-stu-id="cec3d-103">Create windowsUpdateState</span></span>

> <span data-ttu-id="cec3d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cec3d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cec3d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cec3d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cec3d-106">Создание нового объекта [виндовсупдатестате](../resources/intune-deviceconfig-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="cec3d-106">Create a new [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cec3d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cec3d-107">Prerequisites</span></span>
<span data-ttu-id="cec3d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cec3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cec3d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cec3d-110">Permission type</span></span>|<span data-ttu-id="cec3d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cec3d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cec3d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cec3d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cec3d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cec3d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cec3d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cec3d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cec3d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cec3d-115">Not supported.</span></span>|
|<span data-ttu-id="cec3d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cec3d-116">Application</span></span>|<span data-ttu-id="cec3d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cec3d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cec3d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cec3d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="cec3d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cec3d-119">Request headers</span></span>
|<span data-ttu-id="cec3d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cec3d-120">Header</span></span>|<span data-ttu-id="cec3d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cec3d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cec3d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cec3d-122">Authorization</span></span>|<span data-ttu-id="cec3d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cec3d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cec3d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cec3d-124">Accept</span></span>|<span data-ttu-id="cec3d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cec3d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cec3d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cec3d-126">Request body</span></span>
<span data-ttu-id="cec3d-127">В тексте запроса добавьте представление объекта Виндовсупдатестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cec3d-127">In the request body, supply a JSON representation for the windowsUpdateState object.</span></span>

<span data-ttu-id="cec3d-128">В следующей таблице приведены свойства, необходимые при создании Виндовсупдатестате.</span><span class="sxs-lookup"><span data-stu-id="cec3d-128">The following table shows the properties that are required when you create the windowsUpdateState.</span></span>

|<span data-ttu-id="cec3d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cec3d-129">Property</span></span>|<span data-ttu-id="cec3d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cec3d-130">Type</span></span>|<span data-ttu-id="cec3d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cec3d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cec3d-132">id</span><span class="sxs-lookup"><span data-stu-id="cec3d-132">id</span></span>|<span data-ttu-id="cec3d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="cec3d-133">String</span></span>|<span data-ttu-id="cec3d-134">Это идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="cec3d-134">This is Id of the entity.</span></span>|
|<span data-ttu-id="cec3d-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="cec3d-135">deviceId</span></span>|<span data-ttu-id="cec3d-136">String</span><span class="sxs-lookup"><span data-stu-id="cec3d-136">String</span></span>|<span data-ttu-id="cec3d-137">Идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="cec3d-137">The id of the device.</span></span>|
|<span data-ttu-id="cec3d-138">userId</span><span class="sxs-lookup"><span data-stu-id="cec3d-138">userId</span></span>|<span data-ttu-id="cec3d-139">String</span><span class="sxs-lookup"><span data-stu-id="cec3d-139">String</span></span>|<span data-ttu-id="cec3d-140">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="cec3d-140">The id of the user.</span></span>|
|<span data-ttu-id="cec3d-141">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="cec3d-141">deviceDisplayName</span></span>|<span data-ttu-id="cec3d-142">String</span><span class="sxs-lookup"><span data-stu-id="cec3d-142">String</span></span>|<span data-ttu-id="cec3d-143">Отображаемое имя устройства.</span><span class="sxs-lookup"><span data-stu-id="cec3d-143">Device display name.</span></span>|
|<span data-ttu-id="cec3d-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cec3d-144">userPrincipalName</span></span>|<span data-ttu-id="cec3d-145">Строка</span><span class="sxs-lookup"><span data-stu-id="cec3d-145">String</span></span>|<span data-ttu-id="cec3d-146">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="cec3d-146">User principal name.</span></span>|
|<span data-ttu-id="cec3d-147">status</span><span class="sxs-lookup"><span data-stu-id="cec3d-147">status</span></span>|[<span data-ttu-id="cec3d-148">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="cec3d-148">windowsUpdateStatus</span></span>](../resources/intune-deviceconfig-windowsupdatestatus.md)|<span data-ttu-id="cec3d-149">Состояние Windows удпате.</span><span class="sxs-lookup"><span data-stu-id="cec3d-149">Windows udpate status.</span></span> <span data-ttu-id="cec3d-150">Возможные значения: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="cec3d-150">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="cec3d-151">куалитюпдатеверсион</span><span class="sxs-lookup"><span data-stu-id="cec3d-151">qualityUpdateVersion</span></span>|<span data-ttu-id="cec3d-152">String</span><span class="sxs-lookup"><span data-stu-id="cec3d-152">String</span></span>|<span data-ttu-id="cec3d-153">Версия устройства для обновления качества.</span><span class="sxs-lookup"><span data-stu-id="cec3d-153">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="cec3d-154">феатуреупдатеверсион</span><span class="sxs-lookup"><span data-stu-id="cec3d-154">featureUpdateVersion</span></span>|<span data-ttu-id="cec3d-155">String</span><span class="sxs-lookup"><span data-stu-id="cec3d-155">String</span></span>|<span data-ttu-id="cec3d-156">Текущая версия обновления компонентов устройства.</span><span class="sxs-lookup"><span data-stu-id="cec3d-156">The current feature update version of the device.</span></span>|
|<span data-ttu-id="cec3d-157">ластскандатетиме</span><span class="sxs-lookup"><span data-stu-id="cec3d-157">lastScanDateTime</span></span>|<span data-ttu-id="cec3d-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cec3d-158">DateTimeOffset</span></span>|<span data-ttu-id="cec3d-159">Дата и время, когда агент обновления Windows успешно выполнил сканирование.</span><span class="sxs-lookup"><span data-stu-id="cec3d-159">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="cec3d-160">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="cec3d-160">lastSyncDateTime</span></span>|<span data-ttu-id="cec3d-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cec3d-161">DateTimeOffset</span></span>|<span data-ttu-id="cec3d-162">Дата и время последней синхронизации устройства с Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="cec3d-162">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="cec3d-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="cec3d-163">Response</span></span>
<span data-ttu-id="cec3d-164">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсупдатестате](../resources/intune-deviceconfig-windowsupdatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cec3d-164">If successful, this method returns a `201 Created` response code and a [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cec3d-165">Пример</span><span class="sxs-lookup"><span data-stu-id="cec3d-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="cec3d-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="cec3d-166">Request</span></span>
<span data-ttu-id="cec3d-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cec3d-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cec3d-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="cec3d-168">Response</span></span>
<span data-ttu-id="cec3d-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cec3d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






