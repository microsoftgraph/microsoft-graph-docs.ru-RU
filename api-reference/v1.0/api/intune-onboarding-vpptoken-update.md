---
title: Обновить VPP токен
description: Обновление свойств объекта VPP токен.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0fb6a3024f87295c9cc764279a035040727243a6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52743310"
---
# <a name="update-vpptoken"></a><span data-ttu-id="973a7-103">Обновить VPP токен</span><span class="sxs-lookup"><span data-stu-id="973a7-103">Update vppToken</span></span>

<span data-ttu-id="973a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="973a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="973a7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="973a7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="973a7-106">Обновление свойств объекта [VPP токен](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="973a7-106">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="973a7-107">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="973a7-107">Prerequisites</span></span>
<span data-ttu-id="973a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="973a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="973a7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="973a7-110">Permission type</span></span>|<span data-ttu-id="973a7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="973a7-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="973a7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="973a7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="973a7-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="973a7-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="973a7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="973a7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="973a7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="973a7-115">Not supported.</span></span>|
|<span data-ttu-id="973a7-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="973a7-116">Application</span></span>|<span data-ttu-id="973a7-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="973a7-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="973a7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="973a7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="973a7-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="973a7-119">Request headers</span></span>
|<span data-ttu-id="973a7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="973a7-120">Header</span></span>|<span data-ttu-id="973a7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="973a7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="973a7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="973a7-122">Authorization</span></span>|<span data-ttu-id="973a7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="973a7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="973a7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="973a7-124">Accept</span></span>|<span data-ttu-id="973a7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="973a7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="973a7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="973a7-126">Request body</span></span>
<span data-ttu-id="973a7-127">В тексте запроса добавьте представление объекта [VPP токен](../resources/intune-onboarding-vpptoken.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="973a7-127">In the request body, supply a JSON representation for the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

<span data-ttu-id="973a7-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [VPP токен](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="973a7-128">The following table shows the properties that are required when you create the [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

|<span data-ttu-id="973a7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="973a7-129">Property</span></span>|<span data-ttu-id="973a7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="973a7-130">Type</span></span>|<span data-ttu-id="973a7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="973a7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="973a7-132">id</span><span class="sxs-lookup"><span data-stu-id="973a7-132">id</span></span>|<span data-ttu-id="973a7-133">String</span><span class="sxs-lookup"><span data-stu-id="973a7-133">String</span></span>|<span data-ttu-id="973a7-134">Создается автоматически при создании appleVolumePurchaseProgramToken.</span><span class="sxs-lookup"><span data-stu-id="973a7-134">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="973a7-135">Это ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="973a7-135">It is the Key of the entity.</span></span>|
|<span data-ttu-id="973a7-136">organizationName</span><span class="sxs-lookup"><span data-stu-id="973a7-136">organizationName</span></span>|<span data-ttu-id="973a7-137">Строка</span><span class="sxs-lookup"><span data-stu-id="973a7-137">String</span></span>|<span data-ttu-id="973a7-138">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="973a7-138">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="973a7-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="973a7-139">vppTokenAccountType</span></span>|[<span data-ttu-id="973a7-140">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="973a7-140">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="973a7-141">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="973a7-141">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="973a7-142">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="973a7-142">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="973a7-143">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="973a7-143">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="973a7-144">appleId</span><span class="sxs-lookup"><span data-stu-id="973a7-144">appleId</span></span>|<span data-ttu-id="973a7-145">Строка</span><span class="sxs-lookup"><span data-stu-id="973a7-145">String</span></span>|<span data-ttu-id="973a7-146">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="973a7-146">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="973a7-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="973a7-147">expirationDateTime</span></span>|<span data-ttu-id="973a7-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="973a7-148">DateTimeOffset</span></span>|<span data-ttu-id="973a7-149">Дата и время завершения срока действия токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="973a7-149">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="973a7-150">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="973a7-150">lastSyncDateTime</span></span>|<span data-ttu-id="973a7-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="973a7-151">DateTimeOffset</span></span>|<span data-ttu-id="973a7-152">Последнее выполнение синхронизации приложения при помощи службы Apple Volume Purchase Program с использованием токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="973a7-152">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="973a7-153">токен</span><span class="sxs-lookup"><span data-stu-id="973a7-153">token</span></span>|<span data-ttu-id="973a7-154">Строка</span><span class="sxs-lookup"><span data-stu-id="973a7-154">String</span></span>|<span data-ttu-id="973a7-155">Строка токена Apple Volume Purchase Program; загрузка выполнена из Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="973a7-155">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="973a7-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="973a7-156">lastModifiedDateTime</span></span>|<span data-ttu-id="973a7-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="973a7-157">DateTimeOffset</span></span>|<span data-ttu-id="973a7-158">Дата и время последнего изменения, связанного с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="973a7-158">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="973a7-159">состояние</span><span class="sxs-lookup"><span data-stu-id="973a7-159">state</span></span>|[<span data-ttu-id="973a7-160">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="973a7-160">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="973a7-161">Текущее состояние токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="973a7-161">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="973a7-162">Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="973a7-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="973a7-163">Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="973a7-163">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="973a7-164">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="973a7-164">lastSyncStatus</span></span>|[<span data-ttu-id="973a7-165">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="973a7-165">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="973a7-166">Текущее состояние последней синхронизации приложения, инициированной с помощью токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="973a7-166">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="973a7-167">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="973a7-167">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="973a7-168">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="973a7-168">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="973a7-169">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="973a7-169">automaticallyUpdateApps</span></span>|<span data-ttu-id="973a7-170">Логическое</span><span class="sxs-lookup"><span data-stu-id="973a7-170">Boolean</span></span>|<span data-ttu-id="973a7-171">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="973a7-171">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="973a7-172">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="973a7-172">countryOrRegion</span></span>|<span data-ttu-id="973a7-173">Строка</span><span class="sxs-lookup"><span data-stu-id="973a7-173">String</span></span>|<span data-ttu-id="973a7-174">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="973a7-174">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="973a7-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="973a7-175">Response</span></span>
<span data-ttu-id="973a7-176">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [VPP токен](../resources/intune-onboarding-vpptoken.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="973a7-176">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="973a7-177">Пример</span><span class="sxs-lookup"><span data-stu-id="973a7-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="973a7-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="973a7-178">Request</span></span>
<span data-ttu-id="973a7-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="973a7-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="973a7-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="973a7-180">Response</span></span>
<span data-ttu-id="973a7-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="973a7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




