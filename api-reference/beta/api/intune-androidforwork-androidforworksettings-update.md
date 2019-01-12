---
title: Update androidForWorkSettings
description: Обновление свойств объекта androidForWorkSettings.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: de0100581fab02dcb1d21739e00a022e82adf9c9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941207"
---
# <a name="update-androidforworksettings"></a><span data-ttu-id="10516-103">Update androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="10516-103">Update androidForWorkSettings</span></span>

> <span data-ttu-id="10516-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="10516-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10516-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10516-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10516-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="10516-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10516-107">Обновление свойств объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="10516-107">Update the properties of a [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="10516-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="10516-108">Prerequisites</span></span>
<span data-ttu-id="10516-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10516-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10516-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10516-111">Permission type</span></span>|<span data-ttu-id="10516-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="10516-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10516-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10516-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10516-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10516-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="10516-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10516-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10516-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10516-116">Not supported.</span></span>|
|<span data-ttu-id="10516-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10516-117">Application</span></span>|<span data-ttu-id="10516-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10516-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10516-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10516-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="10516-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10516-120">Request headers</span></span>
|<span data-ttu-id="10516-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10516-121">Header</span></span>|<span data-ttu-id="10516-122">Значение</span><span class="sxs-lookup"><span data-stu-id="10516-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10516-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="10516-123">Authorization</span></span>|<span data-ttu-id="10516-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="10516-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10516-125">Accept</span><span class="sxs-lookup"><span data-stu-id="10516-125">Accept</span></span>|<span data-ttu-id="10516-126">application/json</span><span class="sxs-lookup"><span data-stu-id="10516-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10516-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10516-127">Request body</span></span>
<span data-ttu-id="10516-128">В тексте запроса добавьте представление объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10516-128">In the request body, supply a JSON representation for the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>

<span data-ttu-id="10516-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span><span class="sxs-lookup"><span data-stu-id="10516-129">The following table shows the properties that are required when you create the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md).</span></span>

|<span data-ttu-id="10516-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="10516-130">Property</span></span>|<span data-ttu-id="10516-131">Тип</span><span class="sxs-lookup"><span data-stu-id="10516-131">Type</span></span>|<span data-ttu-id="10516-132">Описание</span><span class="sxs-lookup"><span data-stu-id="10516-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10516-133">id</span><span class="sxs-lookup"><span data-stu-id="10516-133">id</span></span>|<span data-ttu-id="10516-134">String</span><span class="sxs-lookup"><span data-stu-id="10516-134">String</span></span>|<span data-ttu-id="10516-135">Идентификатор параметров Android for Work</span><span class="sxs-lookup"><span data-stu-id="10516-135">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="10516-136">bindStatus</span><span class="sxs-lookup"><span data-stu-id="10516-136">bindStatus</span></span>|[<span data-ttu-id="10516-137">androidForWorkBindStatus</span><span class="sxs-lookup"><span data-stu-id="10516-137">androidForWorkBindStatus</span></span>](../resources/intune-androidforwork-androidforworkbindstatus.md)|<span data-ttu-id="10516-138">Привязка состояния клиента с помощью API EMM Google.</span><span class="sxs-lookup"><span data-stu-id="10516-138">Bind status of the tenant with the Google EMM API.</span></span> <span data-ttu-id="10516-139">Возможные значения: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span><span class="sxs-lookup"><span data-stu-id="10516-139">Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="10516-140">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="10516-140">lastAppSyncDateTime</span></span>|<span data-ttu-id="10516-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10516-141">DateTimeOffset</span></span>|<span data-ttu-id="10516-142">Время завершения последней синхронизации приложения</span><span class="sxs-lookup"><span data-stu-id="10516-142">Last completion time for app sync</span></span>|
|<span data-ttu-id="10516-143">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="10516-143">lastAppSyncStatus</span></span>|[<span data-ttu-id="10516-144">androidForWorkSyncStatus</span><span class="sxs-lookup"><span data-stu-id="10516-144">androidForWorkSyncStatus</span></span>](../resources/intune-androidforwork-androidforworksyncstatus.md)|<span data-ttu-id="10516-145">Результат последней синхронизации приложения.</span><span class="sxs-lookup"><span data-stu-id="10516-145">Last application sync result.</span></span> <span data-ttu-id="10516-146">Возможные значения: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span><span class="sxs-lookup"><span data-stu-id="10516-146">Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="10516-147">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="10516-147">ownerUserPrincipalName</span></span>|<span data-ttu-id="10516-148">String</span><span class="sxs-lookup"><span data-stu-id="10516-148">String</span></span>|<span data-ttu-id="10516-149">UPN владельца, создавшего предприятие</span><span class="sxs-lookup"><span data-stu-id="10516-149">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="10516-150">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="10516-150">ownerOrganizationName</span></span>|<span data-ttu-id="10516-151">String</span><span class="sxs-lookup"><span data-stu-id="10516-151">String</span></span>|<span data-ttu-id="10516-152">Имя организации, используемое при входящей миграции Android for Work</span><span class="sxs-lookup"><span data-stu-id="10516-152">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="10516-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10516-153">lastModifiedDateTime</span></span>|<span data-ttu-id="10516-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10516-154">DateTimeOffset</span></span>|<span data-ttu-id="10516-155">Время последнего изменения параметров Android for Work</span><span class="sxs-lookup"><span data-stu-id="10516-155">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="10516-156">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="10516-156">enrollmentTarget</span></span>|[<span data-ttu-id="10516-157">androidForWorkEnrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="10516-157">androidForWorkEnrollmentTarget</span></span>](../resources/intune-androidforwork-androidforworkenrollmenttarget.md)|<span data-ttu-id="10516-158">Указывает пользователей, которые можно зарегистрировать устройств в Android для управления работой устройства.</span><span class="sxs-lookup"><span data-stu-id="10516-158">Indicates which users can enroll devices in Android for Work device management.</span></span> <span data-ttu-id="10516-159">Возможные значения: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="10516-159">Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="10516-160">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="10516-160">targetGroupIds</span></span>|<span data-ttu-id="10516-161">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="10516-161">String collection</span></span>|<span data-ttu-id="10516-162">Указывает, какие группы AAD могут регистрировать устройства для управления с помощью Android for Work, если для параметра enrollmentTarget задано значение Targeted.</span><span class="sxs-lookup"><span data-stu-id="10516-162">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|
|<span data-ttu-id="10516-163">deviceOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="10516-163">deviceOwnerManagementEnabled</span></span>|<span data-ttu-id="10516-164">Логический</span><span class="sxs-lookup"><span data-stu-id="10516-164">Boolean</span></span>|<span data-ttu-id="10516-165">Указывает, если эта учетная запись flighting для Android владелец управление устройствами с CloudDPC.</span><span class="sxs-lookup"><span data-stu-id="10516-165">Indicates if this account is flighting for Android Device Owner Management with CloudDPC.</span></span>|



## <a name="response"></a><span data-ttu-id="10516-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="10516-166">Response</span></span>
<span data-ttu-id="10516-167">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="10516-167">If successful, this method returns a `200 OK` response code and an updated [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10516-168">Пример</span><span class="sxs-lookup"><span data-stu-id="10516-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="10516-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="10516-169">Request</span></span>
<span data-ttu-id="10516-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10516-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings
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

### <a name="response"></a><span data-ttu-id="10516-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="10516-171">Response</span></span>
<span data-ttu-id="10516-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="10516-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





