---
title: Создать VPP токен
description: Создайте новый объект vppToken.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7536e9c78245aecec3acf1985593277007398740
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419837"
---
# <a name="create-vpptoken"></a><span data-ttu-id="3f180-103">Создать VPP токен</span><span class="sxs-lookup"><span data-stu-id="3f180-103">Create vppToken</span></span>

> <span data-ttu-id="3f180-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3f180-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3f180-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f180-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3f180-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f180-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f180-107">Создайте новый объект [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="3f180-107">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f180-108">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="3f180-108">Prerequisites</span></span>
<span data-ttu-id="3f180-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3f180-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3f180-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f180-111">Permission type</span></span>|<span data-ttu-id="3f180-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f180-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f180-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f180-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f180-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f180-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3f180-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f180-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f180-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f180-116">Not supported.</span></span>|
|<span data-ttu-id="3f180-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f180-117">Application</span></span>|<span data-ttu-id="3f180-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f180-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f180-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f180-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="3f180-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f180-120">Request headers</span></span>
|<span data-ttu-id="3f180-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f180-121">Header</span></span>|<span data-ttu-id="3f180-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3f180-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f180-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f180-123">Authorization</span></span>|<span data-ttu-id="3f180-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3f180-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f180-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3f180-125">Accept</span></span>|<span data-ttu-id="3f180-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f180-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f180-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f180-127">Request body</span></span>
<span data-ttu-id="3f180-128">В тексте запроса добавьте представление объекта VPP токен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f180-128">In the request body, supply a JSON representation for the vppToken object.</span></span>

<span data-ttu-id="3f180-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта VPP токен.</span><span class="sxs-lookup"><span data-stu-id="3f180-129">The following table shows the properties that are required when you create the vppToken.</span></span>

|<span data-ttu-id="3f180-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f180-130">Property</span></span>|<span data-ttu-id="3f180-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3f180-131">Type</span></span>|<span data-ttu-id="3f180-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3f180-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f180-133">id</span><span class="sxs-lookup"><span data-stu-id="3f180-133">id</span></span>|<span data-ttu-id="3f180-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3f180-134">String</span></span>|<span data-ttu-id="3f180-135">Автоматически генерируется при создании appleVolumePurchaseProgramToken.</span><span class="sxs-lookup"><span data-stu-id="3f180-135">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="3f180-136">Это ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3f180-136">It is the Key of the entity.</span></span>|
|<span data-ttu-id="3f180-137">organizationName</span><span class="sxs-lookup"><span data-stu-id="3f180-137">organizationName</span></span>|<span data-ttu-id="3f180-138">Строка</span><span class="sxs-lookup"><span data-stu-id="3f180-138">String</span></span>|<span data-ttu-id="3f180-139">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3f180-139">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="3f180-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="3f180-140">vppTokenAccountType</span></span>|[<span data-ttu-id="3f180-141">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="3f180-141">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="3f180-142">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3f180-142">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="3f180-143">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="3f180-143">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="3f180-144">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="3f180-144">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="3f180-145">appleId</span><span class="sxs-lookup"><span data-stu-id="3f180-145">appleId</span></span>|<span data-ttu-id="3f180-146">Строка</span><span class="sxs-lookup"><span data-stu-id="3f180-146">String</span></span>|<span data-ttu-id="3f180-147">Идентификатор Apple ID, связанный с заданным маркером Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3f180-147">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="3f180-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3f180-148">expirationDateTime</span></span>|<span data-ttu-id="3f180-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f180-149">DateTimeOffset</span></span>|<span data-ttu-id="3f180-150">Дата и время завершения срока действия маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3f180-150">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="3f180-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3f180-151">lastSyncDateTime</span></span>|<span data-ttu-id="3f180-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f180-152">DateTimeOffset</span></span>|<span data-ttu-id="3f180-153">Последнее выполнение синхронизации приложения при помощи службы Apple Volume Purchase Program с использованием токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3f180-153">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="3f180-154">токен</span><span class="sxs-lookup"><span data-stu-id="3f180-154">token</span></span>|<span data-ttu-id="3f180-155">Строка</span><span class="sxs-lookup"><span data-stu-id="3f180-155">String</span></span>|<span data-ttu-id="3f180-156">Строка токена Apple Volume Purchase Program; загрузка выполнена из Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3f180-156">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="3f180-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f180-157">lastModifiedDateTime</span></span>|<span data-ttu-id="3f180-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f180-158">DateTimeOffset</span></span>|<span data-ttu-id="3f180-159">Дата и время последнего изменения, связанного с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3f180-159">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="3f180-160">состояние</span><span class="sxs-lookup"><span data-stu-id="3f180-160">state</span></span>|[<span data-ttu-id="3f180-161">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="3f180-161">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="3f180-162">Текущее состояние токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3f180-162">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="3f180-163">Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="3f180-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="3f180-164">Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="3f180-164">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="3f180-165">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="3f180-165">tokenActionResults</span></span>|<span data-ttu-id="3f180-166">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="3f180-166">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="3f180-167">Коллекции состояния действия выполнить на Apple тома покупки программа маркеров.</span><span class="sxs-lookup"><span data-stu-id="3f180-167">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="3f180-168">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="3f180-168">lastSyncStatus</span></span>|[<span data-ttu-id="3f180-169">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="3f180-169">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="3f180-170">Текущее состояние последней синхронизации приложения, инициированной с помощью токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3f180-170">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="3f180-171">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="3f180-171">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="3f180-172">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="3f180-172">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="3f180-173">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="3f180-173">automaticallyUpdateApps</span></span>|<span data-ttu-id="3f180-174">Логическое</span><span class="sxs-lookup"><span data-stu-id="3f180-174">Boolean</span></span>|<span data-ttu-id="3f180-175">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="3f180-175">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="3f180-176">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="3f180-176">countryOrRegion</span></span>|<span data-ttu-id="3f180-177">Строка</span><span class="sxs-lookup"><span data-stu-id="3f180-177">String</span></span>|<span data-ttu-id="3f180-178">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="3f180-178">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="3f180-179">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="3f180-179">dataSharingConsentGranted</span></span>|<span data-ttu-id="3f180-180">Логический</span><span class="sxs-lookup"><span data-stu-id="3f180-180">Boolean</span></span>|<span data-ttu-id="3f180-181">Согласны полномочия для данных, общий доступ для покупки программа корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="3f180-181">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="3f180-182">displayName</span><span class="sxs-lookup"><span data-stu-id="3f180-182">displayName</span></span>|<span data-ttu-id="3f180-183">String</span><span class="sxs-lookup"><span data-stu-id="3f180-183">String</span></span>|<span data-ttu-id="3f180-184">Администратор указанного маркера понятное имя.</span><span class="sxs-lookup"><span data-stu-id="3f180-184">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="3f180-185">locationName</span><span class="sxs-lookup"><span data-stu-id="3f180-185">locationName</span></span>|<span data-ttu-id="3f180-186">String</span><span class="sxs-lookup"><span data-stu-id="3f180-186">String</span></span>|<span data-ttu-id="3f180-187">Маркер расположение, возвращенные Apple VPP.</span><span class="sxs-lookup"><span data-stu-id="3f180-187">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="3f180-188">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="3f180-188">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="3f180-189">Логический</span><span class="sxs-lookup"><span data-stu-id="3f180-189">Boolean</span></span>|<span data-ttu-id="3f180-190">Admin разрешаете разрешить информация по получению маркеров управления из внешнего MDM.</span><span class="sxs-lookup"><span data-stu-id="3f180-190">Admin consent to allow claiming token management from external MDM.</span></span>|
|<span data-ttu-id="3f180-191">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3f180-191">roleScopeTagIds</span></span>|<span data-ttu-id="3f180-192">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3f180-192">String collection</span></span>|<span data-ttu-id="3f180-193">Роль область теги идентификаторов для этой сущности.</span><span class="sxs-lookup"><span data-stu-id="3f180-193">Role Scope Tags IDs assigned to this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="3f180-194">Ответ</span><span class="sxs-lookup"><span data-stu-id="3f180-194">Response</span></span>
<span data-ttu-id="3f180-195">В случае успешного выполнения данный метод возвращает`201 Created` код отклика и объект [vppToken](../resources/intune-onboarding-vpptoken.md) в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="3f180-195">If successful, this method returns a `201 Created` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f180-196">Пример</span><span class="sxs-lookup"><span data-stu-id="3f180-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f180-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f180-197">Request</span></span>
<span data-ttu-id="3f180-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f180-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3f180-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f180-199">Response</span></span>
<span data-ttu-id="3f180-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3f180-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




