---
title: Создание depOnboardingSetting
description: Создайте новый объект depOnboardingSetting.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e4417c01a435ceb8392eff280992877ebdeb79e4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135735"
---
# <a name="create-deponboardingsetting"></a><span data-ttu-id="2519c-103">Создание depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="2519c-103">Create depOnboardingSetting</span></span>

<span data-ttu-id="2519c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2519c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2519c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2519c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2519c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2519c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2519c-107">Создайте [новый объект depOnboardingSetting.](../resources/intune-enrollment-deponboardingsetting.md)</span><span class="sxs-lookup"><span data-stu-id="2519c-107">Create a new [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2519c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2519c-108">Prerequisites</span></span>
<span data-ttu-id="2519c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2519c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2519c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2519c-111">Permission type</span></span>|<span data-ttu-id="2519c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2519c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2519c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2519c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2519c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2519c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2519c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2519c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2519c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2519c-116">Not supported.</span></span>|
|<span data-ttu-id="2519c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2519c-117">Application</span></span>|<span data-ttu-id="2519c-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2519c-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2519c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2519c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="2519c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2519c-120">Request headers</span></span>
|<span data-ttu-id="2519c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2519c-121">Header</span></span>|<span data-ttu-id="2519c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2519c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2519c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2519c-123">Authorization</span></span>|<span data-ttu-id="2519c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2519c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2519c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2519c-125">Accept</span></span>|<span data-ttu-id="2519c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2519c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2519c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2519c-127">Request body</span></span>
<span data-ttu-id="2519c-128">В теле запроса поставляем представление JSON для объекта depOnboardingSetting.</span><span class="sxs-lookup"><span data-stu-id="2519c-128">In the request body, supply a JSON representation for the depOnboardingSetting object.</span></span>

<span data-ttu-id="2519c-129">В следующей таблице показаны свойства, необходимые при создании depOnboardingSetting.</span><span class="sxs-lookup"><span data-stu-id="2519c-129">The following table shows the properties that are required when you create the depOnboardingSetting.</span></span>

|<span data-ttu-id="2519c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2519c-130">Property</span></span>|<span data-ttu-id="2519c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2519c-131">Type</span></span>|<span data-ttu-id="2519c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2519c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2519c-133">id</span><span class="sxs-lookup"><span data-stu-id="2519c-133">id</span></span>|<span data-ttu-id="2519c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2519c-134">String</span></span>|<span data-ttu-id="2519c-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="2519c-135">UUID for the object</span></span>|
|<span data-ttu-id="2519c-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="2519c-136">appleIdentifier</span></span>|<span data-ttu-id="2519c-137">String</span><span class="sxs-lookup"><span data-stu-id="2519c-137">String</span></span>|<span data-ttu-id="2519c-138">ID Apple, используемый для получения текущего маркера.</span><span class="sxs-lookup"><span data-stu-id="2519c-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="2519c-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2519c-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="2519c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2519c-140">DateTimeOffset</span></span>|<span data-ttu-id="2519c-141">По истечении срока действия маркера.</span><span class="sxs-lookup"><span data-stu-id="2519c-141">When the token will expire.</span></span>|
|<span data-ttu-id="2519c-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2519c-142">lastModifiedDateTime</span></span>|<span data-ttu-id="2519c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2519c-143">DateTimeOffset</span></span>|<span data-ttu-id="2519c-144">Когда служба была на борту.</span><span class="sxs-lookup"><span data-stu-id="2519c-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="2519c-145">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2519c-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="2519c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2519c-146">DateTimeOffset</span></span>|<span data-ttu-id="2519c-147">Когда служба последний раз синхронизирована с Intune</span><span class="sxs-lookup"><span data-stu-id="2519c-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="2519c-148">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="2519c-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="2519c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2519c-149">DateTimeOffset</span></span>|<span data-ttu-id="2519c-150">Когда Intune в последний раз запрашивала синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="2519c-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="2519c-151">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="2519c-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="2519c-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="2519c-152">Boolean</span></span>|<span data-ttu-id="2519c-153">Включено ли совместное использование маркеров Dep с помощью службы синхронизации данных школы.</span><span class="sxs-lookup"><span data-stu-id="2519c-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="2519c-154">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="2519c-154">lastSyncErrorCode</span></span>|<span data-ttu-id="2519c-155">Int32</span><span class="sxs-lookup"><span data-stu-id="2519c-155">Int32</span></span>|<span data-ttu-id="2519c-156">Код ошибки, сообщаемой Apple во время последней синхронизации dep.</span><span class="sxs-lookup"><span data-stu-id="2519c-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="2519c-157">tokenType</span><span class="sxs-lookup"><span data-stu-id="2519c-157">tokenType</span></span>|<span data-ttu-id="2519c-158">[depTokenType](../resources/intune-enrollment-deptokentype.md);</span><span class="sxs-lookup"><span data-stu-id="2519c-158">[depTokenType](../resources/intune-enrollment-deptokentype.md)</span></span>|<span data-ttu-id="2519c-159">Получает или задает тип маркера Dep.</span><span class="sxs-lookup"><span data-stu-id="2519c-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="2519c-160">Возможные значения: `none`, `dep`, `appleSchoolManager`.</span><span class="sxs-lookup"><span data-stu-id="2519c-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="2519c-161">tokenName</span><span class="sxs-lookup"><span data-stu-id="2519c-161">tokenName</span></span>|<span data-ttu-id="2519c-162">Строка</span><span class="sxs-lookup"><span data-stu-id="2519c-162">String</span></span>|<span data-ttu-id="2519c-163">Friendly Name for Dep Token</span><span class="sxs-lookup"><span data-stu-id="2519c-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="2519c-164">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2519c-164">syncedDeviceCount</span></span>|<span data-ttu-id="2519c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2519c-165">Int32</span></span>|<span data-ttu-id="2519c-166">Получает синхронизированное количество устройств</span><span class="sxs-lookup"><span data-stu-id="2519c-166">Gets synced device count</span></span>|
|<span data-ttu-id="2519c-167">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="2519c-167">dataSharingConsentGranted</span></span>|<span data-ttu-id="2519c-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="2519c-168">Boolean</span></span>|<span data-ttu-id="2519c-169">Согласие, предоставленное для обмена данными с службой Apple Dep</span><span class="sxs-lookup"><span data-stu-id="2519c-169">Consent granted for data sharing with Apple Dep Service</span></span>|
|<span data-ttu-id="2519c-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2519c-170">roleScopeTagIds</span></span>|<span data-ttu-id="2519c-171">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2519c-171">String collection</span></span>|<span data-ttu-id="2519c-172">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="2519c-172">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="2519c-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="2519c-173">Response</span></span>
<span data-ttu-id="2519c-174">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2519c-174">If successful, this method returns a `201 Created` response code and a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2519c-175">Пример</span><span class="sxs-lookup"><span data-stu-id="2519c-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="2519c-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="2519c-176">Request</span></span>
<span data-ttu-id="2519c-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2519c-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2519c-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="2519c-178">Response</span></span>
<span data-ttu-id="2519c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2519c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




