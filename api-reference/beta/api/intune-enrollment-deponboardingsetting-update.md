---
title: Обновление depOnboardingSetting
description: Обновление свойства объекта depOnboardingSetting.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 78d3138950776dd74a055fbb00339e9e69b5f0f1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412291"
---
# <a name="update-deponboardingsetting"></a><span data-ttu-id="11379-103">Обновление depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="11379-103">Update depOnboardingSetting</span></span>

> <span data-ttu-id="11379-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="11379-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="11379-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11379-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11379-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11379-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11379-107">Обновление свойства объекта [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="11379-107">Update the properties of a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11379-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="11379-108">Prerequisites</span></span>
<span data-ttu-id="11379-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="11379-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="11379-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11379-111">Permission type</span></span>|<span data-ttu-id="11379-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="11379-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11379-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11379-113">Delegated (work or school account)</span></span>|<span data-ttu-id="11379-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11379-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="11379-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11379-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11379-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11379-116">Not supported.</span></span>|
|<span data-ttu-id="11379-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11379-117">Application</span></span>|<span data-ttu-id="11379-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11379-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11379-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11379-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
```

## <a name="request-headers"></a><span data-ttu-id="11379-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11379-120">Request headers</span></span>
|<span data-ttu-id="11379-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="11379-121">Header</span></span>|<span data-ttu-id="11379-122">Значение</span><span class="sxs-lookup"><span data-stu-id="11379-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11379-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="11379-123">Authorization</span></span>|<span data-ttu-id="11379-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="11379-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11379-125">Accept</span><span class="sxs-lookup"><span data-stu-id="11379-125">Accept</span></span>|<span data-ttu-id="11379-126">application/json</span><span class="sxs-lookup"><span data-stu-id="11379-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11379-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11379-127">Request body</span></span>
<span data-ttu-id="11379-128">В тексте запроса укажите представление JSON для объекта [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="11379-128">In the request body, supply a JSON representation for the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>

<span data-ttu-id="11379-129">В следующей таблице показаны свойства, которые необходимы для создания [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).</span><span class="sxs-lookup"><span data-stu-id="11379-129">The following table shows the properties that are required when you create the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).</span></span>

|<span data-ttu-id="11379-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="11379-130">Property</span></span>|<span data-ttu-id="11379-131">Тип</span><span class="sxs-lookup"><span data-stu-id="11379-131">Type</span></span>|<span data-ttu-id="11379-132">Описание</span><span class="sxs-lookup"><span data-stu-id="11379-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11379-133">id</span><span class="sxs-lookup"><span data-stu-id="11379-133">id</span></span>|<span data-ttu-id="11379-134">String</span><span class="sxs-lookup"><span data-stu-id="11379-134">String</span></span>|<span data-ttu-id="11379-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="11379-135">UUID for the object</span></span>|
|<span data-ttu-id="11379-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="11379-136">appleIdentifier</span></span>|<span data-ttu-id="11379-137">String</span><span class="sxs-lookup"><span data-stu-id="11379-137">String</span></span>|<span data-ttu-id="11379-138">Apple идентификатор, используемый для получения текущего маркера.</span><span class="sxs-lookup"><span data-stu-id="11379-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="11379-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="11379-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="11379-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11379-140">DateTimeOffset</span></span>|<span data-ttu-id="11379-141">Маркер истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="11379-141">When the token will expire.</span></span>|
|<span data-ttu-id="11379-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11379-142">lastModifiedDateTime</span></span>|<span data-ttu-id="11379-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11379-143">DateTimeOffset</span></span>|<span data-ttu-id="11379-144">Когда служба была onboarded.</span><span class="sxs-lookup"><span data-stu-id="11379-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="11379-145">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="11379-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="11379-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11379-146">DateTimeOffset</span></span>|<span data-ttu-id="11379-147">При последней syned службы с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="11379-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="11379-148">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="11379-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="11379-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11379-149">DateTimeOffset</span></span>|<span data-ttu-id="11379-150">Когда Intune запрашивает последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="11379-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="11379-151">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="11379-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="11379-152">Логический</span><span class="sxs-lookup"><span data-stu-id="11379-152">Boolean</span></span>|<span data-ttu-id="11379-153">Ли Dep маркеров общий доступ к включается со службой синхронизации данных School.</span><span class="sxs-lookup"><span data-stu-id="11379-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="11379-154">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="11379-154">lastSyncErrorCode</span></span>|<span data-ttu-id="11379-155">Int32</span><span class="sxs-lookup"><span data-stu-id="11379-155">Int32</span></span>|<span data-ttu-id="11379-156">Код ошибки Apple во время последней синхронизации dep.</span><span class="sxs-lookup"><span data-stu-id="11379-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="11379-157">tokenType</span><span class="sxs-lookup"><span data-stu-id="11379-157">tokenType</span></span>|<span data-ttu-id="11379-158">[depTokenType](../resources/intune-enrollment-deptokentype.md);</span><span class="sxs-lookup"><span data-stu-id="11379-158">[depTokenType](../resources/intune-enrollment-deptokentype.md)</span></span>|<span data-ttu-id="11379-159">Получает или задает тип токена Dep.</span><span class="sxs-lookup"><span data-stu-id="11379-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="11379-160">Возможные значения: `none`, `dep`, `appleSchoolManager`.</span><span class="sxs-lookup"><span data-stu-id="11379-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="11379-161">tokenName</span><span class="sxs-lookup"><span data-stu-id="11379-161">tokenName</span></span>|<span data-ttu-id="11379-162">String</span><span class="sxs-lookup"><span data-stu-id="11379-162">String</span></span>|<span data-ttu-id="11379-163">Понятное имя для маркера Dep</span><span class="sxs-lookup"><span data-stu-id="11379-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="11379-164">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="11379-164">syncedDeviceCount</span></span>|<span data-ttu-id="11379-165">Int32</span><span class="sxs-lookup"><span data-stu-id="11379-165">Int32</span></span>|<span data-ttu-id="11379-166">Получает количество синхронизированных устройства</span><span class="sxs-lookup"><span data-stu-id="11379-166">Gets synced device count</span></span>|
|<span data-ttu-id="11379-167">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="11379-167">dataSharingConsentGranted</span></span>|<span data-ttu-id="11379-168">Логический</span><span class="sxs-lookup"><span data-stu-id="11379-168">Boolean</span></span>|<span data-ttu-id="11379-169">Предоставляются разрешения для данных, общий доступ к службе Dep Apple</span><span class="sxs-lookup"><span data-stu-id="11379-169">Consent granted for data sharing with Apple Dep Service</span></span>|



## <a name="response"></a><span data-ttu-id="11379-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="11379-170">Response</span></span>
<span data-ttu-id="11379-171">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="11379-171">If successful, this method returns a `200 OK` response code and an updated [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11379-172">Пример</span><span class="sxs-lookup"><span data-stu-id="11379-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="11379-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="11379-173">Request</span></span>
<span data-ttu-id="11379-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11379-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}
Content-type: application/json
Content-length: 514

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
  "dataSharingConsentGranted": true
}
```

### <a name="response"></a><span data-ttu-id="11379-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="11379-175">Response</span></span>
<span data-ttu-id="11379-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="11379-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 627

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
  "dataSharingConsentGranted": true
}
```




