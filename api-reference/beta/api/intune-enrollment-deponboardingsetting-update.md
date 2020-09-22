---
title: Обновление depOnboardingSetting
description: Обновление свойств объекта depOnboardingSetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5af52b0f1d06edf1908f90d153e2036e5de3c03e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054170"
---
# <a name="update-deponboardingsetting"></a><span data-ttu-id="f99d1-103">Обновление depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="f99d1-103">Update depOnboardingSetting</span></span>

<span data-ttu-id="f99d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f99d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f99d1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f99d1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f99d1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f99d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f99d1-107">Обновление свойств объекта [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="f99d1-107">Update the properties of a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f99d1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f99d1-108">Prerequisites</span></span>
<span data-ttu-id="f99d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f99d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f99d1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f99d1-111">Permission type</span></span>|<span data-ttu-id="f99d1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f99d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f99d1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f99d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f99d1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f99d1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f99d1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f99d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f99d1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f99d1-116">Not supported.</span></span>|
|<span data-ttu-id="f99d1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f99d1-117">Application</span></span>|<span data-ttu-id="f99d1-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f99d1-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f99d1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f99d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="request-headers"></a><span data-ttu-id="f99d1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f99d1-120">Request headers</span></span>
|<span data-ttu-id="f99d1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f99d1-121">Header</span></span>|<span data-ttu-id="f99d1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f99d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f99d1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f99d1-123">Authorization</span></span>|<span data-ttu-id="f99d1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f99d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f99d1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f99d1-125">Accept</span></span>|<span data-ttu-id="f99d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f99d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f99d1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f99d1-127">Request body</span></span>
<span data-ttu-id="f99d1-128">В тексте запроса добавьте представление объекта [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f99d1-128">In the request body, supply a JSON representation for the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

<span data-ttu-id="f99d1-129">В следующей таблице приведены свойства, необходимые при создании [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).</span><span class="sxs-lookup"><span data-stu-id="f99d1-129">The following table shows the properties that are required when you create the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).</span></span>

|<span data-ttu-id="f99d1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f99d1-130">Property</span></span>|<span data-ttu-id="f99d1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f99d1-131">Type</span></span>|<span data-ttu-id="f99d1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f99d1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f99d1-133">id</span><span class="sxs-lookup"><span data-stu-id="f99d1-133">id</span></span>|<span data-ttu-id="f99d1-134">String</span><span class="sxs-lookup"><span data-stu-id="f99d1-134">String</span></span>|<span data-ttu-id="f99d1-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="f99d1-135">UUID for the object</span></span>|
|<span data-ttu-id="f99d1-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="f99d1-136">appleIdentifier</span></span>|<span data-ttu-id="f99d1-137">String</span><span class="sxs-lookup"><span data-stu-id="f99d1-137">String</span></span>|<span data-ttu-id="f99d1-138">Идентификатор Apple ID, используемый для получения текущего маркера.</span><span class="sxs-lookup"><span data-stu-id="f99d1-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="f99d1-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f99d1-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="f99d1-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f99d1-140">DateTimeOffset</span></span>|<span data-ttu-id="f99d1-141">По истечении срока действия маркера.</span><span class="sxs-lookup"><span data-stu-id="f99d1-141">When the token will expire.</span></span>|
|<span data-ttu-id="f99d1-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f99d1-142">lastModifiedDateTime</span></span>|<span data-ttu-id="f99d1-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f99d1-143">DateTimeOffset</span></span>|<span data-ttu-id="f99d1-144">При подключении службы.</span><span class="sxs-lookup"><span data-stu-id="f99d1-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="f99d1-145">ластсукцессфулсинкдатетиме</span><span class="sxs-lookup"><span data-stu-id="f99d1-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="f99d1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f99d1-146">DateTimeOffset</span></span>|<span data-ttu-id="f99d1-147">Когда служба последний синед с Intune</span><span class="sxs-lookup"><span data-stu-id="f99d1-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="f99d1-148">ластсинктригжереддатетиме</span><span class="sxs-lookup"><span data-stu-id="f99d1-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="f99d1-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f99d1-149">DateTimeOffset</span></span>|<span data-ttu-id="f99d1-150">При последнем запросе синхронизации в Intune.</span><span class="sxs-lookup"><span data-stu-id="f99d1-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="f99d1-151">Свойства sharetokenwithschooldatasyncservice</span><span class="sxs-lookup"><span data-stu-id="f99d1-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="f99d1-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="f99d1-152">Boolean</span></span>|<span data-ttu-id="f99d1-153">Указывает, включен ли общий доступ к маркеру DEP для службы School Data Sync.</span><span class="sxs-lookup"><span data-stu-id="f99d1-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="f99d1-154">Lastsyncerrorcode к объекту</span><span class="sxs-lookup"><span data-stu-id="f99d1-154">lastSyncErrorCode</span></span>|<span data-ttu-id="f99d1-155">Int32</span><span class="sxs-lookup"><span data-stu-id="f99d1-155">Int32</span></span>|<span data-ttu-id="f99d1-156">Код ошибки, полученный от Apple во время последней синхронизации DEP.</span><span class="sxs-lookup"><span data-stu-id="f99d1-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="f99d1-157">токентипе</span><span class="sxs-lookup"><span data-stu-id="f99d1-157">tokenType</span></span>|<span data-ttu-id="f99d1-158">[depTokenType](../resources/intune-enrollment-deptokentype.md);</span><span class="sxs-lookup"><span data-stu-id="f99d1-158">[depTokenType](../resources/intune-enrollment-deptokentype.md)</span></span>|<span data-ttu-id="f99d1-159">Получает или задает тип токена DEP.</span><span class="sxs-lookup"><span data-stu-id="f99d1-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="f99d1-160">Возможные значения: `none`, `dep`, `appleSchoolManager`.</span><span class="sxs-lookup"><span data-stu-id="f99d1-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="f99d1-161">токеннаме</span><span class="sxs-lookup"><span data-stu-id="f99d1-161">tokenName</span></span>|<span data-ttu-id="f99d1-162">String</span><span class="sxs-lookup"><span data-stu-id="f99d1-162">String</span></span>|<span data-ttu-id="f99d1-163">Понятное имя для токена DEP</span><span class="sxs-lookup"><span data-stu-id="f99d1-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="f99d1-164">синцеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="f99d1-164">syncedDeviceCount</span></span>|<span data-ttu-id="f99d1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f99d1-165">Int32</span></span>|<span data-ttu-id="f99d1-166">Получает число синхронизированных устройств</span><span class="sxs-lookup"><span data-stu-id="f99d1-166">Gets synced device count</span></span>|
|<span data-ttu-id="f99d1-167">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="f99d1-167">dataSharingConsentGranted</span></span>|<span data-ttu-id="f99d1-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="f99d1-168">Boolean</span></span>|<span data-ttu-id="f99d1-169">Разрешение, предоставленное для предоставления общего доступа к данным с помощью службы Apple DEP</span><span class="sxs-lookup"><span data-stu-id="f99d1-169">Consent granted for data sharing with Apple Dep Service</span></span>|
|<span data-ttu-id="f99d1-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f99d1-170">roleScopeTagIds</span></span>|<span data-ttu-id="f99d1-171">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="f99d1-171">String collection</span></span>|<span data-ttu-id="f99d1-172">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f99d1-172">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="f99d1-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="f99d1-173">Response</span></span>
<span data-ttu-id="f99d1-174">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f99d1-174">If successful, this method returns a `200 OK` response code and an updated [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f99d1-175">Пример</span><span class="sxs-lookup"><span data-stu-id="f99d1-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="f99d1-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="f99d1-176">Request</span></span>
<span data-ttu-id="f99d1-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f99d1-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f99d1-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="f99d1-178">Response</span></span>
<span data-ttu-id="f99d1-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f99d1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






