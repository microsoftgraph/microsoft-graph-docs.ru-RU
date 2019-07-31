---
title: Обновление ресурса androidmanagedstoreaccountenterprisesettings
description: Обновление свойств объекта ресурса androidmanagedstoreaccountenterprisesettings.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 698bb3b11f9df052213257f2c882b7a207cb0bcf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35952550"
---
# <a name="update-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="fb839-103">Обновление ресурса androidmanagedstoreaccountenterprisesettings</span><span class="sxs-lookup"><span data-stu-id="fb839-103">Update androidManagedStoreAccountEnterpriseSettings</span></span>

> <span data-ttu-id="fb839-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb839-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb839-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb839-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb839-106">Обновление свойств объекта [ресурса androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="fb839-106">Update the properties of a [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb839-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fb839-107">Prerequisites</span></span>
<span data-ttu-id="fb839-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb839-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb839-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb839-110">Permission type</span></span>|<span data-ttu-id="fb839-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb839-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb839-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb839-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fb839-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb839-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fb839-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb839-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb839-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb839-115">Not supported.</span></span>|
|<span data-ttu-id="fb839-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb839-116">Application</span></span>|<span data-ttu-id="fb839-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb839-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb839-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb839-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="request-headers"></a><span data-ttu-id="fb839-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb839-119">Request headers</span></span>
|<span data-ttu-id="fb839-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb839-120">Header</span></span>|<span data-ttu-id="fb839-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fb839-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb839-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb839-122">Authorization</span></span>|<span data-ttu-id="fb839-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb839-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb839-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fb839-124">Accept</span></span>|<span data-ttu-id="fb839-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fb839-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb839-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fb839-126">Request body</span></span>
<span data-ttu-id="fb839-127">В тексте запроса добавьте представление объекта [ресурса androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb839-127">In the request body, supply a JSON representation for the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

<span data-ttu-id="fb839-128">В следующей таблице приведены свойства, необходимые при создании [ресурса androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span><span class="sxs-lookup"><span data-stu-id="fb839-128">The following table shows the properties that are required when you create the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span></span>

|<span data-ttu-id="fb839-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb839-129">Property</span></span>|<span data-ttu-id="fb839-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fb839-130">Type</span></span>|<span data-ttu-id="fb839-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fb839-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb839-132">id</span><span class="sxs-lookup"><span data-stu-id="fb839-132">id</span></span>|<span data-ttu-id="fb839-133">String</span><span class="sxs-lookup"><span data-stu-id="fb839-133">String</span></span>|<span data-ttu-id="fb839-134">Идентификатор корпоративных параметров учетной записи магазина Android</span><span class="sxs-lookup"><span data-stu-id="fb839-134">The Android store account enterprise settings identifier</span></span>|
|<span data-ttu-id="fb839-135">bindStatus</span><span class="sxs-lookup"><span data-stu-id="fb839-135">bindStatus</span></span>|[<span data-ttu-id="fb839-136">Андроидманажедстореаккаунтбиндстатус</span><span class="sxs-lookup"><span data-stu-id="fb839-136">androidManagedStoreAccountBindStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|<span data-ttu-id="fb839-137">Состояние связывания клиента с помощью API Google EMM.</span><span class="sxs-lookup"><span data-stu-id="fb839-137">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="fb839-138">Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="fb839-138">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="fb839-139">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="fb839-139">lastAppSyncDateTime</span></span>|<span data-ttu-id="fb839-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb839-140">DateTimeOffset</span></span>|<span data-ttu-id="fb839-141">Время завершения последней синхронизации приложения</span><span class="sxs-lookup"><span data-stu-id="fb839-141">Last completion time for app sync</span></span>|
|<span data-ttu-id="fb839-142">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="fb839-142">lastAppSyncStatus</span></span>|[<span data-ttu-id="fb839-143">Андроидманажедстореаккаунтаппсинкстатус</span><span class="sxs-lookup"><span data-stu-id="fb839-143">androidManagedStoreAccountAppSyncStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|<span data-ttu-id="fb839-144">Последний результат синхронизации приложений.</span><span class="sxs-lookup"><span data-stu-id="fb839-144">Last application sync result.</span></span> <span data-ttu-id="fb839-145">Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="fb839-145">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="fb839-146">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fb839-146">ownerUserPrincipalName</span></span>|<span data-ttu-id="fb839-147">String</span><span class="sxs-lookup"><span data-stu-id="fb839-147">String</span></span>|<span data-ttu-id="fb839-148">UPN владельца, создавшего предприятие</span><span class="sxs-lookup"><span data-stu-id="fb839-148">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="fb839-149">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="fb839-149">ownerOrganizationName</span></span>|<span data-ttu-id="fb839-150">String</span><span class="sxs-lookup"><span data-stu-id="fb839-150">String</span></span>|<span data-ttu-id="fb839-151">Название организации, используемое при входящей миграции для Android Enterprise</span><span class="sxs-lookup"><span data-stu-id="fb839-151">Organization name used when onboarding Android Enterprise</span></span>|
|<span data-ttu-id="fb839-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb839-152">lastModifiedDateTime</span></span>|<span data-ttu-id="fb839-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb839-153">DateTimeOffset</span></span>|<span data-ttu-id="fb839-154">Время последнего изменения корпоративных параметров для Android</span><span class="sxs-lookup"><span data-stu-id="fb839-154">Last modification time for Android enterprise settings</span></span>|
|<span data-ttu-id="fb839-155">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="fb839-155">enrollmentTarget</span></span>|[<span data-ttu-id="fb839-156">Андроидманажедстореаккаунтенроллменттаржет</span><span class="sxs-lookup"><span data-stu-id="fb839-156">androidManagedStoreAccountEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|<span data-ttu-id="fb839-157">Указывает, какие пользователи могут регистрировать устройства в управлении устройствами Android Enterprise.</span><span class="sxs-lookup"><span data-stu-id="fb839-157">Indicates which users can enroll devices in Android Enterprise device management.</span></span> <span data-ttu-id="fb839-158">Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="fb839-158">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="fb839-159">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="fb839-159">targetGroupIds</span></span>|<span data-ttu-id="fb839-160">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fb839-160">String collection</span></span>|<span data-ttu-id="fb839-161">Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.</span><span class="sxs-lookup"><span data-stu-id="fb839-161">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="fb839-162">Девицеовнерманажементенаблед</span><span class="sxs-lookup"><span data-stu-id="fb839-162">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="fb839-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb839-163">Boolean</span></span>|<span data-ttu-id="fb839-164">Указывает, передается ли эта учетная запись управлению владельцами устройств Android с помощью Клауддпк.</span><span class="sxs-lookup"><span data-stu-id="fb839-164">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|
|<span data-ttu-id="fb839-165">Компаникодес</span><span class="sxs-lookup"><span data-stu-id="fb839-165">companyCodes</span></span>|<span data-ttu-id="fb839-166">Коллекция [андроиденроллменткомпаникоде](../resources/intune-androidforwork-androidenrollmentcompanycode.md)</span><span class="sxs-lookup"><span data-stu-id="fb839-166">[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md) collection</span></span>|<span data-ttu-id="fb839-167">Коды компаний для ресурса androidmanagedstoreaccountenterprisesettings</span><span class="sxs-lookup"><span data-stu-id="fb839-167">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|
|<span data-ttu-id="fb839-168">Андроиддевицеовнерфуллиманажеденроллментенаблед</span><span class="sxs-lookup"><span data-stu-id="fb839-168">androidDeviceOwnerFullyManagedEnrollmentEnabled</span></span>|<span data-ttu-id="fb839-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb839-169">Boolean</span></span>|<span data-ttu-id="fb839-170">Коды компаний для ресурса androidmanagedstoreaccountenterprisesettings</span><span class="sxs-lookup"><span data-stu-id="fb839-170">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|



## <a name="response"></a><span data-ttu-id="fb839-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb839-171">Response</span></span>
<span data-ttu-id="fb839-172">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [ресурса androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fb839-172">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb839-173">Пример</span><span class="sxs-lookup"><span data-stu-id="fb839-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb839-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb839-174">Request</span></span>
<span data-ttu-id="fb839-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb839-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings
Content-type: application/json
Content-length: 897

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true,
  "companyCodes": [
    {
      "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode",
      "enrollmentToken": "Enrollment Token value",
      "qrCodeContent": "Qr Code Content value",
      "qrCodeImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      }
    }
  ],
  "androidDeviceOwnerFullyManagedEnrollmentEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="fb839-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb839-176">Response</span></span>
<span data-ttu-id="fb839-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb839-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1010

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
  "id": "b71357c9-57c9-b713-c957-13b7c95713b7",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true,
  "companyCodes": [
    {
      "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode",
      "enrollmentToken": "Enrollment Token value",
      "qrCodeContent": "Qr Code Content value",
      "qrCodeImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      }
    }
  ],
  "androidDeviceOwnerFullyManagedEnrollmentEnabled": true
}
```





