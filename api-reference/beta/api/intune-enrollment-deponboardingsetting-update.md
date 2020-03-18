---
title: Обновление depOnboardingSetting
description: Обновление свойств объекта depOnboardingSetting.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cb36a7e6a8205144ac02a8d373a2c2e728029cee
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813213"
---
# <a name="update-deponboardingsetting"></a><span data-ttu-id="99969-103">Обновление depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="99969-103">Update depOnboardingSetting</span></span>

> <span data-ttu-id="99969-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99969-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99969-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="99969-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99969-106">Обновление свойств объекта [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="99969-106">Update the properties of a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99969-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="99969-107">Prerequisites</span></span>
<span data-ttu-id="99969-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99969-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99969-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99969-110">Permission type</span></span>|<span data-ttu-id="99969-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="99969-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99969-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99969-112">Delegated (work or school account)</span></span>|<span data-ttu-id="99969-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99969-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="99969-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99969-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99969-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99969-115">Not supported.</span></span>|
|<span data-ttu-id="99969-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="99969-116">Application</span></span>|<span data-ttu-id="99969-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99969-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99969-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99969-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="request-headers"></a><span data-ttu-id="99969-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="99969-119">Request headers</span></span>
|<span data-ttu-id="99969-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="99969-120">Header</span></span>|<span data-ttu-id="99969-121">Значение</span><span class="sxs-lookup"><span data-stu-id="99969-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99969-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="99969-122">Authorization</span></span>|<span data-ttu-id="99969-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99969-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99969-124">Accept</span><span class="sxs-lookup"><span data-stu-id="99969-124">Accept</span></span>|<span data-ttu-id="99969-125">application/json</span><span class="sxs-lookup"><span data-stu-id="99969-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99969-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99969-126">Request body</span></span>
<span data-ttu-id="99969-127">В тексте запроса добавьте представление объекта [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99969-127">In the request body, supply a JSON representation for the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

<span data-ttu-id="99969-128">В следующей таблице приведены свойства, необходимые при создании [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).</span><span class="sxs-lookup"><span data-stu-id="99969-128">The following table shows the properties that are required when you create the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).</span></span>

