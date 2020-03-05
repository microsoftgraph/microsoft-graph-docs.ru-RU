---
title: Создание depOnboardingSetting
description: Создание нового объекта depOnboardingSetting.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 971702dfab6c4782bfe314d4061fd5cbaccc3794
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467139"
---
# <a name="create-deponboardingsetting"></a><span data-ttu-id="18080-103">Создание depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="18080-103">Create depOnboardingSetting</span></span>

<span data-ttu-id="18080-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="18080-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18080-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18080-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18080-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18080-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18080-107">Создание нового объекта [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="18080-107">Create a new [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18080-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="18080-108">Prerequisites</span></span>
<span data-ttu-id="18080-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18080-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18080-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18080-111">Permission type</span></span>|<span data-ttu-id="18080-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18080-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18080-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18080-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18080-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18080-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="18080-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18080-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18080-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18080-116">Not supported.</span></span>|
|<span data-ttu-id="18080-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18080-117">Application</span></span>|<span data-ttu-id="18080-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18080-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18080-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18080-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="18080-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="18080-120">Request headers</span></span>
|<span data-ttu-id="18080-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18080-121">Header</span></span>|<span data-ttu-id="18080-122">Значение</span><span class="sxs-lookup"><span data-stu-id="18080-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18080-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18080-123">Authorization</span></span>|<span data-ttu-id="18080-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18080-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18080-125">Accept</span><span class="sxs-lookup"><span data-stu-id="18080-125">Accept</span></span>|<span data-ttu-id="18080-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18080-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18080-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18080-127">Request body</span></span>
<span data-ttu-id="18080-128">В тексте запроса добавьте представление объекта depOnboardingSetting в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18080-128">In the request body, supply a JSON representation for the depOnboardingSetting object.</span></span>

<span data-ttu-id="18080-129">В следующей таблице приведены свойства, необходимые при создании depOnboardingSetting.</span><span class="sxs-lookup"><span data-stu-id="18080-129">The following table shows the properties that are required when you create the depOnboardingSetting.</span></span>

