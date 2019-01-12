---
title: Обновить VPP токен
description: Обновление свойств объекта VPP токен.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d1e38660c1fa83ced205b0bbcc506303a3968c41
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954150"
---
# <a name="update-vpptoken"></a><span data-ttu-id="fb37f-103">Обновить VPP токен</span><span class="sxs-lookup"><span data-stu-id="fb37f-103">Update vppToken</span></span>

> <span data-ttu-id="fb37f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fb37f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb37f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb37f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb37f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fb37f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb37f-107">Обновление свойств объекта [VPP токен](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="fb37f-107">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb37f-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="fb37f-108">Prerequisites</span></span>
<span data-ttu-id="fb37f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb37f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb37f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb37f-111">Permission type</span></span>|<span data-ttu-id="fb37f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb37f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb37f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb37f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb37f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb37f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fb37f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb37f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb37f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb37f-116">Not supported.</span></span>|
|<span data-ttu-id="fb37f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb37f-117">Application</span></span>|<span data-ttu-id="fb37f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb37f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb37f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb37f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="fb37f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb37f-120">Request headers</span></span>
|<span data-ttu-id="fb37f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb37f-121">Header</span></span>|<span data-ttu-id="fb37f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fb37f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb37f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb37f-123">Authorization</span></span>|<span data-ttu-id="fb37f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fb37f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb37f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb37f-125">Accept</span></span>|<span data-ttu-id="fb37f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb37f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb37f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb37f-127">Request body</span></span>
<span data-ttu-id="fb37f-128">В тексте запроса добавьте представление объекта [VPP токен](../resources/intune-onboarding-vpptoken.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb37f-128">In the request body, supply a JSON representation for the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

<span data-ttu-id="fb37f-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [VPP токен](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="fb37f-129">The following table shows the properties that are required when you create the [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

|<span data-ttu-id="fb37f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb37f-130">Property</span></span>|<span data-ttu-id="fb37f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fb37f-131">Type</span></span>|<span data-ttu-id="fb37f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fb37f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb37f-133">id</span><span class="sxs-lookup"><span data-stu-id="fb37f-133">id</span></span>|<span data-ttu-id="fb37f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fb37f-134">String</span></span>|<span data-ttu-id="fb37f-135">Автоматически генерируется при создании appleVolumePurchaseProgramToken.</span><span class="sxs-lookup"><span data-stu-id="fb37f-135">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="fb37f-136">Это ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fb37f-136">It is the Key of the entity.</span></span>|
|<span data-ttu-id="fb37f-137">organizationName</span><span class="sxs-lookup"><span data-stu-id="fb37f-137">organizationName</span></span>|<span data-ttu-id="fb37f-138">Строка</span><span class="sxs-lookup"><span data-stu-id="fb37f-138">String</span></span>|<span data-ttu-id="fb37f-139">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="fb37f-139">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="fb37f-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="fb37f-140">vppTokenAccountType</span></span>|[<span data-ttu-id="fb37f-141">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="fb37f-141">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="fb37f-142">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="fb37f-142">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="fb37f-143">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="fb37f-143">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="fb37f-144">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="fb37f-144">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="fb37f-145">appleId</span><span class="sxs-lookup"><span data-stu-id="fb37f-145">appleId</span></span>|<span data-ttu-id="fb37f-146">Строка</span><span class="sxs-lookup"><span data-stu-id="fb37f-146">String</span></span>|<span data-ttu-id="fb37f-147">Идентификатор Apple ID, связанный с заданным маркером Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="fb37f-147">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="fb37f-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fb37f-148">expirationDateTime</span></span>|<span data-ttu-id="fb37f-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb37f-149">DateTimeOffset</span></span>|<span data-ttu-id="fb37f-150">Дата и время завершения срока действия маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="fb37f-150">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="fb37f-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="fb37f-151">lastSyncDateTime</span></span>|<span data-ttu-id="fb37f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb37f-152">DateTimeOffset</span></span>|<span data-ttu-id="fb37f-153">Последнее выполнение синхронизации приложения при помощи службы Apple Volume Purchase Program с использованием токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="fb37f-153">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="fb37f-154">токен</span><span class="sxs-lookup"><span data-stu-id="fb37f-154">token</span></span>|<span data-ttu-id="fb37f-155">Строка</span><span class="sxs-lookup"><span data-stu-id="fb37f-155">String</span></span>|<span data-ttu-id="fb37f-156">Строка токена Apple Volume Purchase Program; загрузка выполнена из Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="fb37f-156">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="fb37f-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb37f-157">lastModifiedDateTime</span></span>|<span data-ttu-id="fb37f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb37f-158">DateTimeOffset</span></span>|<span data-ttu-id="fb37f-159">Дата и время последнего изменения, связанного с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="fb37f-159">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="fb37f-160">состояние</span><span class="sxs-lookup"><span data-stu-id="fb37f-160">state</span></span>|[<span data-ttu-id="fb37f-161">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="fb37f-161">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="fb37f-162">Текущее состояние токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="fb37f-162">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="fb37f-163">Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="fb37f-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="fb37f-164">Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="fb37f-164">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="fb37f-165">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="fb37f-165">tokenActionResults</span></span>|<span data-ttu-id="fb37f-166">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="fb37f-166">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="fb37f-167">Коллекции состояния действия выполнить на Apple тома покупки программа маркеров.</span><span class="sxs-lookup"><span data-stu-id="fb37f-167">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="fb37f-168">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="fb37f-168">lastSyncStatus</span></span>|[<span data-ttu-id="fb37f-169">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="fb37f-169">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="fb37f-170">Текущее состояние последней синхронизации приложения, инициированной с помощью токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="fb37f-170">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="fb37f-171">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="fb37f-171">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="fb37f-172">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="fb37f-172">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="fb37f-173">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="fb37f-173">automaticallyUpdateApps</span></span>|<span data-ttu-id="fb37f-174">Логическое</span><span class="sxs-lookup"><span data-stu-id="fb37f-174">Boolean</span></span>|<span data-ttu-id="fb37f-175">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="fb37f-175">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="fb37f-176">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="fb37f-176">countryOrRegion</span></span>|<span data-ttu-id="fb37f-177">Строка</span><span class="sxs-lookup"><span data-stu-id="fb37f-177">String</span></span>|<span data-ttu-id="fb37f-178">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="fb37f-178">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="fb37f-179">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="fb37f-179">dataSharingConsentGranted</span></span>|<span data-ttu-id="fb37f-180">Логический</span><span class="sxs-lookup"><span data-stu-id="fb37f-180">Boolean</span></span>|<span data-ttu-id="fb37f-181">Согласны полномочия для данных, общий доступ для покупки программа корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="fb37f-181">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="fb37f-182">displayName</span><span class="sxs-lookup"><span data-stu-id="fb37f-182">displayName</span></span>|<span data-ttu-id="fb37f-183">Строка</span><span class="sxs-lookup"><span data-stu-id="fb37f-183">String</span></span>|<span data-ttu-id="fb37f-184">Администратор указанного маркера понятное имя.</span><span class="sxs-lookup"><span data-stu-id="fb37f-184">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="fb37f-185">locationName</span><span class="sxs-lookup"><span data-stu-id="fb37f-185">locationName</span></span>|<span data-ttu-id="fb37f-186">Строка</span><span class="sxs-lookup"><span data-stu-id="fb37f-186">String</span></span>|<span data-ttu-id="fb37f-187">Маркер расположение, возвращенные Apple VPP.</span><span class="sxs-lookup"><span data-stu-id="fb37f-187">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="fb37f-188">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="fb37f-188">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="fb37f-189">Логический</span><span class="sxs-lookup"><span data-stu-id="fb37f-189">Boolean</span></span>|<span data-ttu-id="fb37f-190">Admin разрешаете разрешить информация по получению маркеров управления из внешнего MDM.</span><span class="sxs-lookup"><span data-stu-id="fb37f-190">Admin consent to allow claiming token management from external MDM.</span></span>|



## <a name="response"></a><span data-ttu-id="fb37f-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb37f-191">Response</span></span>
<span data-ttu-id="fb37f-192">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [VPP токен](../resources/intune-onboarding-vpptoken.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fb37f-192">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb37f-193">Пример</span><span class="sxs-lookup"><span data-stu-id="fb37f-193">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb37f-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb37f-194">Request</span></span>
<span data-ttu-id="fb37f-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb37f-195">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
Content-type: application/json
Content-length: 957

{
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
  "claimTokenManagementFromExternalMdm": true
}
```

### <a name="response"></a><span data-ttu-id="fb37f-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb37f-196">Response</span></span>
<span data-ttu-id="fb37f-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fb37f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1053

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
  "claimTokenManagementFromExternalMdm": true
}
```





