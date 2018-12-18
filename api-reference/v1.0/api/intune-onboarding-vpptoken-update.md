---
title: Обновить VPP токен
description: Обновление свойств объекта VPP токен.
author: tfitzmac
ms.openlocfilehash: 56829adcba15ca1c46e5548212e71e619e339a1a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349002"
---
# <a name="update-vpptoken"></a><span data-ttu-id="ba37c-103">Обновить VPP токен</span><span class="sxs-lookup"><span data-stu-id="ba37c-103">Update vppToken</span></span>

> <span data-ttu-id="ba37c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ba37c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ba37c-105">Обновление свойств объекта [VPP токен](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="ba37c-105">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ba37c-106">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="ba37c-106">Prerequisites</span></span>
<span data-ttu-id="ba37c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba37c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba37c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba37c-109">Permission type</span></span>|<span data-ttu-id="ba37c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba37c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba37c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba37c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ba37c-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba37c-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ba37c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba37c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba37c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba37c-114">Not supported.</span></span>|
|<span data-ttu-id="ba37c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba37c-115">Application</span></span>|<span data-ttu-id="ba37c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba37c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba37c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba37c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="ba37c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba37c-118">Request headers</span></span>
|<span data-ttu-id="ba37c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba37c-119">Header</span></span>|<span data-ttu-id="ba37c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ba37c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba37c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba37c-121">Authorization</span></span>|<span data-ttu-id="ba37c-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ba37c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba37c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ba37c-123">Accept</span></span>|<span data-ttu-id="ba37c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ba37c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba37c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba37c-125">Request body</span></span>
<span data-ttu-id="ba37c-126">В тексте запроса добавьте представление объекта [VPP токен](../resources/intune-onboarding-vpptoken.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba37c-126">In the request body, supply a JSON representation for the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>

<span data-ttu-id="ba37c-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [VPP токен](../resources/intune-onboarding-vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="ba37c-127">The following table shows the properties that are required when you create the [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>

|<span data-ttu-id="ba37c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba37c-128">Property</span></span>|<span data-ttu-id="ba37c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ba37c-129">Type</span></span>|<span data-ttu-id="ba37c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ba37c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba37c-131">id</span><span class="sxs-lookup"><span data-stu-id="ba37c-131">id</span></span>|<span data-ttu-id="ba37c-132">Строка</span><span class="sxs-lookup"><span data-stu-id="ba37c-132">String</span></span>|<span data-ttu-id="ba37c-133">Автоматически генерируется при создании appleVolumePurchaseProgramToken.</span><span class="sxs-lookup"><span data-stu-id="ba37c-133">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="ba37c-134">Это ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ba37c-134">It is the Key of the entity.</span></span>|
|<span data-ttu-id="ba37c-135">organizationName</span><span class="sxs-lookup"><span data-stu-id="ba37c-135">organizationName</span></span>|<span data-ttu-id="ba37c-136">Строка</span><span class="sxs-lookup"><span data-stu-id="ba37c-136">String</span></span>|<span data-ttu-id="ba37c-137">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ba37c-137">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="ba37c-138">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="ba37c-138">vppTokenAccountType</span></span>|[<span data-ttu-id="ba37c-139">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="ba37c-139">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="ba37c-140">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ba37c-140">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="ba37c-141">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="ba37c-141">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="ba37c-142">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="ba37c-142">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="ba37c-143">appleId</span><span class="sxs-lookup"><span data-stu-id="ba37c-143">appleId</span></span>|<span data-ttu-id="ba37c-144">Строка</span><span class="sxs-lookup"><span data-stu-id="ba37c-144">String</span></span>|<span data-ttu-id="ba37c-145">Идентификатор Apple ID, связанный с заданным маркером Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ba37c-145">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ba37c-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ba37c-146">expirationDateTime</span></span>|<span data-ttu-id="ba37c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba37c-147">DateTimeOffset</span></span>|<span data-ttu-id="ba37c-148">Дата и время завершения срока действия маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ba37c-148">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ba37c-149">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ba37c-149">lastSyncDateTime</span></span>|<span data-ttu-id="ba37c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba37c-150">DateTimeOffset</span></span>|<span data-ttu-id="ba37c-151">Последнее выполнение синхронизации приложения при помощи службы Apple Volume Purchase Program с использованием токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ba37c-151">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ba37c-152">токен</span><span class="sxs-lookup"><span data-stu-id="ba37c-152">token</span></span>|<span data-ttu-id="ba37c-153">Строка</span><span class="sxs-lookup"><span data-stu-id="ba37c-153">String</span></span>|<span data-ttu-id="ba37c-154">Строка токена Apple Volume Purchase Program; загрузка выполнена из Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ba37c-154">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="ba37c-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba37c-155">lastModifiedDateTime</span></span>|<span data-ttu-id="ba37c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba37c-156">DateTimeOffset</span></span>|<span data-ttu-id="ba37c-157">Дата и время последнего изменения, связанного с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ba37c-157">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ba37c-158">состояние</span><span class="sxs-lookup"><span data-stu-id="ba37c-158">state</span></span>|[<span data-ttu-id="ba37c-159">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="ba37c-159">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="ba37c-160">Текущее состояние токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ba37c-160">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="ba37c-161">Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="ba37c-161">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="ba37c-162">Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span><span class="sxs-lookup"><span data-stu-id="ba37c-162">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="ba37c-163">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="ba37c-163">lastSyncStatus</span></span>|[<span data-ttu-id="ba37c-164">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="ba37c-164">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="ba37c-165">Текущее состояние последней синхронизации приложения, инициированной с помощью токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ba37c-165">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="ba37c-166">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="ba37c-166">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="ba37c-167">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="ba37c-167">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="ba37c-168">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="ba37c-168">automaticallyUpdateApps</span></span>|<span data-ttu-id="ba37c-169">Логическое</span><span class="sxs-lookup"><span data-stu-id="ba37c-169">Boolean</span></span>|<span data-ttu-id="ba37c-170">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="ba37c-170">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="ba37c-171">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="ba37c-171">countryOrRegion</span></span>|<span data-ttu-id="ba37c-172">Строка</span><span class="sxs-lookup"><span data-stu-id="ba37c-172">String</span></span>|<span data-ttu-id="ba37c-173">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="ba37c-173">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="ba37c-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba37c-174">Response</span></span>
<span data-ttu-id="ba37c-175">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [VPP токен](../resources/intune-onboarding-vpptoken.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba37c-175">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune-onboarding-vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba37c-176">Пример</span><span class="sxs-lookup"><span data-stu-id="ba37c-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="ba37c-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba37c-177">Request</span></span>
<span data-ttu-id="ba37c-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba37c-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ba37c-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="ba37c-179">Response</span></span>
<span data-ttu-id="ba37c-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ba37c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



