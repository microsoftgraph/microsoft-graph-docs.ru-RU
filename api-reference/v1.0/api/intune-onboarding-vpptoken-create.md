---
title: Создать VPP токен
description: Создайте новый объект vppToken.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e9c4bde3521fded68ff4a394929b30128f146f53
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452859"
---
# <a name="create-vpptoken"></a><span data-ttu-id="6edce-103">Создать VPP токен</span><span class="sxs-lookup"><span data-stu-id="6edce-103">Create vppToken</span></span>

<span data-ttu-id="6edce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6edce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6edce-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6edce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6edce-106">Создайте новый объект [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="6edce-106">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6edce-107">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="6edce-107">Prerequisites</span></span>
<span data-ttu-id="6edce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6edce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6edce-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6edce-110">Permission type</span></span>|<span data-ttu-id="6edce-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6edce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6edce-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6edce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6edce-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6edce-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6edce-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6edce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6edce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6edce-115">Not supported.</span></span>|
|<span data-ttu-id="6edce-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6edce-116">Application</span></span>|<span data-ttu-id="6edce-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6edce-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6edce-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6edce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="6edce-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6edce-119">Request headers</span></span>
|<span data-ttu-id="6edce-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6edce-120">Header</span></span>|<span data-ttu-id="6edce-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6edce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6edce-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6edce-122">Authorization</span></span>|<span data-ttu-id="6edce-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6edce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6edce-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6edce-124">Accept</span></span>|<span data-ttu-id="6edce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6edce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6edce-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6edce-126">Request body</span></span>
<span data-ttu-id="6edce-127">В тексте запроса добавьте представление объекта VPP токен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6edce-127">In the request body, supply a JSON representation for the vppToken object.</span></span>

<span data-ttu-id="6edce-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта VPP токен.</span><span class="sxs-lookup"><span data-stu-id="6edce-128">The following table shows the properties that are required when you create the vppToken.</span></span>

|<span data-ttu-id="6edce-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6edce-129">Property</span></span>|<span data-ttu-id="6edce-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6edce-130">Type</span></span>|<span data-ttu-id="6edce-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6edce-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6edce-132">id</span><span class="sxs-lookup"><span data-stu-id="6edce-132">id</span></span>|<span data-ttu-id="6edce-133">String</span><span class="sxs-lookup"><span data-stu-id="6edce-133">String</span></span>|<span data-ttu-id="6edce-134">Создается автоматически при создании appleVolumePurchaseProgramToken.</span><span class="sxs-lookup"><span data-stu-id="6edce-134">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="6edce-135">Это ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6edce-135">It is the Key of the entity.</span></span>|
|<span data-ttu-id="6edce-136">organizationName</span><span class="sxs-lookup"><span data-stu-id="6edce-136">organizationName</span></span>|<span data-ttu-id="6edce-137">String</span><span class="sxs-lookup"><span data-stu-id="6edce-137">String</span></span>|<span data-ttu-id="6edce-138">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="6edce-138">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="6edce-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="6edce-139">vppTokenAccountType</span></span>|[<span data-ttu-id="6edce-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="6edce-140">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="6edce-141">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="6edce-141">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="6edce-142">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="6edce-142">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="6edce-143">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="6edce-143">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="6edce-144">appleId</span><span class="sxs-lookup"><span data-stu-id="6edce-144">appleId</span></span>|<span data-ttu-id="6edce-145">String</span><span class="sxs-lookup"><span data-stu-id="6edce-145">String</span></span>|<span data-ttu-id="6edce-146">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="6edce-146">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="6edce-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6edce-147">expirationDateTime</span></span>|<span data-ttu-id="6edce-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6edce-148">DateTimeOffset</span></span>|<span data-ttu-id="6edce-149">Дата и время завершения срока действия токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="6edce-149">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="6edce-150">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6edce-150">lastSyncDateTime</span></span>|<span data-ttu-id="6edce-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6edce-151">DateTimeOffset</span></span>|<span data-ttu-id="6edce-152">Время последнего выполнения синхронизации приложения со службой Apple Volume Purchase Program с помощью маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="6edce-152">The last time when an application sync was done with the Apple volume purchase program service using the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="6edce-153">токен</span><span class="sxs-lookup"><span data-stu-id="6edce-153">token</span></span>|<span data-ttu-id="6edce-154">String</span><span class="sxs-lookup"><span data-stu-id="6edce-154">String</span></span>|<span data-ttu-id="6edce-155">Строка токена Apple Volume Purchase Program; загрузка выполнена из Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="6edce-155">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="6edce-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6edce-156">lastModifiedDateTime</span></span>|<span data-ttu-id="6edce-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6edce-157">DateTimeOffset</span></span>|<span data-ttu-id="6edce-158">Дата и время последнего изменения, связанного с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="6edce-158">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="6edce-159">состояние</span><span class="sxs-lookup"><span data-stu-id="6edce-159">state</span></span>|[<span data-ttu-id="6edce-160">впптокенстате</span><span class="sxs-lookup"><span data-stu-id="6edce-160">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="6edce-161">Текущее состояние токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="6edce-161">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="6edce-162">Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="6edce-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="6edce-163">Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="6edce-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="6edce-164">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="6edce-164">lastSyncStatus</span></span>|[<span data-ttu-id="6edce-165">впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="6edce-165">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="6edce-166">Текущее состояние последней синхронизации приложения, инициированной с помощью токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="6edce-166">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="6edce-167">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="6edce-167">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="6edce-168">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="6edce-168">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="6edce-169">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="6edce-169">automaticallyUpdateApps</span></span>|<span data-ttu-id="6edce-170">Логическое</span><span class="sxs-lookup"><span data-stu-id="6edce-170">Boolean</span></span>|<span data-ttu-id="6edce-171">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="6edce-171">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="6edce-172">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="6edce-172">countryOrRegion</span></span>|<span data-ttu-id="6edce-173">Строка</span><span class="sxs-lookup"><span data-stu-id="6edce-173">String</span></span>|<span data-ttu-id="6edce-174">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="6edce-174">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="6edce-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="6edce-175">Response</span></span>
<span data-ttu-id="6edce-176">В случае успешного выполнения данный метод возвращает`201 Created` код отклика и объект [vppToken](../resources/intune-onboarding-vpptoken.md) в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="6edce-176">If successful, this method returns a `201 Created` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6edce-177">Пример</span><span class="sxs-lookup"><span data-stu-id="6edce-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="6edce-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="6edce-178">Request</span></span>
<span data-ttu-id="6edce-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6edce-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens
Content-type: application/json
Content-length: 461

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```

### <a name="response"></a><span data-ttu-id="6edce-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="6edce-180">Response</span></span>
<span data-ttu-id="6edce-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6edce-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 574

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
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```






