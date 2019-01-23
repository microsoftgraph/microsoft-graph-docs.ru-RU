---
title: Update androidForWorkSettings
description: Обновление свойств объекта androidForWorkSettings.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7332cc22e32abd3722bb2331c721ef730f0b59b8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401742"
---
# <a name="update-androidforworksettings"></a><span data-ttu-id="84615-103">Update androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="84615-103">Update androidForWorkSettings</span></span>

> <span data-ttu-id="84615-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="84615-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="84615-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84615-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84615-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84615-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84615-107">Обновление свойств объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="84615-107">Update the properties of a [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84615-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="84615-108">Prerequisites</span></span>
<span data-ttu-id="84615-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="84615-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="84615-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84615-111">Permission type</span></span>|<span data-ttu-id="84615-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="84615-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84615-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84615-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84615-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84615-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84615-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84615-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84615-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84615-116">Not supported.</span></span>|
|<span data-ttu-id="84615-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84615-117">Application</span></span>|<span data-ttu-id="84615-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84615-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84615-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84615-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="84615-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84615-120">Request headers</span></span>
|<span data-ttu-id="84615-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84615-121">Header</span></span>|<span data-ttu-id="84615-122">Значение</span><span class="sxs-lookup"><span data-stu-id="84615-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84615-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="84615-123">Authorization</span></span>|<span data-ttu-id="84615-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="84615-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84615-125">Accept</span><span class="sxs-lookup"><span data-stu-id="84615-125">Accept</span></span>|<span data-ttu-id="84615-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84615-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84615-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84615-127">Request body</span></span>
<span data-ttu-id="84615-128">В тексте запроса добавьте представление объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84615-128">In the request body, supply a JSON representation for the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

<span data-ttu-id="84615-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="84615-129">The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span></span>

|<span data-ttu-id="84615-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="84615-130">Property</span></span>|<span data-ttu-id="84615-131">Тип</span><span class="sxs-lookup"><span data-stu-id="84615-131">Type</span></span>|<span data-ttu-id="84615-132">Описание</span><span class="sxs-lookup"><span data-stu-id="84615-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84615-133">id</span><span class="sxs-lookup"><span data-stu-id="84615-133">id</span></span>|<span data-ttu-id="84615-134">String</span><span class="sxs-lookup"><span data-stu-id="84615-134">String</span></span>|<span data-ttu-id="84615-135">Идентификатор параметров Android for Work</span><span class="sxs-lookup"><span data-stu-id="84615-135">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="84615-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="84615-136">bindStatus</span></span>|[<span data-ttu-id="84615-137">androidForWorkBindStatus</span><span class="sxs-lookup"><span data-stu-id="84615-137">androidForWorkBindStatus</span></span>](../resources/intune-androidforwork-androidforworkbindstatus.md)|<span data-ttu-id="84615-138">Привязка состояния клиента с помощью API EMM Google.</span><span class="sxs-lookup"><span data-stu-id="84615-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="84615-139">Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="84615-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="84615-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="84615-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="84615-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84615-141">DateTimeOffset</span></span>|<span data-ttu-id="84615-142">Время завершения последней синхронизации приложения</span><span class="sxs-lookup"><span data-stu-id="84615-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="84615-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="84615-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="84615-144">androidForWorkSyncStatus</span><span class="sxs-lookup"><span data-stu-id="84615-144">androidForWorkSyncStatus</span></span>](../resources/intune-androidforwork-androidforworksyncstatus.md)|<span data-ttu-id="84615-145">Результат последней синхронизации приложения.</span><span class="sxs-lookup"><span data-stu-id="84615-145">Last application sync result.</span></span> <span data-ttu-id="84615-146">Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="84615-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="84615-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="84615-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="84615-148">String</span><span class="sxs-lookup"><span data-stu-id="84615-148">String</span></span>|<span data-ttu-id="84615-149">UPN владельца, создавшего предприятие</span><span class="sxs-lookup"><span data-stu-id="84615-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="84615-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="84615-150">ownerOrganizationName</span></span>|<span data-ttu-id="84615-151">String</span><span class="sxs-lookup"><span data-stu-id="84615-151">String</span></span>|<span data-ttu-id="84615-152">Имя организации, используемое при входящей миграции Android for Work</span><span class="sxs-lookup"><span data-stu-id="84615-152">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="84615-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84615-153">lastModifiedDateTime</span></span>|<span data-ttu-id="84615-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84615-154">DateTimeOffset</span></span>|<span data-ttu-id="84615-155">Время последнего изменения параметров Android for Work</span><span class="sxs-lookup"><span data-stu-id="84615-155">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="84615-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="84615-156">enrollmentTarget</span></span>|[<span data-ttu-id="84615-157">androidForWorkEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="84615-157">androidForWorkEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|<span data-ttu-id="84615-158">Указывает пользователей, которые можно зарегистрировать устройств в Android для управления работой устройства.</span><span class="sxs-lookup"><span data-stu-id="84615-158">Indicates which users can enroll devices in Android for Work device management.</span></span> <span data-ttu-id="84615-159">Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="84615-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="84615-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="84615-160">targetGroupIds</span></span>|<span data-ttu-id="84615-161">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="84615-161">String collection</span></span>|<span data-ttu-id="84615-162">Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.</span><span class="sxs-lookup"><span data-stu-id="84615-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="84615-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="84615-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="84615-164">Логический</span><span class="sxs-lookup"><span data-stu-id="84615-164">Boolean</span></span>|<span data-ttu-id="84615-165">Указывает, если эта учетная запись flighting для Android владелец управление устройствами с CloudDPC.</span><span class="sxs-lookup"><span data-stu-id="84615-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="84615-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="84615-166">Response</span></span>
<span data-ttu-id="84615-167">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="84615-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84615-168">Пример</span><span class="sxs-lookup"><span data-stu-id="84615-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="84615-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="84615-169">Request</span></span>
<span data-ttu-id="84615-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84615-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="84615-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="84615-171">Response</span></span>
<span data-ttu-id="84615-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="84615-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




