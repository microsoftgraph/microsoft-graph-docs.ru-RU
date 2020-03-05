---
title: Update androidForWorkSettings
description: Обновление свойств объекта androidForWorkSettings.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ac9fdee72acfedfd8200dcd8c6df8008f4447310
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446144"
---
# <a name="update-androidforworksettings"></a><span data-ttu-id="b0bbf-103">Update androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="b0bbf-103">Update androidForWorkSettings</span></span>

<span data-ttu-id="b0bbf-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b0bbf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0bbf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0bbf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0bbf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0bbf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0bbf-107">Обновление свойств объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="b0bbf-107">Update the properties of a [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0bbf-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b0bbf-108">Prerequisites</span></span>
<span data-ttu-id="b0bbf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0bbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0bbf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0bbf-111">Permission type</span></span>|<span data-ttu-id="b0bbf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0bbf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0bbf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0bbf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0bbf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0bbf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0bbf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0bbf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0bbf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0bbf-116">Not supported.</span></span>|
|<span data-ttu-id="b0bbf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0bbf-117">Application</span></span>|<span data-ttu-id="b0bbf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0bbf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0bbf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0bbf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="b0bbf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b0bbf-120">Request headers</span></span>
|<span data-ttu-id="b0bbf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0bbf-121">Header</span></span>|<span data-ttu-id="b0bbf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b0bbf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0bbf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0bbf-123">Authorization</span></span>|<span data-ttu-id="b0bbf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0bbf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0bbf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b0bbf-125">Accept</span></span>|<span data-ttu-id="b0bbf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0bbf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0bbf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0bbf-127">Request body</span></span>
<span data-ttu-id="b0bbf-128">В тексте запроса добавьте представление объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0bbf-128">In the request body, supply a JSON representation for the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

<span data-ttu-id="b0bbf-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="b0bbf-129">The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span></span>

|<span data-ttu-id="b0bbf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0bbf-130">Property</span></span>|<span data-ttu-id="b0bbf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b0bbf-131">Type</span></span>|<span data-ttu-id="b0bbf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b0bbf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0bbf-133">id</span><span class="sxs-lookup"><span data-stu-id="b0bbf-133">id</span></span>|<span data-ttu-id="b0bbf-134">String</span><span class="sxs-lookup"><span data-stu-id="b0bbf-134">String</span></span>|<span data-ttu-id="b0bbf-135">Идентификатор параметров Android for Work</span><span class="sxs-lookup"><span data-stu-id="b0bbf-135">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="b0bbf-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="b0bbf-136">bindStatus</span></span>|[<span data-ttu-id="b0bbf-137">андроидфорворкбиндстатус</span><span class="sxs-lookup"><span data-stu-id="b0bbf-137">androidForWorkBindStatus</span></span>](../resources/intune-androidforwork-androidforworkbindstatus.md)|<span data-ttu-id="b0bbf-138">Состояние связывания клиента с помощью API Google EMM.</span><span class="sxs-lookup"><span data-stu-id="b0bbf-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="b0bbf-139">Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="b0bbf-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="b0bbf-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b0bbf-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="b0bbf-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0bbf-141">DateTimeOffset</span></span>|<span data-ttu-id="b0bbf-142">Время завершения последней синхронизации приложения</span><span class="sxs-lookup"><span data-stu-id="b0bbf-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="b0bbf-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="b0bbf-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="b0bbf-144">андроидфорворксинкстатус</span><span class="sxs-lookup"><span data-stu-id="b0bbf-144">androidForWorkSyncStatus</span></span>](../resources/intune-androidforwork-androidforworksyncstatus.md)|<span data-ttu-id="b0bbf-145">Последний результат синхронизации приложений.</span><span class="sxs-lookup"><span data-stu-id="b0bbf-145">Last application sync result.</span></span> <span data-ttu-id="b0bbf-146">Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="b0bbf-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="b0bbf-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b0bbf-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="b0bbf-148">String</span><span class="sxs-lookup"><span data-stu-id="b0bbf-148">String</span></span>|<span data-ttu-id="b0bbf-149">UPN владельца, создавшего предприятие</span><span class="sxs-lookup"><span data-stu-id="b0bbf-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="b0bbf-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="b0bbf-150">ownerOrganizationName</span></span>|<span data-ttu-id="b0bbf-151">String</span><span class="sxs-lookup"><span data-stu-id="b0bbf-151">String</span></span>|<span data-ttu-id="b0bbf-152">Имя организации, используемое при входящей миграции Android for Work</span><span class="sxs-lookup"><span data-stu-id="b0bbf-152">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="b0bbf-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0bbf-153">lastModifiedDateTime</span></span>|<span data-ttu-id="b0bbf-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0bbf-154">DateTimeOffset</span></span>|<span data-ttu-id="b0bbf-155">Время последнего изменения параметров Android for Work</span><span class="sxs-lookup"><span data-stu-id="b0bbf-155">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="b0bbf-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="b0bbf-156">enrollmentTarget</span></span>|[<span data-ttu-id="b0bbf-157">андроидфорворкенроллменттаржет</span><span class="sxs-lookup"><span data-stu-id="b0bbf-157">androidForWorkEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|<span data-ttu-id="b0bbf-158">Указывает, какие пользователи могут регистрировать устройства в Android для управления рабочими устройствами.</span><span class="sxs-lookup"><span data-stu-id="b0bbf-158">Indicates which users can enroll devices in Android for Work device management.</span></span> <span data-ttu-id="b0bbf-159">Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="b0bbf-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="b0bbf-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="b0bbf-160">targetGroupIds</span></span>|<span data-ttu-id="b0bbf-161">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b0bbf-161">String collection</span></span>|<span data-ttu-id="b0bbf-162">Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.</span><span class="sxs-lookup"><span data-stu-id="b0bbf-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="b0bbf-163">девицеовнерманажементенаблед</span><span class="sxs-lookup"><span data-stu-id="b0bbf-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="b0bbf-164">Логический</span><span class="sxs-lookup"><span data-stu-id="b0bbf-164">Boolean</span></span>|<span data-ttu-id="b0bbf-165">Указывает, передается ли эта учетная запись управлению владельцами устройств Android с помощью Клауддпк.</span><span class="sxs-lookup"><span data-stu-id="b0bbf-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="b0bbf-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0bbf-166">Response</span></span>
<span data-ttu-id="b0bbf-167">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b0bbf-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0bbf-168">Пример</span><span class="sxs-lookup"><span data-stu-id="b0bbf-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0bbf-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0bbf-169">Request</span></span>
<span data-ttu-id="b0bbf-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0bbf-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b0bbf-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0bbf-171">Response</span></span>
<span data-ttu-id="b0bbf-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0bbf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





