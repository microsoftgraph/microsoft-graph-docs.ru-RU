---
title: Обновление androidManagedStoreAccountEnterpriseSettings
description: Обновление свойства объекта androidManagedStoreAccountEnterpriseSettings.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e57b7965e5393faf9bdb953dc915652772deb14c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398487"
---
# <a name="update-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="8e7db-103">Обновление androidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="8e7db-103">Update androidManagedStoreAccountEnterpriseSettings</span></span>

> <span data-ttu-id="8e7db-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8e7db-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8e7db-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e7db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e7db-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e7db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e7db-107">Обновление свойства объекта [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="8e7db-107">Update the properties of a [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e7db-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="8e7db-108">Prerequisites</span></span>
<span data-ttu-id="8e7db-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8e7db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8e7db-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e7db-111">Permission type</span></span>|<span data-ttu-id="8e7db-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e7db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e7db-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e7db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8e7db-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e7db-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8e7db-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e7db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e7db-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e7db-116">Not supported.</span></span>|
|<span data-ttu-id="8e7db-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e7db-117">Application</span></span>|<span data-ttu-id="8e7db-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e7db-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e7db-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e7db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="request-headers"></a><span data-ttu-id="8e7db-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e7db-120">Request headers</span></span>
|<span data-ttu-id="8e7db-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e7db-121">Header</span></span>|<span data-ttu-id="8e7db-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8e7db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e7db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e7db-123">Authorization</span></span>|<span data-ttu-id="8e7db-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8e7db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e7db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8e7db-125">Accept</span></span>|<span data-ttu-id="8e7db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e7db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e7db-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e7db-127">Request body</span></span>
<span data-ttu-id="8e7db-128">В тексте запроса укажите представление JSON для объекта [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="8e7db-128">In the request body, supply a JSON representation for the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

<span data-ttu-id="8e7db-129">В следующей таблице показаны свойства, которые необходимы для создания [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span><span class="sxs-lookup"><span data-stu-id="8e7db-129">The following table shows the properties that are required when you create the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span></span>

|<span data-ttu-id="8e7db-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e7db-130">Property</span></span>|<span data-ttu-id="8e7db-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8e7db-131">Type</span></span>|<span data-ttu-id="8e7db-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8e7db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e7db-133">id</span><span class="sxs-lookup"><span data-stu-id="8e7db-133">id</span></span>|<span data-ttu-id="8e7db-134">String</span><span class="sxs-lookup"><span data-stu-id="8e7db-134">String</span></span>|<span data-ttu-id="8e7db-135">Android хранения идентификатора параметров учетной записи предприятия</span><span class="sxs-lookup"><span data-stu-id="8e7db-135">The Android store account enterprise settings identifier</span></span>|
|<span data-ttu-id="8e7db-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="8e7db-136">bindStatus</span></span>|[<span data-ttu-id="8e7db-137">androidManagedStoreAccountBindStatus</span><span class="sxs-lookup"><span data-stu-id="8e7db-137">androidManagedStoreAccountBindStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|<span data-ttu-id="8e7db-138">Привязка состояния клиента с помощью API EMM Google.</span><span class="sxs-lookup"><span data-stu-id="8e7db-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="8e7db-139">Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="8e7db-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="8e7db-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8e7db-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="8e7db-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e7db-141">DateTimeOffset</span></span>|<span data-ttu-id="8e7db-142">Время завершения последней синхронизации приложения</span><span class="sxs-lookup"><span data-stu-id="8e7db-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="8e7db-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="8e7db-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="8e7db-144">androidManagedStoreAccountAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="8e7db-144">androidManagedStoreAccountAppSyncStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|<span data-ttu-id="8e7db-145">Результат последней синхронизации приложения.</span><span class="sxs-lookup"><span data-stu-id="8e7db-145">Last application sync result.</span></span> <span data-ttu-id="8e7db-146">Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="8e7db-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="8e7db-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8e7db-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="8e7db-148">String</span><span class="sxs-lookup"><span data-stu-id="8e7db-148">String</span></span>|<span data-ttu-id="8e7db-149">UPN владельца, создавшего предприятие</span><span class="sxs-lookup"><span data-stu-id="8e7db-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="8e7db-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="8e7db-150">ownerOrganizationName</span></span>|<span data-ttu-id="8e7db-151">String</span><span class="sxs-lookup"><span data-stu-id="8e7db-151">String</span></span>|<span data-ttu-id="8e7db-152">Название организации, используемые при адаптация новых сотрудников предприятия Android</span><span class="sxs-lookup"><span data-stu-id="8e7db-152">Organization name used when onboarding Android Enterprise</span></span>|
|<span data-ttu-id="8e7db-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e7db-153">lastModifiedDateTime</span></span>|<span data-ttu-id="8e7db-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e7db-154">DateTimeOffset</span></span>|<span data-ttu-id="8e7db-155">Время последнего изменения для Android Корпоративные параметры</span><span class="sxs-lookup"><span data-stu-id="8e7db-155">Last modification time for Android enterprise settings</span></span>|
|<span data-ttu-id="8e7db-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="8e7db-156">enrollmentTarget</span></span>|[<span data-ttu-id="8e7db-157">androidManagedStoreAccountEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="8e7db-157">androidManagedStoreAccountEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|<span data-ttu-id="8e7db-158">Указывает пользователей, которые можно зарегистрировать устройств в управление устройствами Android предприятия.</span><span class="sxs-lookup"><span data-stu-id="8e7db-158">Indicates which users can enroll devices in Android Enterprise device management.</span></span> <span data-ttu-id="8e7db-159">Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="8e7db-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="8e7db-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="8e7db-160">targetGroupIds</span></span>|<span data-ttu-id="8e7db-161">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8e7db-161">String collection</span></span>|<span data-ttu-id="8e7db-162">Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.</span><span class="sxs-lookup"><span data-stu-id="8e7db-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="8e7db-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="8e7db-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="8e7db-164">Логический</span><span class="sxs-lookup"><span data-stu-id="8e7db-164">Boolean</span></span>|<span data-ttu-id="8e7db-165">Указывает, если эта учетная запись flighting для Android владелец управление устройствами с CloudDPC.</span><span class="sxs-lookup"><span data-stu-id="8e7db-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|
|<span data-ttu-id="8e7db-166">companyCodes</span><span class="sxs-lookup"><span data-stu-id="8e7db-166">companyCodes</span></span>|<span data-ttu-id="8e7db-167">[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8e7db-167">[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md) collection</span></span>|<span data-ttu-id="8e7db-168">Коды компании для AndroidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="8e7db-168">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|
|<span data-ttu-id="8e7db-169">androidDeviceOwnerFullyManagedEnrollmentEnabled</span><span class="sxs-lookup"><span data-stu-id="8e7db-169">androidDeviceOwnerFullyManagedEnrollmentEnabled</span></span>|<span data-ttu-id="8e7db-170">Логический</span><span class="sxs-lookup"><span data-stu-id="8e7db-170">Boolean</span></span>|<span data-ttu-id="8e7db-171">Коды компании для AndroidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="8e7db-171">Company codes for AndroidManagedStoreAccountEnterpriseSettings</span></span>|



## <a name="response"></a><span data-ttu-id="8e7db-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e7db-172">Response</span></span>
<span data-ttu-id="8e7db-173">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8e7db-173">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e7db-174">Пример</span><span class="sxs-lookup"><span data-stu-id="8e7db-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e7db-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e7db-175">Request</span></span>
<span data-ttu-id="8e7db-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e7db-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8e7db-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e7db-177">Response</span></span>
<span data-ttu-id="8e7db-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8e7db-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




