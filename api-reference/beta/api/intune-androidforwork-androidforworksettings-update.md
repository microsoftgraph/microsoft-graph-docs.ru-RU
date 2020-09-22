---
title: Update androidForWorkSettings
description: Обновление свойств объекта androidForWorkSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b7edae1508e981c9afac05fd7b5919b845e52a19
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006533"
---
# <a name="update-androidforworksettings"></a><span data-ttu-id="30727-103">Update androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="30727-103">Update androidForWorkSettings</span></span>

<span data-ttu-id="30727-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30727-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30727-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30727-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30727-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30727-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30727-107">Обновление свойств объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="30727-107">Update the properties of a [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30727-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="30727-108">Prerequisites</span></span>
<span data-ttu-id="30727-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30727-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30727-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30727-111">Permission type</span></span>|<span data-ttu-id="30727-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="30727-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30727-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30727-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30727-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30727-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="30727-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30727-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30727-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30727-116">Not supported.</span></span>|
|<span data-ttu-id="30727-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30727-117">Application</span></span>|<span data-ttu-id="30727-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30727-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30727-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30727-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="30727-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="30727-120">Request headers</span></span>
|<span data-ttu-id="30727-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30727-121">Header</span></span>|<span data-ttu-id="30727-122">Значение</span><span class="sxs-lookup"><span data-stu-id="30727-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30727-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="30727-123">Authorization</span></span>|<span data-ttu-id="30727-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30727-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30727-125">Accept</span><span class="sxs-lookup"><span data-stu-id="30727-125">Accept</span></span>|<span data-ttu-id="30727-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30727-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30727-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="30727-127">Request body</span></span>
<span data-ttu-id="30727-128">В тексте запроса добавьте представление объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30727-128">In the request body, supply a JSON representation for the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

<span data-ttu-id="30727-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="30727-129">The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span></span>

|<span data-ttu-id="30727-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="30727-130">Property</span></span>|<span data-ttu-id="30727-131">Тип</span><span class="sxs-lookup"><span data-stu-id="30727-131">Type</span></span>|<span data-ttu-id="30727-132">Описание</span><span class="sxs-lookup"><span data-stu-id="30727-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30727-133">id</span><span class="sxs-lookup"><span data-stu-id="30727-133">id</span></span>|<span data-ttu-id="30727-134">String</span><span class="sxs-lookup"><span data-stu-id="30727-134">String</span></span>|<span data-ttu-id="30727-135">Идентификатор параметров Android for Work</span><span class="sxs-lookup"><span data-stu-id="30727-135">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="30727-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="30727-136">bindStatus</span></span>|[<span data-ttu-id="30727-137">андроидфорворкбиндстатус</span><span class="sxs-lookup"><span data-stu-id="30727-137">androidForWorkBindStatus</span></span>](../resources/intune-androidforwork-androidforworkbindstatus.md)|<span data-ttu-id="30727-138">Состояние связывания клиента с помощью API Google EMM.</span><span class="sxs-lookup"><span data-stu-id="30727-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="30727-139">Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="30727-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="30727-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="30727-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="30727-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30727-141">DateTimeOffset</span></span>|<span data-ttu-id="30727-142">Время завершения последней синхронизации приложения</span><span class="sxs-lookup"><span data-stu-id="30727-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="30727-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="30727-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="30727-144">андроидфорворксинкстатус</span><span class="sxs-lookup"><span data-stu-id="30727-144">androidForWorkSyncStatus</span></span>](../resources/intune-androidforwork-androidforworksyncstatus.md)|<span data-ttu-id="30727-145">Последний результат синхронизации приложений.</span><span class="sxs-lookup"><span data-stu-id="30727-145">Last application sync result.</span></span> <span data-ttu-id="30727-146">Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="30727-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="30727-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="30727-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="30727-148">String</span><span class="sxs-lookup"><span data-stu-id="30727-148">String</span></span>|<span data-ttu-id="30727-149">UPN владельца, создавшего предприятие</span><span class="sxs-lookup"><span data-stu-id="30727-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="30727-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="30727-150">ownerOrganizationName</span></span>|<span data-ttu-id="30727-151">String</span><span class="sxs-lookup"><span data-stu-id="30727-151">String</span></span>|<span data-ttu-id="30727-152">Имя организации, используемое при входящей миграции Android for Work</span><span class="sxs-lookup"><span data-stu-id="30727-152">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="30727-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30727-153">lastModifiedDateTime</span></span>|<span data-ttu-id="30727-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30727-154">DateTimeOffset</span></span>|<span data-ttu-id="30727-155">Время последнего изменения параметров Android for Work</span><span class="sxs-lookup"><span data-stu-id="30727-155">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="30727-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="30727-156">enrollmentTarget</span></span>|[<span data-ttu-id="30727-157">андроидфорворкенроллменттаржет</span><span class="sxs-lookup"><span data-stu-id="30727-157">androidForWorkEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|<span data-ttu-id="30727-158">Указывает, какие пользователи могут регистрировать устройства в Android для управления рабочими устройствами.</span><span class="sxs-lookup"><span data-stu-id="30727-158">Indicates which users can enroll devices in Android for Work device management.</span></span> <span data-ttu-id="30727-159">Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="30727-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="30727-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="30727-160">targetGroupIds</span></span>|<span data-ttu-id="30727-161">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="30727-161">String collection</span></span>|<span data-ttu-id="30727-162">Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.</span><span class="sxs-lookup"><span data-stu-id="30727-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="30727-163">девицеовнерманажементенаблед</span><span class="sxs-lookup"><span data-stu-id="30727-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="30727-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="30727-164">Boolean</span></span>|<span data-ttu-id="30727-165">Указывает, передается ли эта учетная запись управлению владельцами устройств Android с помощью Клауддпк.</span><span class="sxs-lookup"><span data-stu-id="30727-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="30727-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="30727-166">Response</span></span>
<span data-ttu-id="30727-167">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="30727-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30727-168">Пример</span><span class="sxs-lookup"><span data-stu-id="30727-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="30727-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="30727-169">Request</span></span>
<span data-ttu-id="30727-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30727-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ],
  "deviceOwnerManagementEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="30727-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="30727-171">Response</span></span>
<span data-ttu-id="30727-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30727-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 568

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "97adc169-c169-97ad-69c1-ad9769c1ad97",
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






