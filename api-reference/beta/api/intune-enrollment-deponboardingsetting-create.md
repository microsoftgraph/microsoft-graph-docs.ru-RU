---
title: Создание depOnboardingSetting
description: Создание нового объекта depOnboardingSetting.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 89e46c715b5f888ae3c9f1fb02a0566da8485944
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854903"
---
# <a name="create-deponboardingsetting"></a><span data-ttu-id="969d0-103">Создание depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="969d0-103">Create depOnboardingSetting</span></span>

> <span data-ttu-id="969d0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="969d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="969d0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="969d0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="969d0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="969d0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="969d0-107">Создание нового объекта [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="969d0-107">Create a new [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="969d0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="969d0-108">Prerequisites</span></span>
<span data-ttu-id="969d0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="969d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="969d0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="969d0-111">Permission type</span></span>|<span data-ttu-id="969d0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="969d0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="969d0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="969d0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="969d0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="969d0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="969d0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="969d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="969d0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="969d0-116">Not supported.</span></span>|
|<span data-ttu-id="969d0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="969d0-117">Application</span></span>|<span data-ttu-id="969d0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="969d0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="969d0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="969d0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="969d0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="969d0-120">Request headers</span></span>
|<span data-ttu-id="969d0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="969d0-121">Header</span></span>|<span data-ttu-id="969d0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="969d0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="969d0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="969d0-123">Authorization</span></span>|<span data-ttu-id="969d0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="969d0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="969d0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="969d0-125">Accept</span></span>|<span data-ttu-id="969d0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="969d0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="969d0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="969d0-127">Request body</span></span>
<span data-ttu-id="969d0-128">В тексте запроса укажите представление JSON для объекта depOnboardingSetting.</span><span class="sxs-lookup"><span data-stu-id="969d0-128">In the request body, supply a JSON representation for the depOnboardingSetting object.</span></span>

<span data-ttu-id="969d0-129">В следующей таблице показаны свойства, которые необходимы для создания depOnboardingSetting.</span><span class="sxs-lookup"><span data-stu-id="969d0-129">The following table shows the properties that are required when you create the depOnboardingSetting.</span></span>

|<span data-ttu-id="969d0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="969d0-130">Property</span></span>|<span data-ttu-id="969d0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="969d0-131">Type</span></span>|<span data-ttu-id="969d0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="969d0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="969d0-133">id</span><span class="sxs-lookup"><span data-stu-id="969d0-133">id</span></span>|<span data-ttu-id="969d0-134">String</span><span class="sxs-lookup"><span data-stu-id="969d0-134">String</span></span>|<span data-ttu-id="969d0-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="969d0-135">UUID for the object</span></span>|
|<span data-ttu-id="969d0-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="969d0-136">appleIdentifier</span></span>|<span data-ttu-id="969d0-137">String</span><span class="sxs-lookup"><span data-stu-id="969d0-137">String</span></span>|<span data-ttu-id="969d0-138">Apple идентификатор, используемый для получения текущего маркера.</span><span class="sxs-lookup"><span data-stu-id="969d0-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="969d0-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="969d0-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="969d0-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="969d0-140">DateTimeOffset</span></span>|<span data-ttu-id="969d0-141">Маркер истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="969d0-141">When the token will expire.</span></span>|
|<span data-ttu-id="969d0-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="969d0-142">lastModifiedDateTime</span></span>|<span data-ttu-id="969d0-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="969d0-143">DateTimeOffset</span></span>|<span data-ttu-id="969d0-144">Когда служба была onboarded.</span><span class="sxs-lookup"><span data-stu-id="969d0-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="969d0-145">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="969d0-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="969d0-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="969d0-146">DateTimeOffset</span></span>|<span data-ttu-id="969d0-147">При последней syned службы с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="969d0-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="969d0-148">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="969d0-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="969d0-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="969d0-149">DateTimeOffset</span></span>|<span data-ttu-id="969d0-150">Когда Intune запрашивает последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="969d0-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="969d0-151">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="969d0-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="969d0-152">Логический</span><span class="sxs-lookup"><span data-stu-id="969d0-152">Boolean</span></span>|<span data-ttu-id="969d0-153">Ли Dep маркеров общий доступ к включается со службой синхронизации данных School.</span><span class="sxs-lookup"><span data-stu-id="969d0-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="969d0-154">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="969d0-154">lastSyncErrorCode</span></span>|<span data-ttu-id="969d0-155">Int32</span><span class="sxs-lookup"><span data-stu-id="969d0-155">Int32</span></span>|<span data-ttu-id="969d0-156">Код ошибки Apple во время последней синхронизации dep.</span><span class="sxs-lookup"><span data-stu-id="969d0-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="969d0-157">tokenType</span><span class="sxs-lookup"><span data-stu-id="969d0-157">tokenType</span></span>|<span data-ttu-id="969d0-158">[depTokenType](../resources/intune-enrollment-deptokentype.md);</span><span class="sxs-lookup"><span data-stu-id="969d0-158">[depTokenType](../resources/intune-enrollment-deptokentype.md)</span></span>|<span data-ttu-id="969d0-159">Получает или задает тип токена Dep.</span><span class="sxs-lookup"><span data-stu-id="969d0-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="969d0-160">Возможные значения: `none`, `dep`, `appleSchoolManager`.</span><span class="sxs-lookup"><span data-stu-id="969d0-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="969d0-161">tokenName</span><span class="sxs-lookup"><span data-stu-id="969d0-161">tokenName</span></span>|<span data-ttu-id="969d0-162">Строка</span><span class="sxs-lookup"><span data-stu-id="969d0-162">String</span></span>|<span data-ttu-id="969d0-163">Понятное имя для маркера Dep</span><span class="sxs-lookup"><span data-stu-id="969d0-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="969d0-164">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="969d0-164">syncedDeviceCount</span></span>|<span data-ttu-id="969d0-165">Int32</span><span class="sxs-lookup"><span data-stu-id="969d0-165">Int32</span></span>|<span data-ttu-id="969d0-166">Получает количество синхронизированных устройства</span><span class="sxs-lookup"><span data-stu-id="969d0-166">Gets synced device count</span></span>|
|<span data-ttu-id="969d0-167">defaultProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="969d0-167">defaultProfileDisplayName</span></span>|<span data-ttu-id="969d0-168">Строка</span><span class="sxs-lookup"><span data-stu-id="969d0-168">String</span></span>|<span data-ttu-id="969d0-169">Получает количество синхронизированных устройства</span><span class="sxs-lookup"><span data-stu-id="969d0-169">Gets synced device count</span></span>|
|<span data-ttu-id="969d0-170">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="969d0-170">dataSharingConsentGranted</span></span>|<span data-ttu-id="969d0-171">Логический</span><span class="sxs-lookup"><span data-stu-id="969d0-171">Boolean</span></span>|<span data-ttu-id="969d0-172">Предоставляются разрешения для данных, общий доступ к службе Dep Apple</span><span class="sxs-lookup"><span data-stu-id="969d0-172">Consent granted for data sharing with Apple Dep Service</span></span>|



## <a name="response"></a><span data-ttu-id="969d0-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="969d0-173">Response</span></span>
<span data-ttu-id="969d0-174">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="969d0-174">If successful, this method returns a `201 Created` response code and a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="969d0-175">Пример</span><span class="sxs-lookup"><span data-stu-id="969d0-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="969d0-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="969d0-176">Request</span></span>
<span data-ttu-id="969d0-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="969d0-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
Content-type: application/json
Content-length: 648

{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
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
  "defaultProfileDisplayName": "Default Profile Display Name value",
  "dataSharingConsentGranted": true
}
```

### <a name="response"></a><span data-ttu-id="969d0-178">Ответ</span><span class="sxs-lookup"><span data-stu-id="969d0-178">Response</span></span>
<span data-ttu-id="969d0-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="969d0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 697

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
  "defaultProfileDisplayName": "Default Profile Display Name value",
  "dataSharingConsentGranted": true
}
```





