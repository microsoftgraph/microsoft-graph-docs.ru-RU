---
title: Обновление ресурса androidmanagedstoreaccountenterprisesettings
description: Обновление свойств объекта ресурса androidmanagedstoreaccountenterprisesettings.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e5df0d4e008dce234858334c42d2841ab2c0332e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43417897"
---
# <a name="update-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="ba1b5-103">Обновление ресурса androidmanagedstoreaccountenterprisesettings</span><span class="sxs-lookup"><span data-stu-id="ba1b5-103">Update androidManagedStoreAccountEnterpriseSettings</span></span>

<span data-ttu-id="ba1b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba1b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba1b5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba1b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba1b5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba1b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba1b5-107">Обновление свойств объекта [ресурса androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="ba1b5-107">Update the properties of a [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba1b5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ba1b5-108">Prerequisites</span></span>
<span data-ttu-id="ba1b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba1b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba1b5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba1b5-111">Permission type</span></span>|<span data-ttu-id="ba1b5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba1b5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba1b5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba1b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba1b5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba1b5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ba1b5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba1b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba1b5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba1b5-116">Not supported.</span></span>|
|<span data-ttu-id="ba1b5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ba1b5-117">Application</span></span>|<span data-ttu-id="ba1b5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba1b5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba1b5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba1b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="request-headers"></a><span data-ttu-id="ba1b5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ba1b5-120">Request headers</span></span>
|<span data-ttu-id="ba1b5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba1b5-121">Header</span></span>|<span data-ttu-id="ba1b5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ba1b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba1b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba1b5-123">Authorization</span></span>|<span data-ttu-id="ba1b5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba1b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba1b5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ba1b5-125">Accept</span></span>|<span data-ttu-id="ba1b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ba1b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba1b5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba1b5-127">Request body</span></span>
<span data-ttu-id="ba1b5-128">В тексте запроса добавьте представление объекта [ресурса androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba1b5-128">In the request body, supply a JSON representation for the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

<span data-ttu-id="ba1b5-129">В следующей таблице приведены свойства, необходимые при создании [ресурса androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span><span class="sxs-lookup"><span data-stu-id="ba1b5-129">The following table shows the properties that are required when you create the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span></span>

|<span data-ttu-id="ba1b5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba1b5-130">Property</span></span>|<span data-ttu-id="ba1b5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ba1b5-131">Type</span></span>|<span data-ttu-id="ba1b5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ba1b5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba1b5-133">id</span><span class="sxs-lookup"><span data-stu-id="ba1b5-133">id</span></span>|<span data-ttu-id="ba1b5-134">String</span><span class="sxs-lookup"><span data-stu-id="ba1b5-134">String</span></span>|<span data-ttu-id="ba1b5-135">Идентификатор корпоративных параметров учетной записи магазина Android</span><span class="sxs-lookup"><span data-stu-id="ba1b5-135">The Android store account enterprise settings identifier</span></span>|
|<span data-ttu-id="ba1b5-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="ba1b5-136">bindStatus</span></span>|[<span data-ttu-id="ba1b5-137">андроидманажедстореаккаунтбиндстатус</span><span class="sxs-lookup"><span data-stu-id="ba1b5-137">androidManagedStoreAccountBindStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|<span data-ttu-id="ba1b5-138">Состояние связывания клиента с помощью API Google EMM.</span><span class="sxs-lookup"><span data-stu-id="ba1b5-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="ba1b5-139">Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="ba1b5-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="ba1b5-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ba1b5-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="ba1b5-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba1b5-141">DateTimeOffset</span></span>|<span data-ttu-id="ba1b5-142">Время завершения последней синхронизации приложения</span><span class="sxs-lookup"><span data-stu-id="ba1b5-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="ba1b5-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="ba1b5-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="ba1b5-144">андроидманажедстореаккаунтаппсинкстатус</span><span class="sxs-lookup"><span data-stu-id="ba1b5-144">androidManagedStoreAccountAppSyncStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|<span data-ttu-id="ba1b5-145">Последний результат синхронизации приложений.</span><span class="sxs-lookup"><span data-stu-id="ba1b5-145">Last application sync result.</span></span> <span data-ttu-id="ba1b5-146">Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="ba1b5-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="ba1b5-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ba1b5-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="ba1b5-148">String</span><span class="sxs-lookup"><span data-stu-id="ba1b5-148">String</span></span>|<span data-ttu-id="ba1b5-149">UPN владельца, создавшего предприятие</span><span class="sxs-lookup"><span data-stu-id="ba1b5-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="ba1b5-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="ba1b5-150">ownerOrganizationName</span></span>|<span data-ttu-id="ba1b5-151">String</span><span class="sxs-lookup"><span data-stu-id="ba1b5-151">String</span></span>|<span data-ttu-id="ba1b5-152">Название организации, используемое при входящей миграции для Android Enterprise</span><span class="sxs-lookup"><span data-stu-id="ba1b5-152">Organization name used when onboarding Android Enterprise</span></span>|
|<span data-ttu-id="ba1b5-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba1b5-153">lastModifiedDateTime</span></span>|<span data-ttu-id="ba1b5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba1b5-154">DateTimeOffset</span></span>|<span data-ttu-id="ba1b5-155">Время последнего изменения корпоративных параметров для Android</span><span class="sxs-lookup"><span data-stu-id="ba1b5-155">Last modification time for Android enterprise settings</span></span>|
|<span data-ttu-id="ba1b5-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="ba1b5-156">enrollmentTarget</span></span>|[<span data-ttu-id="ba1b5-157">андроидманажедстореаккаунтенроллменттаржет</span><span class="sxs-lookup"><span data-stu-id="ba1b5-157">androidManagedStoreAccountEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|<span data-ttu-id="ba1b5-158">Указывает, какие пользователи могут регистрировать устройства в управлении устройствами Android Enterprise.</span><span class="sxs-lookup"><span data-stu-id="ba1b5-158">Indicates which users can enroll devices in Android Enterprise device management.</span></span> <span data-ttu-id="ba1b5-159">Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="ba1b5-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="ba1b5-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="ba1b5-160">targetGroupIds</span></span>|<span data-ttu-id="ba1b5-161">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ba1b5-161">String collection</span></span>|<span data-ttu-id="ba1b5-162">Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.</span><span class="sxs-lookup"><span data-stu-id="ba1b5-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="ba1b5-163">девицеовнерманажементенаблед</span><span class="sxs-lookup"><span data-stu-id="ba1b5-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="ba1b5-164">Логическое</span><span class="sxs-lookup"><span data-stu-id="ba1b5-164">Boolean</span></span>|<span data-ttu-id="ba1b5-165">Указывает, передается ли эта учетная запись управлению владельцами устройств Android с помощью Клауддпк.</span><span class="sxs-lookup"><span data-stu-id="ba1b5-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|
|<span data-ttu-id="ba1b5-166">компаникодес</span><span class="sxs-lookup"><span data-stu-id="ba1b5-166">companyCodes</span></span>|<span data-ttu-id="ba1b5-167">Коллекция [андроиденроллменткомпаникоде](../resources/intune-androidforwork-androidenrollmentcompanycode.md)</span><span class="sxs-lookup"><span data-stu-id="ba1b5-167">[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md) collection</span></span>|<span data-ttu-id="ba1b5-168">Коды компаний для ресурса androidmanagedstoreaccountenterprisesettings</span><span class="sxs-lookup"><span data-stu-id="ba1b5-168">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|
|<span data-ttu-id="ba1b5-169">андроиддевицеовнерфуллиманажеденроллментенаблед</span><span class="sxs-lookup"><span data-stu-id="ba1b5-169">androidDeviceOwnerFullyManagedEnrollmentEnabled</span></span>|<span data-ttu-id="ba1b5-170">Логическое</span><span class="sxs-lookup"><span data-stu-id="ba1b5-170">Boolean</span></span>|<span data-ttu-id="ba1b5-171">Коды компаний для ресурса androidmanagedstoreaccountenterprisesettings</span><span class="sxs-lookup"><span data-stu-id="ba1b5-171">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|



## <a name="response"></a><span data-ttu-id="ba1b5-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba1b5-172">Response</span></span>
<span data-ttu-id="ba1b5-173">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [ресурса androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba1b5-173">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba1b5-174">Пример</span><span class="sxs-lookup"><span data-stu-id="ba1b5-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba1b5-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba1b5-175">Request</span></span>
<span data-ttu-id="ba1b5-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba1b5-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ba1b5-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba1b5-177">Response</span></span>
<span data-ttu-id="ba1b5-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba1b5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



