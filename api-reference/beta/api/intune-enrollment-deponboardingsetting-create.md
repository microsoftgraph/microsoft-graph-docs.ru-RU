---
title: Создание depOnboardingSetting
description: Создание нового объекта depOnboardingSetting.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 71d942195ff6f55a8455fe8b5f687ebe45053c51
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34980238"
---
# <a name="create-deponboardingsetting"></a><span data-ttu-id="5b4b2-103">Создание depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="5b4b2-103">Create depOnboardingSetting</span></span>

> <span data-ttu-id="5b4b2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b4b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b4b2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b4b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b4b2-106">Создание нового объекта [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="5b4b2-106">Create a new [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b4b2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5b4b2-107">Prerequisites</span></span>
<span data-ttu-id="5b4b2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b4b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b4b2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b4b2-110">Permission type</span></span>|<span data-ttu-id="5b4b2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b4b2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b4b2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b4b2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b4b2-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b4b2-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5b4b2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b4b2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b4b2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b4b2-115">Not supported.</span></span>|
|<span data-ttu-id="5b4b2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b4b2-116">Application</span></span>|<span data-ttu-id="5b4b2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b4b2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b4b2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b4b2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="5b4b2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b4b2-119">Request headers</span></span>
|<span data-ttu-id="5b4b2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b4b2-120">Header</span></span>|<span data-ttu-id="5b4b2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5b4b2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b4b2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b4b2-122">Authorization</span></span>|<span data-ttu-id="5b4b2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b4b2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b4b2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5b4b2-124">Accept</span></span>|<span data-ttu-id="5b4b2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5b4b2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b4b2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5b4b2-126">Request body</span></span>
<span data-ttu-id="5b4b2-127">В тексте запроса добавьте представление объекта depOnboardingSetting в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b4b2-127">In the request body, supply a JSON representation for the depOnboardingSetting object.</span></span>

<span data-ttu-id="5b4b2-128">В следующей таблице приведены свойства, необходимые при создании depOnboardingSetting.</span><span class="sxs-lookup"><span data-stu-id="5b4b2-128">The following table shows the properties that are required when you create the depOnboardingSetting.</span></span>

|<span data-ttu-id="5b4b2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b4b2-129">Property</span></span>|<span data-ttu-id="5b4b2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5b4b2-130">Type</span></span>|<span data-ttu-id="5b4b2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5b4b2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b4b2-132">id</span><span class="sxs-lookup"><span data-stu-id="5b4b2-132">id</span></span>|<span data-ttu-id="5b4b2-133">String</span><span class="sxs-lookup"><span data-stu-id="5b4b2-133">String</span></span>|<span data-ttu-id="5b4b2-134">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="5b4b2-134">UUID for the object</span></span>|
|<span data-ttu-id="5b4b2-135">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="5b4b2-135">appleIdentifier</span></span>|<span data-ttu-id="5b4b2-136">String</span><span class="sxs-lookup"><span data-stu-id="5b4b2-136">String</span></span>|<span data-ttu-id="5b4b2-137">Идентификатор Apple ID, используемый для получения текущего маркера.</span><span class="sxs-lookup"><span data-stu-id="5b4b2-137">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="5b4b2-138">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5b4b2-138">tokenExpirationDateTime</span></span>|<span data-ttu-id="5b4b2-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b4b2-139">DateTimeOffset</span></span>|<span data-ttu-id="5b4b2-140">По истечении срока действия маркера.</span><span class="sxs-lookup"><span data-stu-id="5b4b2-140">When the token will expire.</span></span>|
|<span data-ttu-id="5b4b2-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b4b2-141">lastModifiedDateTime</span></span>|<span data-ttu-id="5b4b2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b4b2-142">DateTimeOffset</span></span>|<span data-ttu-id="5b4b2-143">При подключении службы.</span><span class="sxs-lookup"><span data-stu-id="5b4b2-143">When the service was onboarded.</span></span>|
|<span data-ttu-id="5b4b2-144">Ластсукцессфулсинкдатетиме</span><span class="sxs-lookup"><span data-stu-id="5b4b2-144">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="5b4b2-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b4b2-145">DateTimeOffset</span></span>|<span data-ttu-id="5b4b2-146">Когда служба последний синед с Intune</span><span class="sxs-lookup"><span data-stu-id="5b4b2-146">When the service last syned with Intune</span></span>|
|<span data-ttu-id="5b4b2-147">Ластсинктригжереддатетиме</span><span class="sxs-lookup"><span data-stu-id="5b4b2-147">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="5b4b2-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b4b2-148">DateTimeOffset</span></span>|<span data-ttu-id="5b4b2-149">При последнем запросе синхронизации в Intune.</span><span class="sxs-lookup"><span data-stu-id="5b4b2-149">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="5b4b2-150">Свойства sharetokenwithschooldatasyncservice</span><span class="sxs-lookup"><span data-stu-id="5b4b2-150">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="5b4b2-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b4b2-151">Boolean</span></span>|<span data-ttu-id="5b4b2-152">Указывает, включен ли общий доступ к маркеру DEP для службы School Data Sync.</span><span class="sxs-lookup"><span data-stu-id="5b4b2-152">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="5b4b2-153">Lastsyncerrorcode к объекту</span><span class="sxs-lookup"><span data-stu-id="5b4b2-153">lastSyncErrorCode</span></span>|<span data-ttu-id="5b4b2-154">Int32</span><span class="sxs-lookup"><span data-stu-id="5b4b2-154">Int32</span></span>|<span data-ttu-id="5b4b2-155">Код ошибки, полученный от Apple во время последней синхронизации DEP.</span><span class="sxs-lookup"><span data-stu-id="5b4b2-155">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="5b4b2-156">Токентипе</span><span class="sxs-lookup"><span data-stu-id="5b4b2-156">tokenType</span></span>|<span data-ttu-id="5b4b2-157">[depTokenType](../resources/intune-enrollment-deptokentype.md);</span><span class="sxs-lookup"><span data-stu-id="5b4b2-157">[depTokenType](../resources/intune-enrollment-deptokentype.md)</span></span>|<span data-ttu-id="5b4b2-158">Получает или задает тип токена DEP.</span><span class="sxs-lookup"><span data-stu-id="5b4b2-158">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="5b4b2-159">Возможные значения: `none`, `dep`, `appleSchoolManager`.</span><span class="sxs-lookup"><span data-stu-id="5b4b2-159">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="5b4b2-160">Токеннаме</span><span class="sxs-lookup"><span data-stu-id="5b4b2-160">tokenName</span></span>|<span data-ttu-id="5b4b2-161">String</span><span class="sxs-lookup"><span data-stu-id="5b4b2-161">String</span></span>|<span data-ttu-id="5b4b2-162">Понятное имя для токена DEP</span><span class="sxs-lookup"><span data-stu-id="5b4b2-162">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="5b4b2-163">Синцеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="5b4b2-163">syncedDeviceCount</span></span>|<span data-ttu-id="5b4b2-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5b4b2-164">Int32</span></span>|<span data-ttu-id="5b4b2-165">Получает число синхронизированных устройств</span><span class="sxs-lookup"><span data-stu-id="5b4b2-165">Gets synced device count</span></span>|
|<span data-ttu-id="5b4b2-166">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="5b4b2-166">dataSharingConsentGranted</span></span>|<span data-ttu-id="5b4b2-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b4b2-167">Boolean</span></span>|<span data-ttu-id="5b4b2-168">Разрешение, предоставленное для предоставления общего доступа к данным с помощью службы Apple DEP</span><span class="sxs-lookup"><span data-stu-id="5b4b2-168">Consent granted for data sharing with Apple Dep Service</span></span>|
|<span data-ttu-id="5b4b2-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5b4b2-169">roleScopeTagIds</span></span>|<span data-ttu-id="5b4b2-170">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5b4b2-170">String collection</span></span>|<span data-ttu-id="5b4b2-171">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5b4b2-171">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="5b4b2-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b4b2-172">Response</span></span>
<span data-ttu-id="5b4b2-173">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b4b2-173">If successful, this method returns a `201 Created` response code and a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b4b2-174">Пример</span><span class="sxs-lookup"><span data-stu-id="5b4b2-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b4b2-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b4b2-175">Request</span></span>
<span data-ttu-id="5b4b2-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b4b2-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5b4b2-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b4b2-177">Response</span></span>
<span data-ttu-id="5b4b2-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b4b2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





