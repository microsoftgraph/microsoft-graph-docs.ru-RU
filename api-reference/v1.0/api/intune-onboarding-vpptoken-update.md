---
title: Обновить VPP токен
description: Обновление свойств объекта VPP токен.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ca7bd9b6a6ec7bf95c403834a9cb4e392ce3ad7c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362052"
---
# <a name="update-vpptoken"></a><span data-ttu-id="123b1-103">Обновить VPP токен</span><span class="sxs-lookup"><span data-stu-id="123b1-103">Update vppToken</span></span>

> <span data-ttu-id="123b1-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="123b1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="123b1-105">Обновление свойств объекта [VPP токен](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="123b1-105">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="123b1-106">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="123b1-106">Prerequisites</span></span>
<span data-ttu-id="123b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="123b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="123b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="123b1-109">Permission type</span></span>|<span data-ttu-id="123b1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="123b1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="123b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="123b1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="123b1-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="123b1-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="123b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="123b1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="123b1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="123b1-114">Not supported.</span></span>|
|<span data-ttu-id="123b1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="123b1-115">Application</span></span>|<span data-ttu-id="123b1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="123b1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="123b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="123b1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="123b1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="123b1-118">Request headers</span></span>
|<span data-ttu-id="123b1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="123b1-119">Header</span></span>|<span data-ttu-id="123b1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="123b1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="123b1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="123b1-121">Authorization</span></span>|<span data-ttu-id="123b1-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="123b1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="123b1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="123b1-123">Accept</span></span>|<span data-ttu-id="123b1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="123b1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="123b1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="123b1-125">Request body</span></span>
<span data-ttu-id="123b1-126">В тексте запроса добавьте представление объекта [VPP токен](../resources/intune-onboarding-vpptoken.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="123b1-126">In the request body, supply a JSON representation for the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

<span data-ttu-id="123b1-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [VPP токен](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="123b1-127">The following table shows the properties that are required when you create the [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

|<span data-ttu-id="123b1-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="123b1-128">Property</span></span>|<span data-ttu-id="123b1-129">Тип</span><span class="sxs-lookup"><span data-stu-id="123b1-129">Type</span></span>|<span data-ttu-id="123b1-130">Описание</span><span class="sxs-lookup"><span data-stu-id="123b1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="123b1-131">id</span><span class="sxs-lookup"><span data-stu-id="123b1-131">id</span></span>|<span data-ttu-id="123b1-132">String</span><span class="sxs-lookup"><span data-stu-id="123b1-132">String</span></span>|<span data-ttu-id="123b1-133">Создается автоматически при создании appleVolumePurchaseProgramToken.</span><span class="sxs-lookup"><span data-stu-id="123b1-133">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="123b1-134">Это ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="123b1-134">It is the Key of the entity.</span></span>|
|<span data-ttu-id="123b1-135">organizationName</span><span class="sxs-lookup"><span data-stu-id="123b1-135">organizationName</span></span>|<span data-ttu-id="123b1-136">String</span><span class="sxs-lookup"><span data-stu-id="123b1-136">String</span></span>|<span data-ttu-id="123b1-137">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="123b1-137">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="123b1-138">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="123b1-138">vppTokenAccountType</span></span>|[<span data-ttu-id="123b1-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="123b1-139">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="123b1-140">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="123b1-140">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="123b1-141">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="123b1-141">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="123b1-142">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="123b1-142">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="123b1-143">appleId</span><span class="sxs-lookup"><span data-stu-id="123b1-143">appleId</span></span>|<span data-ttu-id="123b1-144">String</span><span class="sxs-lookup"><span data-stu-id="123b1-144">String</span></span>|<span data-ttu-id="123b1-145">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="123b1-145">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="123b1-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="123b1-146">expirationDateTime</span></span>|<span data-ttu-id="123b1-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="123b1-147">DateTimeOffset</span></span>|<span data-ttu-id="123b1-148">Дата и время завершения срока действия токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="123b1-148">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="123b1-149">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="123b1-149">lastSyncDateTime</span></span>|<span data-ttu-id="123b1-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="123b1-150">DateTimeOffset</span></span>|<span data-ttu-id="123b1-151">Время последнего выполнения синхронизации приложения со службой Apple Volume Purchase Program с помощью маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="123b1-151">The last time when an application sync was done with the Apple volume purchase program service using the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="123b1-152">токен</span><span class="sxs-lookup"><span data-stu-id="123b1-152">token</span></span>|<span data-ttu-id="123b1-153">String</span><span class="sxs-lookup"><span data-stu-id="123b1-153">String</span></span>|<span data-ttu-id="123b1-154">Строка токена Apple Volume Purchase Program; загрузка выполнена из Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="123b1-154">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="123b1-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="123b1-155">lastModifiedDateTime</span></span>|<span data-ttu-id="123b1-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="123b1-156">DateTimeOffset</span></span>|<span data-ttu-id="123b1-157">Дата и время последнего изменения, связанного с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="123b1-157">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="123b1-158">состояние</span><span class="sxs-lookup"><span data-stu-id="123b1-158">state</span></span>|[<span data-ttu-id="123b1-159">впптокенстате</span><span class="sxs-lookup"><span data-stu-id="123b1-159">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="123b1-160">Текущее состояние токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="123b1-160">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="123b1-161">Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="123b1-161">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="123b1-162">Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="123b1-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="123b1-163">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="123b1-163">lastSyncStatus</span></span>|[<span data-ttu-id="123b1-164">впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="123b1-164">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="123b1-165">Текущее состояние последней синхронизации приложения, инициированной с помощью токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="123b1-165">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="123b1-166">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="123b1-166">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="123b1-167">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="123b1-167">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="123b1-168">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="123b1-168">automaticallyUpdateApps</span></span>|<span data-ttu-id="123b1-169">Логическое</span><span class="sxs-lookup"><span data-stu-id="123b1-169">Boolean</span></span>|<span data-ttu-id="123b1-170">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="123b1-170">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="123b1-171">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="123b1-171">countryOrRegion</span></span>|<span data-ttu-id="123b1-172">Строка</span><span class="sxs-lookup"><span data-stu-id="123b1-172">String</span></span>|<span data-ttu-id="123b1-173">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="123b1-173">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="123b1-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="123b1-174">Response</span></span>
<span data-ttu-id="123b1-175">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [VPP токен](../resources/intune-onboarding-vpptoken.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="123b1-175">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="123b1-176">Пример</span><span class="sxs-lookup"><span data-stu-id="123b1-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="123b1-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="123b1-177">Request</span></span>
<span data-ttu-id="123b1-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="123b1-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}
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

### <a name="response"></a><span data-ttu-id="123b1-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="123b1-179">Response</span></span>
<span data-ttu-id="123b1-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="123b1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




