---
title: Создание depOnboardingSetting
description: Создание нового объекта depOnboardingSetting.
author: tfitzmac
ms.openlocfilehash: 11f2e5217e4040a7d4345c9271b459e608075498
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330662"
---
# <a name="create-deponboardingsetting"></a><span data-ttu-id="81480-103">Создание depOnboardingSetting</span><span class="sxs-lookup"><span data-stu-id="81480-103">Create depOnboardingSetting</span></span>

> <span data-ttu-id="81480-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="81480-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81480-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81480-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81480-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="81480-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81480-107">Создание нового объекта [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .</span><span class="sxs-lookup"><span data-stu-id="81480-107">Create a new [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="81480-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="81480-108">Prerequisites</span></span>
<span data-ttu-id="81480-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81480-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81480-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81480-111">Permission type</span></span>|<span data-ttu-id="81480-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="81480-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81480-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81480-113">Delegated (work or school account)</span></span>|<span data-ttu-id="81480-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81480-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="81480-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81480-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81480-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81480-116">Not supported.</span></span>|
|<span data-ttu-id="81480-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81480-117">Application</span></span>|<span data-ttu-id="81480-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81480-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81480-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81480-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="81480-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81480-120">Request headers</span></span>
|<span data-ttu-id="81480-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="81480-121">Header</span></span>|<span data-ttu-id="81480-122">Значение</span><span class="sxs-lookup"><span data-stu-id="81480-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81480-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81480-123">Authorization</span></span>|<span data-ttu-id="81480-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="81480-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81480-125">Accept</span><span class="sxs-lookup"><span data-stu-id="81480-125">Accept</span></span>|<span data-ttu-id="81480-126">application/json</span><span class="sxs-lookup"><span data-stu-id="81480-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81480-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81480-127">Request body</span></span>
<span data-ttu-id="81480-128">В тексте запроса укажите представление JSON для объекта depOnboardingSetting.</span><span class="sxs-lookup"><span data-stu-id="81480-128">In the request body, supply a JSON representation for the depOnboardingSetting object.</span></span>

<span data-ttu-id="81480-129">В следующей таблице показаны свойства, которые необходимы для создания depOnboardingSetting.</span><span class="sxs-lookup"><span data-stu-id="81480-129">The following table shows the properties that are required when you create the depOnboardingSetting.</span></span>

|<span data-ttu-id="81480-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="81480-130">Property</span></span>|<span data-ttu-id="81480-131">Тип</span><span class="sxs-lookup"><span data-stu-id="81480-131">Type</span></span>|<span data-ttu-id="81480-132">Описание</span><span class="sxs-lookup"><span data-stu-id="81480-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81480-133">id</span><span class="sxs-lookup"><span data-stu-id="81480-133">id</span></span>|<span data-ttu-id="81480-134">String</span><span class="sxs-lookup"><span data-stu-id="81480-134">String</span></span>|<span data-ttu-id="81480-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="81480-135">UUID for the object</span></span>|
|<span data-ttu-id="81480-136">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="81480-136">appleIdentifier</span></span>|<span data-ttu-id="81480-137">String</span><span class="sxs-lookup"><span data-stu-id="81480-137">String</span></span>|<span data-ttu-id="81480-138">Apple идентификатор, используемый для получения текущего маркера.</span><span class="sxs-lookup"><span data-stu-id="81480-138">The Apple ID used to obtain the current token.</span></span>|
|<span data-ttu-id="81480-139">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="81480-139">tokenExpirationDateTime</span></span>|<span data-ttu-id="81480-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81480-140">DateTimeOffset</span></span>|<span data-ttu-id="81480-141">Маркер истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="81480-141">When the token will expire.</span></span>|
|<span data-ttu-id="81480-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81480-142">lastModifiedDateTime</span></span>|<span data-ttu-id="81480-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81480-143">DateTimeOffset</span></span>|<span data-ttu-id="81480-144">Когда служба была onboarded.</span><span class="sxs-lookup"><span data-stu-id="81480-144">When the service was onboarded.</span></span>|
|<span data-ttu-id="81480-145">lastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="81480-145">lastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="81480-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81480-146">DateTimeOffset</span></span>|<span data-ttu-id="81480-147">При последней syned службы с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="81480-147">When the service last syned with Intune</span></span>|
|<span data-ttu-id="81480-148">lastSyncTriggeredDateTime</span><span class="sxs-lookup"><span data-stu-id="81480-148">lastSyncTriggeredDateTime</span></span>|<span data-ttu-id="81480-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81480-149">DateTimeOffset</span></span>|<span data-ttu-id="81480-150">Когда Intune запрашивает последней синхронизации.</span><span class="sxs-lookup"><span data-stu-id="81480-150">When Intune last requested a sync.</span></span>|
|<span data-ttu-id="81480-151">shareTokenWithSchoolDataSyncService</span><span class="sxs-lookup"><span data-stu-id="81480-151">shareTokenWithSchoolDataSyncService</span></span>|<span data-ttu-id="81480-152">Boolean.</span><span class="sxs-lookup"><span data-stu-id="81480-152">Boolean</span></span>|<span data-ttu-id="81480-153">Ли Dep маркеров общий доступ к включается со службой синхронизации данных School.</span><span class="sxs-lookup"><span data-stu-id="81480-153">Whether or not the Dep token sharing is enabled with the School Data Sync service.</span></span>|
|<span data-ttu-id="81480-154">lastSyncErrorCode</span><span class="sxs-lookup"><span data-stu-id="81480-154">lastSyncErrorCode</span></span>|<span data-ttu-id="81480-155">Int32</span><span class="sxs-lookup"><span data-stu-id="81480-155">Int32</span></span>|<span data-ttu-id="81480-156">Код ошибки Apple во время последней синхронизации dep.</span><span class="sxs-lookup"><span data-stu-id="81480-156">Error code reported by Apple during last dep sync.</span></span>|
|<span data-ttu-id="81480-157">tokenType</span><span class="sxs-lookup"><span data-stu-id="81480-157">tokenType</span></span>|<span data-ttu-id="81480-158">[depTokenType](../resources/intune-enrollment-deptokentype.md);</span><span class="sxs-lookup"><span data-stu-id="81480-158">[depTokenType](../resources/intune-enrollment-deptokentype.md)</span></span>|<span data-ttu-id="81480-159">Получает или задает тип токена Dep.</span><span class="sxs-lookup"><span data-stu-id="81480-159">Gets or sets the Dep Token Type.</span></span> <span data-ttu-id="81480-160">Возможные значения: `none`, `dep`, `appleSchoolManager`.</span><span class="sxs-lookup"><span data-stu-id="81480-160">Possible values are: `none`, `dep`, `appleSchoolManager`.</span></span>|
|<span data-ttu-id="81480-161">tokenName</span><span class="sxs-lookup"><span data-stu-id="81480-161">tokenName</span></span>|<span data-ttu-id="81480-162">String.</span><span class="sxs-lookup"><span data-stu-id="81480-162">String</span></span>|<span data-ttu-id="81480-163">Понятное имя для маркера Dep</span><span class="sxs-lookup"><span data-stu-id="81480-163">Friendly Name for Dep Token</span></span>|
|<span data-ttu-id="81480-164">syncedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="81480-164">syncedDeviceCount</span></span>|<span data-ttu-id="81480-165">Int32</span><span class="sxs-lookup"><span data-stu-id="81480-165">Int32</span></span>|<span data-ttu-id="81480-166">Получает количество синхронизированных устройства</span><span class="sxs-lookup"><span data-stu-id="81480-166">Gets synced device count</span></span>|
|<span data-ttu-id="81480-167">defaultProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="81480-167">defaultProfileDisplayName</span></span>|<span data-ttu-id="81480-168">String.</span><span class="sxs-lookup"><span data-stu-id="81480-168">String</span></span>|<span data-ttu-id="81480-169">Получает количество синхронизированных устройства</span><span class="sxs-lookup"><span data-stu-id="81480-169">Gets synced device count</span></span>|
|<span data-ttu-id="81480-170">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="81480-170">dataSharingConsentGranted</span></span>|<span data-ttu-id="81480-171">Boolean.</span><span class="sxs-lookup"><span data-stu-id="81480-171">Boolean</span></span>|<span data-ttu-id="81480-172">Предоставляются разрешения для данных, общий доступ к службе Dep Apple</span><span class="sxs-lookup"><span data-stu-id="81480-172">Consent granted for data sharing with Apple Dep Service</span></span>|



## <a name="response"></a><span data-ttu-id="81480-173">Ответ</span><span class="sxs-lookup"><span data-stu-id="81480-173">Response</span></span>
<span data-ttu-id="81480-174">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="81480-174">If successful, this method returns a `201 Created` response code and a [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81480-175">Пример</span><span class="sxs-lookup"><span data-stu-id="81480-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="81480-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="81480-176">Request</span></span>
<span data-ttu-id="81480-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81480-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="81480-178">Ответ</span><span class="sxs-lookup"><span data-stu-id="81480-178">Response</span></span>
<span data-ttu-id="81480-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="81480-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





