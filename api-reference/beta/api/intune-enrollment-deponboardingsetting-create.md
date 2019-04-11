---
title: Создание depOnboardingSetting
description: Создание нового объекта depOnboardingSetting.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1329f2a3bc4694bb288cda75c59271eadee8f8c5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797671"
---
# <a name="create-deponboardingsetting"></a><span data-ttu-id="d8adc-103">Создание depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="d8adc-103">Create depOnboardingSetting</span></span>

> <span data-ttu-id="d8adc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8adc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8adc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8adc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8adc-106">Создание нового объекта [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="d8adc-106">Create a new [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8adc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d8adc-107">Prerequisites</span></span>
<span data-ttu-id="d8adc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8adc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8adc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8adc-110">Permission type</span></span>|<span data-ttu-id="d8adc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8adc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8adc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8adc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d8adc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8adc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d8adc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8adc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8adc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8adc-115">Not supported.</span></span>|
|<span data-ttu-id="d8adc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8adc-116">Application</span></span>|<span data-ttu-id="d8adc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8adc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8adc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8adc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="d8adc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8adc-119">Request headers</span></span>
|<span data-ttu-id="d8adc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8adc-120">Header</span></span>|<span data-ttu-id="d8adc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d8adc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8adc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8adc-122">Authorization</span></span>|<span data-ttu-id="d8adc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8adc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8adc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d8adc-124">Accept</span></span>|<span data-ttu-id="d8adc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d8adc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8adc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8adc-126">Request body</span></span>
<span data-ttu-id="d8adc-127">В тексте запроса добавьте представление объекта depOnboardingSetting в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8adc-127">In the request body, supply a JSON representation for the depOnboardingSetting object.</span></span>

<span data-ttu-id="d8adc-128">В следующей таблице приведены свойства, необходимые при создании depOnboardingSetting.</span><span class="sxs-lookup"><span data-stu-id="d8adc-128">The following table shows the properties that are required when you create the depOnboardingSetting.</span></span>

|<span data-ttu-id="d8adc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8adc-129">Property</span></span>|<span data-ttu-id="d8adc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d8adc-130">Type</span></span>|<span data-ttu-id="d8adc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d8adc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8adc-132">id</span><span class="sxs-lookup"><span data-stu-id="d8adc-132">id</span></span>|<span data-ttu-id="d8adc-133">String</span><span class="sxs-lookup"><span data-stu-id="d8adc-133">String</span></span>|<span data-ttu-id="d8adc-134">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="d8adc-134">UUID for the object</span></span>|
|<span data-ttu-id="d8adc-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="d8adc-135">appleIdentifier</span></span>|<span data-ttu-id="d8adc-136">String</span><span class="sxs-lookup"><span data-stu-id="d8adc-136">String</span></span>|<span data-ttu-id="d8adc-137">Идентификатор Apple ID, используемый для получения текущего маркера.</span><span class="sxs-lookup"><span data-stu-id="d8adc-137">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="d8adc-138">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d8adc-138">tokenExpirationDateTime</span></span>|<span data-ttu-id="d8adc-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8adc-139">DateTimeOffset</span></span>|<span data-ttu-id="d8adc-140">По истечении срока действия маркера.</span><span class="sxs-lookup"><span data-stu-id="d8adc-140">When the token will expire.</span></span>|
|<span data-ttu-id="d8adc-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8adc-141">lastModifiedDateTime</span></span>|<span data-ttu-id="d8adc-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8adc-142">DateTimeOffset</span></span>|<span data-ttu-id="d8adc-143">При подключении службы.</span><span class="sxs-lookup"><span data-stu-id="d8adc-143">When the service was onboarded.</span></span>|
|<span data-ttu-id="d8adc-144">Ластсукцессфулсинкдатетиме</span><span class="sxs-lookup"><span data-stu-id="d8adc-144">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="d8adc-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8adc-145">DateTimeOffset</span></span>|<span data-ttu-id="d8adc-146">Когда служба последний синед с Intune</span><span class="sxs-lookup"><span data-stu-id="d8adc-146">When the service last syned with Intune</span></span>|
|<span data-ttu-id="d8adc-147">Ластсинктригжереддатетиме</span><span class="sxs-lookup"><span data-stu-id="d8adc-147">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="d8adc-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8adc-148">DateTimeOffset</span></span>|<span data-ttu-id="d8adc-149">При последнем запросе синхронизации в Intune.</span><span class="sxs-lookup"><span data-stu-id="d8adc-149">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="d8adc-150">Свойства sharetokenwithschooldatasyncservice</span><span class="sxs-lookup"><span data-stu-id="d8adc-150">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="d8adc-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8adc-151">Boolean</span></span>|<span data-ttu-id="d8adc-152">Указывает, включен ли общий доступ к маркеру DEP для службы School Data Sync.</span><span class="sxs-lookup"><span data-stu-id="d8adc-152">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="d8adc-153">Lastsyncerrorcode к объекту</span><span class="sxs-lookup"><span data-stu-id="d8adc-153">lastSyncErrorCode</span></span>|<span data-ttu-id="d8adc-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d8adc-154">Int32</span></span>|<span data-ttu-id="d8adc-155">Код ошибки, полученный от Apple во время последней синхронизации DEP.</span><span class="sxs-lookup"><span data-stu-id="d8adc-155">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="d8adc-156">Токентипе</span><span class="sxs-lookup"><span data-stu-id="d8adc-156">tokenType</span></span>|[<span data-ttu-id="d8adc-157">depTokenType</span><span class="sxs-lookup"><span data-stu-id="d8adc-157">depTokenType</span></span>](../resources/intune-enrollment-deptokentype.md)|<span data-ttu-id="d8adc-158">Получает или задает тип токена DEP.</span><span class="sxs-lookup"><span data-stu-id="d8adc-158">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="d8adc-159">Возможные значения: `none`, `dep`, `appleSchoolManager`.</span><span class="sxs-lookup"><span data-stu-id="d8adc-159">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="d8adc-160">Токеннаме</span><span class="sxs-lookup"><span data-stu-id="d8adc-160">tokenName</span></span>|<span data-ttu-id="d8adc-161">String</span><span class="sxs-lookup"><span data-stu-id="d8adc-161">String</span></span>|<span data-ttu-id="d8adc-162">Понятное имя для токена DEP</span><span class="sxs-lookup"><span data-stu-id="d8adc-162">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="d8adc-163">Синцеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="d8adc-163">syncedDeviceCount</span></span>|<span data-ttu-id="d8adc-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d8adc-164">Int32</span></span>|<span data-ttu-id="d8adc-165">Получает число синхронизированных устройств</span><span class="sxs-lookup"><span data-stu-id="d8adc-165">Gets synced device count</span></span>|
|<span data-ttu-id="d8adc-166">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="d8adc-166">dataSharingConsentGranted</span></span>|<span data-ttu-id="d8adc-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8adc-167">Boolean</span></span>|<span data-ttu-id="d8adc-168">Разрешение, предоставленное для предоставления общего доступа к данным с помощью службы Apple DEP</span><span class="sxs-lookup"><span data-stu-id="d8adc-168">Consent granted for data sharing with Apple Dep Service</span></span>|
|<span data-ttu-id="d8adc-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d8adc-169">roleScopeTagIds</span></span>|<span data-ttu-id="d8adc-170">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d8adc-170">String collection</span></span>|<span data-ttu-id="d8adc-171">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d8adc-171">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="d8adc-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8adc-172">Response</span></span>
<span data-ttu-id="d8adc-173">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d8adc-173">If successful, this method returns a `201 Created` response code and a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8adc-174">Пример</span><span class="sxs-lookup"><span data-stu-id="d8adc-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8adc-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8adc-175">Request</span></span>
<span data-ttu-id="d8adc-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8adc-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d8adc-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8adc-177">Response</span></span>
<span data-ttu-id="d8adc-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8adc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