|<span data-ttu-id="99969-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="99969-129">Property</span></span>|<span data-ttu-id="99969-130">Тип</span><span class="sxs-lookup"><span data-stu-id="99969-130">Type</span></span>|<span data-ttu-id="99969-131">Описание</span><span class="sxs-lookup"><span data-stu-id="99969-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99969-132">id</span><span class="sxs-lookup"><span data-stu-id="99969-132">id</span></span>|<span data-ttu-id="99969-133">String</span><span class="sxs-lookup"><span data-stu-id="99969-133">String</span></span>|<span data-ttu-id="99969-134">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="99969-134">UUID for the object</span></span>|
|<span data-ttu-id="99969-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="99969-135">appleIdentifier</span></span>|<span data-ttu-id="99969-136">String</span><span class="sxs-lookup"><span data-stu-id="99969-136">String</span></span>|<span data-ttu-id="99969-137">Идентификатор Apple ID, используемый для получения текущего маркера.</span><span class="sxs-lookup"><span data-stu-id="99969-137">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="99969-138">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="99969-138">tokenExpirationDateTime</span></span>|<span data-ttu-id="99969-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99969-139">DateTimeOffset</span></span>|<span data-ttu-id="99969-140">По истечении срока действия маркера.</span><span class="sxs-lookup"><span data-stu-id="99969-140">When the token will expire.</span></span>|
|<span data-ttu-id="99969-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99969-141">lastModifiedDateTime</span></span>|<span data-ttu-id="99969-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99969-142">DateTimeOffset</span></span>|<span data-ttu-id="99969-143">При подключении службы.</span><span class="sxs-lookup"><span data-stu-id="99969-143">When the service was onboarded.</span></span>|
|<span data-ttu-id="99969-144">ластсукцессфулсинкдатетиме</span><span class="sxs-lookup"><span data-stu-id="99969-144">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="99969-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99969-145">DateTimeOffset</span></span>|<span data-ttu-id="99969-146">Когда служба последний синед с Intune</span><span class="sxs-lookup"><span data-stu-id="99969-146">When the service last syned with Intune</span></span>|
|<span data-ttu-id="99969-147">ластсинктригжереддатетиме</span><span class="sxs-lookup"><span data-stu-id="99969-147">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="99969-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99969-148">DateTimeOffset</span></span>|<span data-ttu-id="99969-149">При последнем запросе синхронизации в Intune.</span><span class="sxs-lookup"><span data-stu-id="99969-149">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="99969-150">Свойства sharetokenwithschooldatasyncservice</span><span class="sxs-lookup"><span data-stu-id="99969-150">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="99969-151">Логический</span><span class="sxs-lookup"><span data-stu-id="99969-151">Boolean</span></span>|<span data-ttu-id="99969-152">Указывает, включен ли общий доступ к маркеру DEP для службы School Data Sync.</span><span class="sxs-lookup"><span data-stu-id="99969-152">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="99969-153">Lastsyncerrorcode к объекту</span><span class="sxs-lookup"><span data-stu-id="99969-153">lastSyncErrorCode</span></span>|<span data-ttu-id="99969-154">Int32</span><span class="sxs-lookup"><span data-stu-id="99969-154">Int32</span></span>|<span data-ttu-id="99969-155">Код ошибки, полученный от Apple во время последней синхронизации DEP.</span><span class="sxs-lookup"><span data-stu-id="99969-155">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="99969-156">токентипе</span><span class="sxs-lookup"><span data-stu-id="99969-156">tokenType</span></span>|<span data-ttu-id="99969-157">[depTokenType](../resources/intune-enrollment-deptokentype.md);</span><span class="sxs-lookup"><span data-stu-id="99969-157">[depTokenType](../resources/intune-enrollment-deptokentype.md)</span></span>|<span data-ttu-id="99969-158">Получает или задает тип токена DEP.</span><span class="sxs-lookup"><span data-stu-id="99969-158">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="99969-159">Возможные значения: `none`, `dep`, `appleSchoolManager`.</span><span class="sxs-lookup"><span data-stu-id="99969-159">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="99969-160">токеннаме</span><span class="sxs-lookup"><span data-stu-id="99969-160">tokenName</span></span>|<span data-ttu-id="99969-161">String</span><span class="sxs-lookup"><span data-stu-id="99969-161">String</span></span>|<span data-ttu-id="99969-162">Понятное имя для токена DEP</span><span class="sxs-lookup"><span data-stu-id="99969-162">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="99969-163">синцеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="99969-163">syncedDeviceCount</span></span>|<span data-ttu-id="99969-164">Int32</span><span class="sxs-lookup"><span data-stu-id="99969-164">Int32</span></span>|<span data-ttu-id="99969-165">Получает число синхронизированных устройств</span><span class="sxs-lookup"><span data-stu-id="99969-165">Gets synced device count</span></span>|
|<span data-ttu-id="99969-166">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="99969-166">dataSharingConsentGranted</span></span>|<span data-ttu-id="99969-167">Логический</span><span class="sxs-lookup"><span data-stu-id="99969-167">Boolean</span></span>|<span data-ttu-id="99969-168">Разрешение, предоставленное для предоставления общего доступа к данным с помощью службы Apple DEP</span><span class="sxs-lookup"><span data-stu-id="99969-168">Consent granted for data sharing with Apple Dep Service</span></span>|
|<span data-ttu-id="99969-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="99969-169">roleScopeTagIds</span></span>|<span data-ttu-id="99969-170">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="99969-170">String collection</span></span>|<span data-ttu-id="99969-171">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="99969-171">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="99969-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="99969-172">Response</span></span>
<span data-ttu-id="99969-173">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="99969-173">If successful, this method returns a `200 OK` response code and an updated [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99969-174">Пример</span><span class="sxs-lookup"><span data-stu-id="99969-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="99969-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="99969-175">Request</span></span>
<span data-ttu-id="99969-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99969-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
Content-type: application/json
Content-length: 576

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="99969-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="99969-177">Response</span></span>
<span data-ttu-id="99969-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="99969-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 689

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "id": "40342229-2229-4034-2922-344029223440",
  "appleIdentifier": "Apple Identifier value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
  "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1,
  "tokenType": "dep",
  "tokenName": "Token Name value",
  "syncedDeviceCount": 1,
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




