---
title: Создать VPP токен
description: Создайте новый объект vppToken.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b4283b7215467f18fb12b626a24f94aedf84af8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147462"
---
# <a name="create-vpptoken"></a><span data-ttu-id="9847d-103">Создать VPP токен</span><span class="sxs-lookup"><span data-stu-id="9847d-103">Create vppToken</span></span>

> <span data-ttu-id="9847d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9847d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9847d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9847d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9847d-106">Создайте новый объект [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="9847d-106">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9847d-107">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="9847d-107">Prerequisites</span></span>
<span data-ttu-id="9847d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9847d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9847d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9847d-110">Permission type</span></span>|<span data-ttu-id="9847d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9847d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9847d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9847d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9847d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9847d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9847d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9847d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9847d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9847d-115">Not supported.</span></span>|
|<span data-ttu-id="9847d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9847d-116">Application</span></span>|<span data-ttu-id="9847d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9847d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9847d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9847d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="9847d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9847d-119">Request headers</span></span>
|<span data-ttu-id="9847d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9847d-120">Header</span></span>|<span data-ttu-id="9847d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9847d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9847d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9847d-122">Authorization</span></span>|<span data-ttu-id="9847d-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9847d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9847d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9847d-124">Accept</span></span>|<span data-ttu-id="9847d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9847d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9847d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9847d-126">Request body</span></span>
<span data-ttu-id="9847d-127">В тексте запроса добавьте представление объекта VPP токен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9847d-127">In the request body, supply a JSON representation for the vppToken object.</span></span>

<span data-ttu-id="9847d-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта VPP токен.</span><span class="sxs-lookup"><span data-stu-id="9847d-128">The following table shows the properties that are required when you create the vppToken.</span></span>

|<span data-ttu-id="9847d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9847d-129">Property</span></span>|<span data-ttu-id="9847d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9847d-130">Type</span></span>|<span data-ttu-id="9847d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9847d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9847d-132">id</span><span class="sxs-lookup"><span data-stu-id="9847d-132">id</span></span>|<span data-ttu-id="9847d-133">String</span><span class="sxs-lookup"><span data-stu-id="9847d-133">String</span></span>|<span data-ttu-id="9847d-134">Автоматически генерируется при создании appleVolumePurchaseProgramToken.</span><span class="sxs-lookup"><span data-stu-id="9847d-134">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="9847d-135">Это ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9847d-135">It is the Key of the entity.</span></span>|
|<span data-ttu-id="9847d-136">organizationName</span><span class="sxs-lookup"><span data-stu-id="9847d-136">organizationName</span></span>|<span data-ttu-id="9847d-137">String</span><span class="sxs-lookup"><span data-stu-id="9847d-137">String</span></span>|<span data-ttu-id="9847d-138">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="9847d-138">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="9847d-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="9847d-139">vppTokenAccountType</span></span>|[<span data-ttu-id="9847d-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="9847d-140">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="9847d-141">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="9847d-141">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="9847d-142">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="9847d-142">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="9847d-143">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="9847d-143">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="9847d-144">appleId</span><span class="sxs-lookup"><span data-stu-id="9847d-144">appleId</span></span>|<span data-ttu-id="9847d-145">String</span><span class="sxs-lookup"><span data-stu-id="9847d-145">String</span></span>|<span data-ttu-id="9847d-146">Идентификатор Apple ID, связанный с заданным маркером Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="9847d-146">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="9847d-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9847d-147">expirationDateTime</span></span>|<span data-ttu-id="9847d-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9847d-148">DateTimeOffset</span></span>|<span data-ttu-id="9847d-149">Дата и время завершения срока действия маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="9847d-149">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="9847d-150">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9847d-150">lastSyncDateTime</span></span>|<span data-ttu-id="9847d-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9847d-151">DateTimeOffset</span></span>|<span data-ttu-id="9847d-152">Последнее выполнение синхронизации приложения при помощи службы Apple Volume Purchase Program с использованием токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="9847d-152">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="9847d-153">токен</span><span class="sxs-lookup"><span data-stu-id="9847d-153">token</span></span>|<span data-ttu-id="9847d-154">String</span><span class="sxs-lookup"><span data-stu-id="9847d-154">String</span></span>|<span data-ttu-id="9847d-155">Строка токена Apple Volume Purchase Program; загрузка выполнена из Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="9847d-155">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="9847d-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9847d-156">lastModifiedDateTime</span></span>|<span data-ttu-id="9847d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9847d-157">DateTimeOffset</span></span>|<span data-ttu-id="9847d-158">Дата и время последнего изменения, связанного с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="9847d-158">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="9847d-159">состояние</span><span class="sxs-lookup"><span data-stu-id="9847d-159">state</span></span>|[<span data-ttu-id="9847d-160">Впптокенстате</span><span class="sxs-lookup"><span data-stu-id="9847d-160">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="9847d-161">Текущее состояние токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="9847d-161">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="9847d-162">Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="9847d-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="9847d-163">Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="9847d-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="9847d-164">Токенактионресултс</span><span class="sxs-lookup"><span data-stu-id="9847d-164">tokenActionResults</span></span>|<span data-ttu-id="9847d-165">Коллекция [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9847d-165">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="9847d-166">Коллекция состояний действий, выполняемых с помощью маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="9847d-166">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="9847d-167">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="9847d-167">lastSyncStatus</span></span>|[<span data-ttu-id="9847d-168">Впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="9847d-168">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="9847d-169">Текущее состояние последней синхронизации приложения, инициированной с помощью токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="9847d-169">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="9847d-170">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="9847d-170">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="9847d-171">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="9847d-171">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="9847d-172">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="9847d-172">automaticallyUpdateApps</span></span>|<span data-ttu-id="9847d-173">Логическое</span><span class="sxs-lookup"><span data-stu-id="9847d-173">Boolean</span></span>|<span data-ttu-id="9847d-174">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="9847d-174">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="9847d-175">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="9847d-175">countryOrRegion</span></span>|<span data-ttu-id="9847d-176">Строка</span><span class="sxs-lookup"><span data-stu-id="9847d-176">String</span></span>|<span data-ttu-id="9847d-177">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="9847d-177">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="9847d-178">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="9847d-178">dataSharingConsentGranted</span></span>|<span data-ttu-id="9847d-179">Логический</span><span class="sxs-lookup"><span data-stu-id="9847d-179">Boolean</span></span>|<span data-ttu-id="9847d-180">Разрешение, предоставленное для предоставления общего доступа к данным с помощью программы Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="9847d-180">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="9847d-181">displayName</span><span class="sxs-lookup"><span data-stu-id="9847d-181">displayName</span></span>|<span data-ttu-id="9847d-182">String</span><span class="sxs-lookup"><span data-stu-id="9847d-182">String</span></span>|<span data-ttu-id="9847d-183">Понятное имя маркера, указанного администратором.</span><span class="sxs-lookup"><span data-stu-id="9847d-183">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="9847d-184">Локатионнаме</span><span class="sxs-lookup"><span data-stu-id="9847d-184">locationName</span></span>|<span data-ttu-id="9847d-185">String</span><span class="sxs-lookup"><span data-stu-id="9847d-185">String</span></span>|<span data-ttu-id="9847d-186">Расположение маркера возвращено от Apple VPP.</span><span class="sxs-lookup"><span data-stu-id="9847d-186">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="9847d-187">Клаимтокенманажементфромекстерналмдм</span><span class="sxs-lookup"><span data-stu-id="9847d-187">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="9847d-188">Логический</span><span class="sxs-lookup"><span data-stu-id="9847d-188">Boolean</span></span>|<span data-ttu-id="9847d-189">Согласие администратора, чтобы разрешить управление маркерами из внешних MDM.</span><span class="sxs-lookup"><span data-stu-id="9847d-189">Admin consent to allow claiming token management from external MDM.</span></span>|
|<span data-ttu-id="9847d-190">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9847d-190">roleScopeTagIds</span></span>|<span data-ttu-id="9847d-191">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9847d-191">String collection</span></span>|<span data-ttu-id="9847d-192">Идентификаторы тегов области ролей, назначенных этой сущности.</span><span class="sxs-lookup"><span data-stu-id="9847d-192">Role Scope Tags IDs assigned to this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="9847d-193">Ответ</span><span class="sxs-lookup"><span data-stu-id="9847d-193">Response</span></span>
<span data-ttu-id="9847d-194">В случае успешного выполнения данный метод возвращает`201 Created` код отклика и объект [vppToken](../resources/intune-onboarding-vpptoken.md) в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="9847d-194">If successful, this method returns a `201 Created` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9847d-195">Пример</span><span class="sxs-lookup"><span data-stu-id="9847d-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="9847d-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="9847d-196">Request</span></span>
<span data-ttu-id="9847d-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9847d-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/vppTokens
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

### <a name="response"></a><span data-ttu-id="9847d-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="9847d-198">Response</span></span>
<span data-ttu-id="9847d-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9847d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




