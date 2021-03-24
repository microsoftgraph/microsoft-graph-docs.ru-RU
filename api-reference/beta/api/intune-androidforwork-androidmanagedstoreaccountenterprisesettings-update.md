---
title: Обновление androidManagedStoreAccountEnterpriseSettings
description: Обновление свойств объекта AndroidManagedStoreAccountEnterpriseSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc7a1cd9291ca0fad18dedd905b484536fbe2fb0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141136"
---
# <a name="update-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="74282-103">Обновление androidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="74282-103">Update androidManagedStoreAccountEnterpriseSettings</span></span>

<span data-ttu-id="74282-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74282-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74282-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74282-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74282-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="74282-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74282-107">Обновление свойств объекта [AndroidManagedStoreAccountEnterpriseSettings.](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)</span><span class="sxs-lookup"><span data-stu-id="74282-107">Update the properties of a [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74282-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="74282-108">Prerequisites</span></span>
<span data-ttu-id="74282-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74282-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74282-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74282-111">Permission type</span></span>|<span data-ttu-id="74282-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74282-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74282-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74282-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74282-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74282-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="74282-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74282-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74282-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74282-116">Not supported.</span></span>|
|<span data-ttu-id="74282-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="74282-117">Application</span></span>|<span data-ttu-id="74282-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74282-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="74282-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74282-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="request-headers"></a><span data-ttu-id="74282-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="74282-120">Request headers</span></span>
|<span data-ttu-id="74282-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74282-121">Header</span></span>|<span data-ttu-id="74282-122">Значение</span><span class="sxs-lookup"><span data-stu-id="74282-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74282-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74282-123">Authorization</span></span>|<span data-ttu-id="74282-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74282-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74282-125">Accept</span><span class="sxs-lookup"><span data-stu-id="74282-125">Accept</span></span>|<span data-ttu-id="74282-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74282-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74282-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74282-127">Request body</span></span>
<span data-ttu-id="74282-128">В теле запроса поставляем представление JSON для [объекта AndroidManagedStoreAccountEnterpriseSettings.](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)</span><span class="sxs-lookup"><span data-stu-id="74282-128">In the request body, supply a JSON representation for the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

<span data-ttu-id="74282-129">В следующей таблице показаны свойства, необходимые при создании [androidManagedStoreAccountEnterpriseSettings.](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)</span><span class="sxs-lookup"><span data-stu-id="74282-129">The following table shows the properties that are required when you create the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span></span>

|<span data-ttu-id="74282-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="74282-130">Property</span></span>|<span data-ttu-id="74282-131">Тип</span><span class="sxs-lookup"><span data-stu-id="74282-131">Type</span></span>|<span data-ttu-id="74282-132">Описание</span><span class="sxs-lookup"><span data-stu-id="74282-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74282-133">id</span><span class="sxs-lookup"><span data-stu-id="74282-133">id</span></span>|<span data-ttu-id="74282-134">Строка</span><span class="sxs-lookup"><span data-stu-id="74282-134">String</span></span>|<span data-ttu-id="74282-135">Идентификатор корпоративных параметров учетной записи магазина Android</span><span class="sxs-lookup"><span data-stu-id="74282-135">The Android store account enterprise settings identifier</span></span>|
|<span data-ttu-id="74282-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="74282-136">bindStatus</span></span>|[<span data-ttu-id="74282-137">AndroidManagedStoreAccountBindStatus</span><span class="sxs-lookup"><span data-stu-id="74282-137">androidManagedStoreAccountBindStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|<span data-ttu-id="74282-138">Связать состояние клиента с API EMM Google.</span><span class="sxs-lookup"><span data-stu-id="74282-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="74282-139">Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="74282-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="74282-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="74282-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="74282-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74282-141">DateTimeOffset</span></span>|<span data-ttu-id="74282-142">Время завершения последней синхронизации приложения</span><span class="sxs-lookup"><span data-stu-id="74282-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="74282-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="74282-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="74282-144">AndroidManagedStoreAccountAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="74282-144">androidManagedStoreAccountAppSyncStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|<span data-ttu-id="74282-145">Результат синхронизации последнего приложения.</span><span class="sxs-lookup"><span data-stu-id="74282-145">Last application sync result.</span></span> <span data-ttu-id="74282-146">Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="74282-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="74282-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="74282-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="74282-148">String</span><span class="sxs-lookup"><span data-stu-id="74282-148">String</span></span>|<span data-ttu-id="74282-149">UPN владельца, создавшего предприятие</span><span class="sxs-lookup"><span data-stu-id="74282-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="74282-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="74282-150">ownerOrganizationName</span></span>|<span data-ttu-id="74282-151">String</span><span class="sxs-lookup"><span data-stu-id="74282-151">String</span></span>|<span data-ttu-id="74282-152">Имя организации, используемая при взявке Android Enterprise</span><span class="sxs-lookup"><span data-stu-id="74282-152">Organization name used when onboarding Android Enterprise</span></span>|
|<span data-ttu-id="74282-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74282-153">lastModifiedDateTime</span></span>|<span data-ttu-id="74282-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74282-154">DateTimeOffset</span></span>|<span data-ttu-id="74282-155">Время последней модификации для корпоративных параметров Android</span><span class="sxs-lookup"><span data-stu-id="74282-155">Last modification time for Android enterprise settings</span></span>|
|<span data-ttu-id="74282-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="74282-156">enrollmentTarget</span></span>|[<span data-ttu-id="74282-157">AndroidManagedStoreAccountEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="74282-157">androidManagedStoreAccountEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|<span data-ttu-id="74282-158">Указывает, какие пользователи могут записать устройства в управление устройствами Android Enterprise.</span><span class="sxs-lookup"><span data-stu-id="74282-158">Indicates which users can enroll devices in Android Enterprise device management.</span></span> <span data-ttu-id="74282-159">Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="74282-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="74282-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="74282-160">targetGroupIds</span></span>|<span data-ttu-id="74282-161">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="74282-161">String collection</span></span>|<span data-ttu-id="74282-162">Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.</span><span class="sxs-lookup"><span data-stu-id="74282-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="74282-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="74282-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="74282-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="74282-164">Boolean</span></span>|<span data-ttu-id="74282-165">Указывает, работает ли эта учетная запись для управления владельцем android-устройств с помощью CloudDPC.</span><span class="sxs-lookup"><span data-stu-id="74282-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|
|<span data-ttu-id="74282-166">companyCodes</span><span class="sxs-lookup"><span data-stu-id="74282-166">companyCodes</span></span>|<span data-ttu-id="74282-167">[коллекция androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md)</span><span class="sxs-lookup"><span data-stu-id="74282-167">[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md) collection</span></span>|<span data-ttu-id="74282-168">Коды компании для AndroidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="74282-168">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|
|<span data-ttu-id="74282-169">androidDeviceOwnerFullyManagedEnrollmentEnabled</span><span class="sxs-lookup"><span data-stu-id="74282-169">androidDeviceOwnerFullyManagedEnrollmentEnabled</span></span>|<span data-ttu-id="74282-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="74282-170">Boolean</span></span>|<span data-ttu-id="74282-171">Коды компании для AndroidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="74282-171">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|



## <a name="response"></a><span data-ttu-id="74282-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="74282-172">Response</span></span>
<span data-ttu-id="74282-173">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект AndroidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="74282-173">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74282-174">Пример</span><span class="sxs-lookup"><span data-stu-id="74282-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="74282-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="74282-175">Request</span></span>
<span data-ttu-id="74282-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74282-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="74282-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="74282-177">Response</span></span>
<span data-ttu-id="74282-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="74282-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




