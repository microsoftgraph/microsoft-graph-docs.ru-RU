---
title: Update androidForWorkSettings
description: Обновление свойств объекта androidForWorkSettings.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d3693cc86ddb38b16d195e599f7c4d09c9afc1da
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43395587"
---
# <a name="update-androidforworksettings"></a><span data-ttu-id="d0734-103">Update androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="d0734-103">Update androidForWorkSettings</span></span>

<span data-ttu-id="d0734-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0734-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0734-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0734-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0734-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0734-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0734-107">Обновление свойств объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="d0734-107">Update the properties of a [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0734-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d0734-108">Prerequisites</span></span>
<span data-ttu-id="d0734-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0734-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0734-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0734-111">Permission type</span></span>|<span data-ttu-id="d0734-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0734-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0734-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0734-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d0734-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0734-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d0734-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0734-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0734-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0734-116">Not supported.</span></span>|
|<span data-ttu-id="d0734-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="d0734-117">Application</span></span>|<span data-ttu-id="d0734-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0734-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0734-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0734-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="d0734-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d0734-120">Request headers</span></span>
|<span data-ttu-id="d0734-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d0734-121">Header</span></span>|<span data-ttu-id="d0734-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d0734-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0734-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0734-123">Authorization</span></span>|<span data-ttu-id="d0734-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0734-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0734-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d0734-125">Accept</span></span>|<span data-ttu-id="d0734-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d0734-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0734-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0734-127">Request body</span></span>
<span data-ttu-id="d0734-128">В тексте запроса добавьте представление объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0734-128">In the request body, supply a JSON representation for the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

<span data-ttu-id="d0734-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="d0734-129">The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span></span>

|<span data-ttu-id="d0734-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0734-130">Property</span></span>|<span data-ttu-id="d0734-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d0734-131">Type</span></span>|<span data-ttu-id="d0734-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d0734-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0734-133">id</span><span class="sxs-lookup"><span data-stu-id="d0734-133">id</span></span>|<span data-ttu-id="d0734-134">String</span><span class="sxs-lookup"><span data-stu-id="d0734-134">String</span></span>|<span data-ttu-id="d0734-135">Идентификатор параметров Android for Work</span><span class="sxs-lookup"><span data-stu-id="d0734-135">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="d0734-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="d0734-136">bindStatus</span></span>|[<span data-ttu-id="d0734-137">андроидфорворкбиндстатус</span><span class="sxs-lookup"><span data-stu-id="d0734-137">androidForWorkBindStatus</span></span>](../resources/intune-androidforwork-androidforworkbindstatus.md)|<span data-ttu-id="d0734-138">Состояние связывания клиента с помощью API Google EMM.</span><span class="sxs-lookup"><span data-stu-id="d0734-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="d0734-139">Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="d0734-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="d0734-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d0734-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="d0734-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0734-141">DateTimeOffset</span></span>|<span data-ttu-id="d0734-142">Время завершения последней синхронизации приложения</span><span class="sxs-lookup"><span data-stu-id="d0734-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="d0734-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="d0734-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="d0734-144">андроидфорворксинкстатус</span><span class="sxs-lookup"><span data-stu-id="d0734-144">androidForWorkSyncStatus</span></span>](../resources/intune-androidforwork-androidforworksyncstatus.md)|<span data-ttu-id="d0734-145">Последний результат синхронизации приложений.</span><span class="sxs-lookup"><span data-stu-id="d0734-145">Last application sync result.</span></span> <span data-ttu-id="d0734-146">Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="d0734-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="d0734-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d0734-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="d0734-148">String</span><span class="sxs-lookup"><span data-stu-id="d0734-148">String</span></span>|<span data-ttu-id="d0734-149">UPN владельца, создавшего предприятие</span><span class="sxs-lookup"><span data-stu-id="d0734-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="d0734-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="d0734-150">ownerOrganizationName</span></span>|<span data-ttu-id="d0734-151">String</span><span class="sxs-lookup"><span data-stu-id="d0734-151">String</span></span>|<span data-ttu-id="d0734-152">Имя организации, используемое при входящей миграции Android for Work</span><span class="sxs-lookup"><span data-stu-id="d0734-152">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="d0734-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0734-153">lastModifiedDateTime</span></span>|<span data-ttu-id="d0734-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0734-154">DateTimeOffset</span></span>|<span data-ttu-id="d0734-155">Время последнего изменения параметров Android for Work</span><span class="sxs-lookup"><span data-stu-id="d0734-155">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="d0734-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="d0734-156">enrollmentTarget</span></span>|[<span data-ttu-id="d0734-157">андроидфорворкенроллменттаржет</span><span class="sxs-lookup"><span data-stu-id="d0734-157">androidForWorkEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|<span data-ttu-id="d0734-158">Указывает, какие пользователи могут регистрировать устройства в Android для управления рабочими устройствами.</span><span class="sxs-lookup"><span data-stu-id="d0734-158">Indicates which users can enroll devices in Android for Work device management.</span></span> <span data-ttu-id="d0734-159">Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="d0734-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="d0734-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="d0734-160">targetGroupIds</span></span>|<span data-ttu-id="d0734-161">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d0734-161">String collection</span></span>|<span data-ttu-id="d0734-162">Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.</span><span class="sxs-lookup"><span data-stu-id="d0734-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="d0734-163">девицеовнерманажементенаблед</span><span class="sxs-lookup"><span data-stu-id="d0734-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="d0734-164">Логическое</span><span class="sxs-lookup"><span data-stu-id="d0734-164">Boolean</span></span>|<span data-ttu-id="d0734-165">Указывает, передается ли эта учетная запись управлению владельцами устройств Android с помощью Клауддпк.</span><span class="sxs-lookup"><span data-stu-id="d0734-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="d0734-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="d0734-166">Response</span></span>
<span data-ttu-id="d0734-167">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d0734-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0734-168">Пример</span><span class="sxs-lookup"><span data-stu-id="d0734-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0734-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0734-169">Request</span></span>
<span data-ttu-id="d0734-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0734-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d0734-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0734-171">Response</span></span>
<span data-ttu-id="d0734-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0734-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