|<span data-ttu-id="18080-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="18080-130">Property</span></span>|<span data-ttu-id="18080-131">Тип</span><span class="sxs-lookup"><span data-stu-id="18080-131">Type</span></span>|<span data-ttu-id="18080-132">Описание</span><span class="sxs-lookup"><span data-stu-id="18080-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18080-133">id</span><span class="sxs-lookup"><span data-stu-id="18080-133">id</span></span>|<span data-ttu-id="18080-134">String</span><span class="sxs-lookup"><span data-stu-id="18080-134">String</span></span>|<span data-ttu-id="18080-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="18080-135">UUID for the object</span></span>|
|<span data-ttu-id="18080-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="18080-136">appleIdentifier</span></span>|<span data-ttu-id="18080-137">String</span><span class="sxs-lookup"><span data-stu-id="18080-137">String</span></span>|<span data-ttu-id="18080-138">Идентификатор Apple ID, используемый для получения текущего маркера.</span><span class="sxs-lookup"><span data-stu-id="18080-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="18080-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="18080-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="18080-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18080-140">DateTimeOffset</span></span>|<span data-ttu-id="18080-141">По истечении срока действия маркера.</span><span class="sxs-lookup"><span data-stu-id="18080-141">When the token will expire.</span></span>|
|<span data-ttu-id="18080-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18080-142">lastModifiedDateTime</span></span>|<span data-ttu-id="18080-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18080-143">DateTimeOffset</span></span>|<span data-ttu-id="18080-144">При подключении службы.</span><span class="sxs-lookup"><span data-stu-id="18080-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="18080-145">ластсукцессфулсинкдатетиме</span><span class="sxs-lookup"><span data-stu-id="18080-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="18080-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18080-146">DateTimeOffset</span></span>|<span data-ttu-id="18080-147">Когда служба последний синед с Intune</span><span class="sxs-lookup"><span data-stu-id="18080-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="18080-148">ластсинктригжереддатетиме</span><span class="sxs-lookup"><span data-stu-id="18080-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="18080-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18080-149">DateTimeOffset</span></span>|<span data-ttu-id="18080-150">При последнем запросе синхронизации в Intune.</span><span class="sxs-lookup"><span data-stu-id="18080-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="18080-151">Свойства sharetokenwithschooldatasyncservice</span><span class="sxs-lookup"><span data-stu-id="18080-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="18080-152">Логический</span><span class="sxs-lookup"><span data-stu-id="18080-152">Boolean</span></span>|<span data-ttu-id="18080-153">Указывает, включен ли общий доступ к маркеру DEP для службы School Data Sync.</span><span class="sxs-lookup"><span data-stu-id="18080-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="18080-154">Lastsyncerrorcode к объекту</span><span class="sxs-lookup"><span data-stu-id="18080-154">lastSyncErrorCode</span></span>|<span data-ttu-id="18080-155">Int32</span><span class="sxs-lookup"><span data-stu-id="18080-155">Int32</span></span>|<span data-ttu-id="18080-156">Код ошибки, полученный от Apple во время последней синхронизации DEP.</span><span class="sxs-lookup"><span data-stu-id="18080-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="18080-157">токентипе</span><span class="sxs-lookup"><span data-stu-id="18080-157">tokenType</span></span>|<span data-ttu-id="18080-158">[depTokenType](../resources/intune-enrollment-deptokentype.md);</span><span class="sxs-lookup"><span data-stu-id="18080-158">[depTokenType](../resources/intune-enrollment-deptokentype.md)</span></span>|<span data-ttu-id="18080-159">Получает или задает тип токена DEP.</span><span class="sxs-lookup"><span data-stu-id="18080-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="18080-160">Возможные значения: `none`, `dep`, `appleSchoolManager`.</span><span class="sxs-lookup"><span data-stu-id="18080-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="18080-161">токеннаме</span><span class="sxs-lookup"><span data-stu-id="18080-161">tokenName</span></span>|<span data-ttu-id="18080-162">String</span><span class="sxs-lookup"><span data-stu-id="18080-162">String</span></span>|<span data-ttu-id="18080-163">Понятное имя для токена DEP</span><span class="sxs-lookup"><span data-stu-id="18080-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="18080-164">синцеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="18080-164">syncedDeviceCount</span></span>|<span data-ttu-id="18080-165">Int32</span><span class="sxs-lookup"><span data-stu-id="18080-165">Int32</span></span>|<span data-ttu-id="18080-166">Получает число синхронизированных устройств</span><span class="sxs-lookup"><span data-stu-id="18080-166">Gets synced device count</span></span>|
|<span data-ttu-id="18080-167">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="18080-167">dataSharingConsentGranted</span></span>|<span data-ttu-id="18080-168">Логический</span><span class="sxs-lookup"><span data-stu-id="18080-168">Boolean</span></span>|<span data-ttu-id="18080-169">Разрешение, предоставленное для предоставления общего доступа к данным с помощью службы Apple DEP</span><span class="sxs-lookup"><span data-stu-id="18080-169">Consent granted for data sharing with Apple Dep Service</span></span>|
|<span data-ttu-id="18080-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="18080-170">roleScopeTagIds</span></span>|<span data-ttu-id="18080-171">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="18080-171">String collection</span></span>|<span data-ttu-id="18080-172">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="18080-172">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="18080-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="18080-173">Response</span></span>
<span data-ttu-id="18080-174">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18080-174">If successful, this method returns a `201 Created` response code and a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18080-175">Пример</span><span class="sxs-lookup"><span data-stu-id="18080-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="18080-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="18080-176">Request</span></span>
<span data-ttu-id="18080-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18080-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
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

### <a name="response"></a><span data-ttu-id="18080-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="18080-178">Response</span></span>
<span data-ttu-id="18080-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18080-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





