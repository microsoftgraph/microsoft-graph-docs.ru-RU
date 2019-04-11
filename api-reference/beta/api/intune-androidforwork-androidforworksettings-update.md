---
title: Update androidForWorkSettings
description: Обновление свойств объекта androidForWorkSettings.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f71d9087b457189d3796306e0585981c0e58855
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785148"
---
# <a name="update-androidforworksettings"></a><span data-ttu-id="3ff9d-103">Update androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="3ff9d-103">Update androidForWorkSettings</span></span>

> <span data-ttu-id="3ff9d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ff9d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ff9d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ff9d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ff9d-106">Обновление свойств объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="3ff9d-106">Update the properties of a [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ff9d-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3ff9d-107">Prerequisites</span></span>
<span data-ttu-id="3ff9d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ff9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ff9d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ff9d-110">Permission type</span></span>|<span data-ttu-id="3ff9d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ff9d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ff9d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ff9d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3ff9d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ff9d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3ff9d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ff9d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ff9d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ff9d-115">Not supported.</span></span>|
|<span data-ttu-id="3ff9d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ff9d-116">Application</span></span>|<span data-ttu-id="3ff9d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ff9d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ff9d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ff9d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="3ff9d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ff9d-119">Request headers</span></span>
|<span data-ttu-id="3ff9d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ff9d-120">Header</span></span>|<span data-ttu-id="3ff9d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3ff9d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ff9d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ff9d-122">Authorization</span></span>|<span data-ttu-id="3ff9d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ff9d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ff9d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3ff9d-124">Accept</span></span>|<span data-ttu-id="3ff9d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3ff9d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ff9d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ff9d-126">Request body</span></span>
<span data-ttu-id="3ff9d-127">В тексте запроса добавьте представление объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ff9d-127">In the request body, supply a JSON representation for the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

<span data-ttu-id="3ff9d-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="3ff9d-128">The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span></span>

|<span data-ttu-id="3ff9d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ff9d-129">Property</span></span>|<span data-ttu-id="3ff9d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3ff9d-130">Type</span></span>|<span data-ttu-id="3ff9d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3ff9d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ff9d-132">id</span><span class="sxs-lookup"><span data-stu-id="3ff9d-132">id</span></span>|<span data-ttu-id="3ff9d-133">String</span><span class="sxs-lookup"><span data-stu-id="3ff9d-133">String</span></span>|<span data-ttu-id="3ff9d-134">Идентификатор параметров Android for Work</span><span class="sxs-lookup"><span data-stu-id="3ff9d-134">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="3ff9d-135">bindStatus</span><span class="sxs-lookup"><span data-stu-id="3ff9d-135">bindStatus</span></span>|[<span data-ttu-id="3ff9d-136">Андроидфорворкбиндстатус</span><span class="sxs-lookup"><span data-stu-id="3ff9d-136">androidForWorkBindStatus</span></span>](../resources/intune-androidforwork-androidforworkbindstatus.md)|<span data-ttu-id="3ff9d-137">Состояние связывания клиента с помощью API Google EMM.</span><span class="sxs-lookup"><span data-stu-id="3ff9d-137">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="3ff9d-138">Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="3ff9d-138">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="3ff9d-139">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3ff9d-139">lastAppSyncDateTime</span></span>|<span data-ttu-id="3ff9d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ff9d-140">DateTimeOffset</span></span>|<span data-ttu-id="3ff9d-141">Время завершения последней синхронизации приложения</span><span class="sxs-lookup"><span data-stu-id="3ff9d-141">Last completion time for app sync</span></span>|
|<span data-ttu-id="3ff9d-142">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="3ff9d-142">lastAppSyncStatus</span></span>|[<span data-ttu-id="3ff9d-143">Андроидфорворксинкстатус</span><span class="sxs-lookup"><span data-stu-id="3ff9d-143">androidForWorkSyncStatus</span></span>](../resources/intune-androidforwork-androidforworksyncstatus.md)|<span data-ttu-id="3ff9d-144">Последний результат синхронизации приложений.</span><span class="sxs-lookup"><span data-stu-id="3ff9d-144">Last application sync result.</span></span> <span data-ttu-id="3ff9d-145">Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="3ff9d-145">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="3ff9d-146">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3ff9d-146">ownerUserPrincipalName</span></span>|<span data-ttu-id="3ff9d-147">String</span><span class="sxs-lookup"><span data-stu-id="3ff9d-147">String</span></span>|<span data-ttu-id="3ff9d-148">UPN владельца, создавшего предприятие</span><span class="sxs-lookup"><span data-stu-id="3ff9d-148">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="3ff9d-149">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="3ff9d-149">ownerOrganizationName</span></span>|<span data-ttu-id="3ff9d-150">String</span><span class="sxs-lookup"><span data-stu-id="3ff9d-150">String</span></span>|<span data-ttu-id="3ff9d-151">Имя организации, используемое при входящей миграции Android for Work</span><span class="sxs-lookup"><span data-stu-id="3ff9d-151">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="3ff9d-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ff9d-152">lastModifiedDateTime</span></span>|<span data-ttu-id="3ff9d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ff9d-153">DateTimeOffset</span></span>|<span data-ttu-id="3ff9d-154">Время последнего изменения параметров Android for Work</span><span class="sxs-lookup"><span data-stu-id="3ff9d-154">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="3ff9d-155">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="3ff9d-155">enrollmentTarget</span></span>|[<span data-ttu-id="3ff9d-156">Андроидфорворкенроллменттаржет</span><span class="sxs-lookup"><span data-stu-id="3ff9d-156">androidForWorkEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|<span data-ttu-id="3ff9d-157">Указывает, какие пользователи могут регистрировать устройства в Android для управления рабочими устройствами.</span><span class="sxs-lookup"><span data-stu-id="3ff9d-157">Indicates which users can enroll devices in Android for Work device management.</span></span> <span data-ttu-id="3ff9d-158">Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="3ff9d-158">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="3ff9d-159">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="3ff9d-159">targetGroupIds</span></span>|<span data-ttu-id="3ff9d-160">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3ff9d-160">String collection</span></span>|<span data-ttu-id="3ff9d-161">Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.</span><span class="sxs-lookup"><span data-stu-id="3ff9d-161">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="3ff9d-162">Девицеовнерманажементенаблед</span><span class="sxs-lookup"><span data-stu-id="3ff9d-162">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="3ff9d-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ff9d-163">Boolean</span></span>|<span data-ttu-id="3ff9d-164">Указывает, передается ли эта учетная запись управлению владельцами устройств Android с помощью Клауддпк.</span><span class="sxs-lookup"><span data-stu-id="3ff9d-164">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="3ff9d-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ff9d-165">Response</span></span>
<span data-ttu-id="3ff9d-166">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3ff9d-166">If successful, this method returns a `200 OK` response code and an updated [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ff9d-167">Пример</span><span class="sxs-lookup"><span data-stu-id="3ff9d-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ff9d-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ff9d-168">Request</span></span>
<span data-ttu-id="3ff9d-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ff9d-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3ff9d-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ff9d-170">Response</span></span>
<span data-ttu-id="3ff9d-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ff9d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





