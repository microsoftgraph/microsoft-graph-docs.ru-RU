---
title: Update androidForWorkSettings
description: Обновление свойств объекта androidForWorkSettings.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 65550bc588eb5fb0f4d2f11ac785d458e8821a7d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170793"
---
# <a name="update-androidforworksettings"></a><span data-ttu-id="2b6b5-103">Update androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="2b6b5-103">Update androidForWorkSettings</span></span>

> <span data-ttu-id="2b6b5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b6b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b6b5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b6b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b6b5-106">Обновление свойств объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="2b6b5-106">Update the properties of a [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b6b5-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2b6b5-107">Prerequisites</span></span>
<span data-ttu-id="2b6b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2b6b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2b6b5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b6b5-110">Permission type</span></span>|<span data-ttu-id="2b6b5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b6b5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b6b5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b6b5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2b6b5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b6b5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2b6b5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b6b5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b6b5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b6b5-115">Not supported.</span></span>|
|<span data-ttu-id="2b6b5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b6b5-116">Application</span></span>|<span data-ttu-id="2b6b5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b6b5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b6b5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b6b5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="2b6b5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b6b5-119">Request headers</span></span>
|<span data-ttu-id="2b6b5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b6b5-120">Header</span></span>|<span data-ttu-id="2b6b5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2b6b5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b6b5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b6b5-122">Authorization</span></span>|<span data-ttu-id="2b6b5-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2b6b5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b6b5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2b6b5-124">Accept</span></span>|<span data-ttu-id="2b6b5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2b6b5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b6b5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b6b5-126">Request body</span></span>
<span data-ttu-id="2b6b5-127">В тексте запроса добавьте представление объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b6b5-127">In the request body, supply a JSON representation for the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

<span data-ttu-id="2b6b5-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="2b6b5-128">The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span></span>

|<span data-ttu-id="2b6b5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b6b5-129">Property</span></span>|<span data-ttu-id="2b6b5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2b6b5-130">Type</span></span>|<span data-ttu-id="2b6b5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2b6b5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b6b5-132">id</span><span class="sxs-lookup"><span data-stu-id="2b6b5-132">id</span></span>|<span data-ttu-id="2b6b5-133">Строка</span><span class="sxs-lookup"><span data-stu-id="2b6b5-133">String</span></span>|<span data-ttu-id="2b6b5-134">Идентификатор параметров Android for Work</span><span class="sxs-lookup"><span data-stu-id="2b6b5-134">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="2b6b5-135">bindStatus</span><span class="sxs-lookup"><span data-stu-id="2b6b5-135">bindStatus</span></span>|[<span data-ttu-id="2b6b5-136">Андроидфорворкбиндстатус</span><span class="sxs-lookup"><span data-stu-id="2b6b5-136">androidForWorkBindStatus</span></span>](../resources/intune-androidforwork-androidforworkbindstatus.md)|<span data-ttu-id="2b6b5-137">Состояние связывания клиента с помощью API Google EMM.</span><span class="sxs-lookup"><span data-stu-id="2b6b5-137">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="2b6b5-138">Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="2b6b5-138">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="2b6b5-139">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2b6b5-139">lastAppSyncDateTime</span></span>|<span data-ttu-id="2b6b5-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b6b5-140">DateTimeOffset</span></span>|<span data-ttu-id="2b6b5-141">Время завершения последней синхронизации приложения</span><span class="sxs-lookup"><span data-stu-id="2b6b5-141">Last completion time for app sync</span></span>|
|<span data-ttu-id="2b6b5-142">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="2b6b5-142">lastAppSyncStatus</span></span>|[<span data-ttu-id="2b6b5-143">Андроидфорворксинкстатус</span><span class="sxs-lookup"><span data-stu-id="2b6b5-143">androidForWorkSyncStatus</span></span>](../resources/intune-androidforwork-androidforworksyncstatus.md)|<span data-ttu-id="2b6b5-144">Последний результат синхронизации приложений.</span><span class="sxs-lookup"><span data-stu-id="2b6b5-144">Last application sync result.</span></span> <span data-ttu-id="2b6b5-145">Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="2b6b5-145">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="2b6b5-146">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2b6b5-146">ownerUserPrincipalName</span></span>|<span data-ttu-id="2b6b5-147">String</span><span class="sxs-lookup"><span data-stu-id="2b6b5-147">String</span></span>|<span data-ttu-id="2b6b5-148">UPN владельца, создавшего предприятие</span><span class="sxs-lookup"><span data-stu-id="2b6b5-148">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="2b6b5-149">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="2b6b5-149">ownerOrganizationName</span></span>|<span data-ttu-id="2b6b5-150">String</span><span class="sxs-lookup"><span data-stu-id="2b6b5-150">String</span></span>|<span data-ttu-id="2b6b5-151">Имя организации, используемое при входящей миграции Android for Work</span><span class="sxs-lookup"><span data-stu-id="2b6b5-151">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="2b6b5-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b6b5-152">lastModifiedDateTime</span></span>|<span data-ttu-id="2b6b5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b6b5-153">DateTimeOffset</span></span>|<span data-ttu-id="2b6b5-154">Время последнего изменения параметров Android for Work</span><span class="sxs-lookup"><span data-stu-id="2b6b5-154">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="2b6b5-155">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="2b6b5-155">enrollmentTarget</span></span>|[<span data-ttu-id="2b6b5-156">Андроидфорворкенроллменттаржет</span><span class="sxs-lookup"><span data-stu-id="2b6b5-156">androidForWorkEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|<span data-ttu-id="2b6b5-157">Указывает, какие пользователи могут регистрировать устройства в Android для управления рабочими устройствами.</span><span class="sxs-lookup"><span data-stu-id="2b6b5-157">Indicates which users can enroll devices in Android for Work device management.</span></span> <span data-ttu-id="2b6b5-158">Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="2b6b5-158">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="2b6b5-159">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="2b6b5-159">targetGroupIds</span></span>|<span data-ttu-id="2b6b5-160">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2b6b5-160">String collection</span></span>|<span data-ttu-id="2b6b5-161">Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.</span><span class="sxs-lookup"><span data-stu-id="2b6b5-161">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="2b6b5-162">Девицеовнерманажементенаблед</span><span class="sxs-lookup"><span data-stu-id="2b6b5-162">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="2b6b5-163">Логический</span><span class="sxs-lookup"><span data-stu-id="2b6b5-163">Boolean</span></span>|<span data-ttu-id="2b6b5-164">Указывает, передается ли эта учетная запись управлению владельцами устройств Android с помощью Клауддпк.</span><span class="sxs-lookup"><span data-stu-id="2b6b5-164">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="2b6b5-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b6b5-165">Response</span></span>
<span data-ttu-id="2b6b5-166">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2b6b5-166">If successful, this method returns a `200 OK` response code and an updated [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b6b5-167">Пример</span><span class="sxs-lookup"><span data-stu-id="2b6b5-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b6b5-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b6b5-168">Request</span></span>
<span data-ttu-id="2b6b5-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b6b5-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2b6b5-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b6b5-170">Response</span></span>
<span data-ttu-id="2b6b5-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b6b5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




