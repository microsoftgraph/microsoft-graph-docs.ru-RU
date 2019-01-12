---
title: Обновление androidManagedStoreAccountEnterpriseSettings
description: Обновление свойства объекта androidManagedStoreAccountEnterpriseSettings.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 82c0ee245b7db91d0a145439018c411493a83efb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951084"
---
# <a name="update-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="ed342-103">Обновление androidManagedStoreAccountEnterpriseSettings</span><span class="sxs-lookup"><span data-stu-id="ed342-103">Update androidManagedStoreAccountEnterpriseSettings</span></span>

> <span data-ttu-id="ed342-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ed342-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed342-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed342-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed342-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ed342-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed342-107">Обновление свойства объекта [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="ed342-107">Update the properties of a [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed342-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ed342-108">Prerequisites</span></span>
<span data-ttu-id="ed342-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed342-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed342-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed342-111">Permission type</span></span>|<span data-ttu-id="ed342-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed342-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed342-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed342-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed342-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed342-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ed342-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed342-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed342-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed342-116">Not supported.</span></span>|
|<span data-ttu-id="ed342-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed342-117">Application</span></span>|<span data-ttu-id="ed342-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed342-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed342-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed342-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="request-headers"></a><span data-ttu-id="ed342-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed342-120">Request headers</span></span>
|<span data-ttu-id="ed342-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ed342-121">Header</span></span>|<span data-ttu-id="ed342-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ed342-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed342-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed342-123">Authorization</span></span>|<span data-ttu-id="ed342-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ed342-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed342-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ed342-125">Accept</span></span>|<span data-ttu-id="ed342-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed342-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed342-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ed342-127">Request body</span></span>
<span data-ttu-id="ed342-128">В тексте запроса укажите представление JSON для объекта [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .</span><span class="sxs-lookup"><span data-stu-id="ed342-128">In the request body, supply a JSON representation for the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

<span data-ttu-id="ed342-129">В следующей таблице показаны свойства, которые необходимы для создания [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span><span class="sxs-lookup"><span data-stu-id="ed342-129">The following table shows the properties that are required when you create the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md).</span></span>

|<span data-ttu-id="ed342-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed342-130">Property</span></span>|<span data-ttu-id="ed342-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ed342-131">Type</span></span>|<span data-ttu-id="ed342-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ed342-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed342-133">id</span><span class="sxs-lookup"><span data-stu-id="ed342-133">id</span></span>|<span data-ttu-id="ed342-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ed342-134">String</span></span>|<span data-ttu-id="ed342-135">Android хранения идентификатора параметров учетной записи предприятия</span><span class="sxs-lookup"><span data-stu-id="ed342-135">The Android store account enterprise settings identifier</span></span>|
|<span data-ttu-id="ed342-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="ed342-136">bindStatus</span></span>|[<span data-ttu-id="ed342-137">androidManagedStoreAccountBindStatus</span><span class="sxs-lookup"><span data-stu-id="ed342-137">androidManagedStoreAccountBindStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|<span data-ttu-id="ed342-138">Привязка состояния клиента с помощью API EMM Google.</span><span class="sxs-lookup"><span data-stu-id="ed342-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="ed342-139">Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="ed342-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="ed342-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ed342-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="ed342-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed342-141">DateTimeOffset</span></span>|<span data-ttu-id="ed342-142">Время завершения последней синхронизации приложения</span><span class="sxs-lookup"><span data-stu-id="ed342-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="ed342-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="ed342-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="ed342-144">androidManagedStoreAccountAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="ed342-144">androidManagedStoreAccountAppSyncStatus</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|<span data-ttu-id="ed342-145">Результат последней синхронизации приложения.</span><span class="sxs-lookup"><span data-stu-id="ed342-145">Last application sync result.</span></span> <span data-ttu-id="ed342-146">Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="ed342-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="ed342-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ed342-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="ed342-148">String</span><span class="sxs-lookup"><span data-stu-id="ed342-148">String</span></span>|<span data-ttu-id="ed342-149">UPN владельца, создавшего предприятие</span><span class="sxs-lookup"><span data-stu-id="ed342-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="ed342-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="ed342-150">ownerOrganizationName</span></span>|<span data-ttu-id="ed342-151">String</span><span class="sxs-lookup"><span data-stu-id="ed342-151">String</span></span>|<span data-ttu-id="ed342-152">Название организации, используемые при адаптация новых сотрудников предприятия Android</span><span class="sxs-lookup"><span data-stu-id="ed342-152">Organization name used when onboarding Android Enterprise</span></span>|
|<span data-ttu-id="ed342-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed342-153">lastModifiedDateTime</span></span>|<span data-ttu-id="ed342-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed342-154">DateTimeOffset</span></span>|<span data-ttu-id="ed342-155">Время последнего изменения для Android Корпоративные параметры</span><span class="sxs-lookup"><span data-stu-id="ed342-155">Last modification time for Android enterprise settings</span></span>|
|<span data-ttu-id="ed342-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="ed342-156">enrollmentTarget</span></span>|[<span data-ttu-id="ed342-157">androidManagedStoreAccountEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="ed342-157">androidManagedStoreAccountEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|<span data-ttu-id="ed342-158">Указывает пользователей, которые можно зарегистрировать устройств в управление устройствами Android предприятия.</span><span class="sxs-lookup"><span data-stu-id="ed342-158">Indicates which users can enroll devices in Android Enterprise device management.</span></span> <span data-ttu-id="ed342-159">Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="ed342-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="ed342-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="ed342-160">targetGroupIds</span></span>|<span data-ttu-id="ed342-161">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ed342-161">String collection</span></span>|<span data-ttu-id="ed342-162">Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.</span><span class="sxs-lookup"><span data-stu-id="ed342-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="ed342-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="ed342-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="ed342-164">Логический</span><span class="sxs-lookup"><span data-stu-id="ed342-164">Boolean</span></span>|<span data-ttu-id="ed342-165">Указывает, если эта учетная запись flighting для Android владелец управление устройствами с CloudDPC.</span><span class="sxs-lookup"><span data-stu-id="ed342-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="ed342-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="ed342-166">Response</span></span>
<span data-ttu-id="ed342-167">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ed342-167">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed342-168">Пример</span><span class="sxs-lookup"><span data-stu-id="ed342-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed342-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed342-169">Request</span></span>
<span data-ttu-id="ed342-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed342-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings
Content-type: application/json
Content-length: 458

{
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
  "deviceOwnerManagementEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="ed342-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="ed342-171">Response</span></span>
<span data-ttu-id="ed342-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ed342-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

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
  "deviceOwnerManagementEnabled": true
}
```





