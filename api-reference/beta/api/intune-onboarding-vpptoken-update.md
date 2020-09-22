---
title: Обновить VPP токен
description: Обновление свойств объекта VPP токен.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc14819f731c1823eb6af2bd9ae9897a8d86a7ff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085733"
---
# <a name="update-vpptoken"></a><span data-ttu-id="81535-103">Обновить VPP токен</span><span class="sxs-lookup"><span data-stu-id="81535-103">Update vppToken</span></span>

<span data-ttu-id="81535-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81535-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81535-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81535-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81535-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81535-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81535-107">Обновление свойств объекта [VPP токен](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="81535-107">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81535-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="81535-108">Prerequisites</span></span>
<span data-ttu-id="81535-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81535-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81535-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81535-111">Permission type</span></span>|<span data-ttu-id="81535-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="81535-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81535-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81535-113">Delegated (work or school account)</span></span>|<span data-ttu-id="81535-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81535-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="81535-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81535-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81535-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81535-116">Not supported.</span></span>|
|<span data-ttu-id="81535-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81535-117">Application</span></span>|<span data-ttu-id="81535-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81535-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81535-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81535-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="81535-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="81535-120">Request headers</span></span>
|<span data-ttu-id="81535-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="81535-121">Header</span></span>|<span data-ttu-id="81535-122">Значение</span><span class="sxs-lookup"><span data-stu-id="81535-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81535-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81535-123">Authorization</span></span>|<span data-ttu-id="81535-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81535-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81535-125">Accept</span><span class="sxs-lookup"><span data-stu-id="81535-125">Accept</span></span>|<span data-ttu-id="81535-126">application/json</span><span class="sxs-lookup"><span data-stu-id="81535-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81535-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81535-127">Request body</span></span>
<span data-ttu-id="81535-128">В тексте запроса добавьте представление объекта [VPP токен](../resources/intune-onboarding-vpptoken.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81535-128">In the request body, supply a JSON representation for the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

<span data-ttu-id="81535-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [VPP токен](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="81535-129">The following table shows the properties that are required when you create the [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

|<span data-ttu-id="81535-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="81535-130">Property</span></span>|<span data-ttu-id="81535-131">Тип</span><span class="sxs-lookup"><span data-stu-id="81535-131">Type</span></span>|<span data-ttu-id="81535-132">Описание</span><span class="sxs-lookup"><span data-stu-id="81535-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81535-133">id</span><span class="sxs-lookup"><span data-stu-id="81535-133">id</span></span>|<span data-ttu-id="81535-134">Строка</span><span class="sxs-lookup"><span data-stu-id="81535-134">String</span></span>|<span data-ttu-id="81535-135">Создается автоматически при создании appleVolumePurchaseProgramToken.</span><span class="sxs-lookup"><span data-stu-id="81535-135">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="81535-136">Это ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="81535-136">It is the Key of the entity.</span></span>|
|<span data-ttu-id="81535-137">organizationName</span><span class="sxs-lookup"><span data-stu-id="81535-137">organizationName</span></span>|<span data-ttu-id="81535-138">Строка</span><span class="sxs-lookup"><span data-stu-id="81535-138">String</span></span>|<span data-ttu-id="81535-139">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="81535-139">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="81535-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="81535-140">vppTokenAccountType</span></span>|[<span data-ttu-id="81535-141">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="81535-141">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="81535-142">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="81535-142">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="81535-143">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="81535-143">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="81535-144">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="81535-144">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="81535-145">appleId</span><span class="sxs-lookup"><span data-stu-id="81535-145">appleId</span></span>|<span data-ttu-id="81535-146">Строка</span><span class="sxs-lookup"><span data-stu-id="81535-146">String</span></span>|<span data-ttu-id="81535-147">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="81535-147">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="81535-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="81535-148">expirationDateTime</span></span>|<span data-ttu-id="81535-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81535-149">DateTimeOffset</span></span>|<span data-ttu-id="81535-150">Дата и время завершения срока действия токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="81535-150">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="81535-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="81535-151">lastSyncDateTime</span></span>|<span data-ttu-id="81535-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81535-152">DateTimeOffset</span></span>|<span data-ttu-id="81535-153">Последнее выполнение синхронизации приложения при помощи службы Apple Volume Purchase Program с использованием токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="81535-153">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="81535-154">токен</span><span class="sxs-lookup"><span data-stu-id="81535-154">token</span></span>|<span data-ttu-id="81535-155">Строка</span><span class="sxs-lookup"><span data-stu-id="81535-155">String</span></span>|<span data-ttu-id="81535-156">Строка токена Apple Volume Purchase Program; загрузка выполнена из Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="81535-156">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="81535-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81535-157">lastModifiedDateTime</span></span>|<span data-ttu-id="81535-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81535-158">DateTimeOffset</span></span>|<span data-ttu-id="81535-159">Дата и время последнего изменения, связанного с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="81535-159">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="81535-160">состояние</span><span class="sxs-lookup"><span data-stu-id="81535-160">state</span></span>|[<span data-ttu-id="81535-161">впптокенстате</span><span class="sxs-lookup"><span data-stu-id="81535-161">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="81535-162">Текущее состояние токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="81535-162">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="81535-163">Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="81535-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="81535-164">Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`, `duplicateLocationId`.</span><span class="sxs-lookup"><span data-stu-id="81535-164">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`, `duplicateLocationId`.</span></span>|
|<span data-ttu-id="81535-165">токенактионресултс</span><span class="sxs-lookup"><span data-stu-id="81535-165">tokenActionResults</span></span>|<span data-ttu-id="81535-166">Коллекция [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="81535-166">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="81535-167">Коллекция состояний действий, выполняемых с помощью маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="81535-167">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="81535-168">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="81535-168">lastSyncStatus</span></span>|[<span data-ttu-id="81535-169">впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="81535-169">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="81535-170">Текущее состояние последней синхронизации приложения, инициированной с помощью токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="81535-170">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="81535-171">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="81535-171">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="81535-172">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="81535-172">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="81535-173">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="81535-173">automaticallyUpdateApps</span></span>|<span data-ttu-id="81535-174">Логическое</span><span class="sxs-lookup"><span data-stu-id="81535-174">Boolean</span></span>|<span data-ttu-id="81535-175">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="81535-175">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="81535-176">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="81535-176">countryOrRegion</span></span>|<span data-ttu-id="81535-177">Строка</span><span class="sxs-lookup"><span data-stu-id="81535-177">String</span></span>|<span data-ttu-id="81535-178">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="81535-178">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="81535-179">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="81535-179">dataSharingConsentGranted</span></span>|<span data-ttu-id="81535-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="81535-180">Boolean</span></span>|<span data-ttu-id="81535-181">Разрешение, предоставленное для предоставления общего доступа к данным с помощью программы Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="81535-181">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="81535-182">displayName</span><span class="sxs-lookup"><span data-stu-id="81535-182">displayName</span></span>|<span data-ttu-id="81535-183">Строка</span><span class="sxs-lookup"><span data-stu-id="81535-183">String</span></span>|<span data-ttu-id="81535-184">Понятное имя маркера, указанного администратором.</span><span class="sxs-lookup"><span data-stu-id="81535-184">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="81535-185">локатионнаме</span><span class="sxs-lookup"><span data-stu-id="81535-185">locationName</span></span>|<span data-ttu-id="81535-186">Строка</span><span class="sxs-lookup"><span data-stu-id="81535-186">String</span></span>|<span data-ttu-id="81535-187">Расположение маркера возвращено от Apple VPP.</span><span class="sxs-lookup"><span data-stu-id="81535-187">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="81535-188">клаимтокенманажементфромекстерналмдм</span><span class="sxs-lookup"><span data-stu-id="81535-188">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="81535-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="81535-189">Boolean</span></span>|<span data-ttu-id="81535-190">Согласие администратора, чтобы разрешить управление маркерами из внешних MDM.</span><span class="sxs-lookup"><span data-stu-id="81535-190">Admin consent to allow claiming token management from external MDM.</span></span>|
|<span data-ttu-id="81535-191">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="81535-191">roleScopeTagIds</span></span>|<span data-ttu-id="81535-192">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="81535-192">String collection</span></span>|<span data-ttu-id="81535-193">Идентификаторы тегов области ролей, назначенных этой сущности.</span><span class="sxs-lookup"><span data-stu-id="81535-193">Role Scope Tags IDs assigned to this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="81535-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="81535-194">Response</span></span>
<span data-ttu-id="81535-195">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [VPP токен](../resources/intune-onboarding-vpptoken.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="81535-195">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81535-196">Пример</span><span class="sxs-lookup"><span data-stu-id="81535-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="81535-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="81535-197">Request</span></span>
<span data-ttu-id="81535-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81535-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
Content-type: application/json
Content-length: 1002

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "state": "valid",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value",
  "dataSharingConsentGranted": true,
  "displayName": "Display Name value",
  "locationName": "Location Name value",
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="81535-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="81535-199">Response</span></span>
<span data-ttu-id="81535-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="81535-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1115

{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value",
  "dataSharingConsentGranted": true,
  "displayName": "Display Name value",
  "locationName": "Location Name value",
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```






