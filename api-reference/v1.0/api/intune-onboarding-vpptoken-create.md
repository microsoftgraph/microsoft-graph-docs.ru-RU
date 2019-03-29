---
title: Создать VPP токен
description: Создайте новый объект vppToken.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 713a6bf583ff9c315ec88a83811312e6a6af5d92
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980476"
---
# <a name="create-vpptoken"></a><span data-ttu-id="633f0-103">Создать VPP токен</span><span class="sxs-lookup"><span data-stu-id="633f0-103">Create vppToken</span></span>

> <span data-ttu-id="633f0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="633f0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="633f0-105">Создайте новый объект [vppToken](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="633f0-105">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="633f0-106">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="633f0-106">Prerequisites</span></span>
<span data-ttu-id="633f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="633f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="633f0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="633f0-109">Permission type</span></span>|<span data-ttu-id="633f0-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="633f0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="633f0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="633f0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="633f0-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="633f0-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="633f0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="633f0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="633f0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="633f0-114">Not supported.</span></span>|
|<span data-ttu-id="633f0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="633f0-115">Application</span></span>|<span data-ttu-id="633f0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="633f0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="633f0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="633f0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="633f0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="633f0-118">Request headers</span></span>
|<span data-ttu-id="633f0-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="633f0-119">Header</span></span>|<span data-ttu-id="633f0-120">Значение</span><span class="sxs-lookup"><span data-stu-id="633f0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="633f0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="633f0-121">Authorization</span></span>|<span data-ttu-id="633f0-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="633f0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="633f0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="633f0-123">Accept</span></span>|<span data-ttu-id="633f0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="633f0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="633f0-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="633f0-125">Request body</span></span>
<span data-ttu-id="633f0-126">В тексте запроса добавьте представление объекта VPP токен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="633f0-126">In the request body, supply a JSON representation for the vppToken object.</span></span>

<span data-ttu-id="633f0-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта VPP токен.</span><span class="sxs-lookup"><span data-stu-id="633f0-127">The following table shows the properties that are required when you create the vppToken.</span></span>

|<span data-ttu-id="633f0-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="633f0-128">Property</span></span>|<span data-ttu-id="633f0-129">Тип</span><span class="sxs-lookup"><span data-stu-id="633f0-129">Type</span></span>|<span data-ttu-id="633f0-130">Описание</span><span class="sxs-lookup"><span data-stu-id="633f0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="633f0-131">id</span><span class="sxs-lookup"><span data-stu-id="633f0-131">id</span></span>|<span data-ttu-id="633f0-132">String</span><span class="sxs-lookup"><span data-stu-id="633f0-132">String</span></span>|<span data-ttu-id="633f0-133">Создается автоматически при создании appleVolumePurchaseProgramToken.</span><span class="sxs-lookup"><span data-stu-id="633f0-133">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="633f0-134">Это ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="633f0-134">It is the Key of the entity.</span></span>|
|<span data-ttu-id="633f0-135">organizationName</span><span class="sxs-lookup"><span data-stu-id="633f0-135">organizationName</span></span>|<span data-ttu-id="633f0-136">String</span><span class="sxs-lookup"><span data-stu-id="633f0-136">String</span></span>|<span data-ttu-id="633f0-137">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="633f0-137">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="633f0-138">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="633f0-138">vppTokenAccountType</span></span>|[<span data-ttu-id="633f0-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="633f0-139">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="633f0-140">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="633f0-140">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="633f0-141">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="633f0-141">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="633f0-142">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="633f0-142">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="633f0-143">appleId</span><span class="sxs-lookup"><span data-stu-id="633f0-143">appleId</span></span>|<span data-ttu-id="633f0-144">String</span><span class="sxs-lookup"><span data-stu-id="633f0-144">String</span></span>|<span data-ttu-id="633f0-145">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="633f0-145">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="633f0-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="633f0-146">expirationDateTime</span></span>|<span data-ttu-id="633f0-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="633f0-147">DateTimeOffset</span></span>|<span data-ttu-id="633f0-148">Дата и время завершения срока действия токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="633f0-148">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="633f0-149">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="633f0-149">lastSyncDateTime</span></span>|<span data-ttu-id="633f0-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="633f0-150">DateTimeOffset</span></span>|<span data-ttu-id="633f0-151">Последнее выполнение синхронизации приложения при помощи службы Apple Volume Purchase Program с использованием токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="633f0-151">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="633f0-152">токен</span><span class="sxs-lookup"><span data-stu-id="633f0-152">token</span></span>|<span data-ttu-id="633f0-153">String</span><span class="sxs-lookup"><span data-stu-id="633f0-153">String</span></span>|<span data-ttu-id="633f0-154">Строка токена Apple Volume Purchase Program; загрузка выполнена из Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="633f0-154">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="633f0-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="633f0-155">lastModifiedDateTime</span></span>|<span data-ttu-id="633f0-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="633f0-156">DateTimeOffset</span></span>|<span data-ttu-id="633f0-157">Дата и время последнего изменения, связанного с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="633f0-157">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="633f0-158">состояние</span><span class="sxs-lookup"><span data-stu-id="633f0-158">state</span></span>|[<span data-ttu-id="633f0-159">Впптокенстате</span><span class="sxs-lookup"><span data-stu-id="633f0-159">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="633f0-160">Текущее состояние токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="633f0-160">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="633f0-161">Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="633f0-161">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="633f0-162">Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="633f0-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="633f0-163">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="633f0-163">lastSyncStatus</span></span>|[<span data-ttu-id="633f0-164">Впптокенсинкстатус</span><span class="sxs-lookup"><span data-stu-id="633f0-164">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="633f0-165">Текущее состояние последней синхронизации приложения, инициированной с помощью токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="633f0-165">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="633f0-166">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="633f0-166">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="633f0-167">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="633f0-167">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="633f0-168">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="633f0-168">automaticallyUpdateApps</span></span>|<span data-ttu-id="633f0-169">Логическое</span><span class="sxs-lookup"><span data-stu-id="633f0-169">Boolean</span></span>|<span data-ttu-id="633f0-170">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="633f0-170">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="633f0-171">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="633f0-171">countryOrRegion</span></span>|<span data-ttu-id="633f0-172">Строка</span><span class="sxs-lookup"><span data-stu-id="633f0-172">String</span></span>|<span data-ttu-id="633f0-173">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="633f0-173">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="633f0-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="633f0-174">Response</span></span>
<span data-ttu-id="633f0-175">В случае успешного выполнения данный метод возвращает`201 Created` код отклика и объект [vppToken](../resources/intune-onboarding-vpptoken.md) в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="633f0-175">If successful, this method returns a `201 Created` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="633f0-176">Пример</span><span class="sxs-lookup"><span data-stu-id="633f0-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="633f0-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="633f0-177">Request</span></span>
<span data-ttu-id="633f0-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="633f0-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="633f0-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="633f0-179">Response</span></span>
<span data-ttu-id="633f0-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="633f0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



