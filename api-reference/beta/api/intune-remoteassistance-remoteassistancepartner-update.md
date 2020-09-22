---
title: Обновление объекта remoteAssistancePartner
description: Обновление свойств объекта remoteAssistancePartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 81367f2ef3789dacafa0dfc3f06754cd4a53a1c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010859"
---
# <a name="update-remoteassistancepartner"></a><span data-ttu-id="1fbc1-103">Обновление объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1fbc1-103">Update remoteAssistancePartner</span></span>

<span data-ttu-id="1fbc1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fbc1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1fbc1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fbc1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fbc1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1fbc1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fbc1-107">Обновление свойств объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="1fbc1-107">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fbc1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1fbc1-108">Prerequisites</span></span>
<span data-ttu-id="1fbc1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fbc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fbc1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fbc1-111">Permission type</span></span>|<span data-ttu-id="1fbc1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fbc1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fbc1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fbc1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1fbc1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fbc1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1fbc1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fbc1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fbc1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fbc1-116">Not supported.</span></span>|
|<span data-ttu-id="1fbc1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1fbc1-117">Application</span></span>|<span data-ttu-id="1fbc1-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fbc1-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fbc1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fbc1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="1fbc1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1fbc1-120">Request headers</span></span>
|<span data-ttu-id="1fbc1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1fbc1-121">Header</span></span>|<span data-ttu-id="1fbc1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1fbc1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fbc1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fbc1-123">Authorization</span></span>|<span data-ttu-id="1fbc1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fbc1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fbc1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1fbc1-125">Accept</span></span>|<span data-ttu-id="1fbc1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1fbc1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fbc1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1fbc1-127">Request body</span></span>
<span data-ttu-id="1fbc1-128">В теле запроса добавьте представление объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1fbc1-128">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="1fbc1-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="1fbc1-129">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

|<span data-ttu-id="1fbc1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1fbc1-130">Property</span></span>|<span data-ttu-id="1fbc1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1fbc1-131">Type</span></span>|<span data-ttu-id="1fbc1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1fbc1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fbc1-133">id</span><span class="sxs-lookup"><span data-stu-id="1fbc1-133">id</span></span>|<span data-ttu-id="1fbc1-134">String</span><span class="sxs-lookup"><span data-stu-id="1fbc1-134">String</span></span>|<span data-ttu-id="1fbc1-135">Уникальный идентификатор партнера.</span><span class="sxs-lookup"><span data-stu-id="1fbc1-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="1fbc1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1fbc1-136">displayName</span></span>|<span data-ttu-id="1fbc1-137">String</span><span class="sxs-lookup"><span data-stu-id="1fbc1-137">String</span></span>|<span data-ttu-id="1fbc1-138">Отображаемое имя партнера.</span><span class="sxs-lookup"><span data-stu-id="1fbc1-138">Display name of the partner.</span></span>|
|<span data-ttu-id="1fbc1-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="1fbc1-139">onboardingUrl</span></span>|<span data-ttu-id="1fbc1-140">String</span><span class="sxs-lookup"><span data-stu-id="1fbc1-140">String</span></span>|<span data-ttu-id="1fbc1-141">URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="1fbc1-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="1fbc1-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="1fbc1-142">onboardingStatus</span></span>|[<span data-ttu-id="1fbc1-143">ремотеассистанцеонбоардингстатус</span><span class="sxs-lookup"><span data-stu-id="1fbc1-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="1fbc1-144">Понятное описание состояния текущего соединителя TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="1fbc1-144">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="1fbc1-145">Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="1fbc1-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="1fbc1-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="1fbc1-146">lastConnectionDateTime</span></span>|<span data-ttu-id="1fbc1-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fbc1-147">DateTimeOffset</span></span>|<span data-ttu-id="1fbc1-148">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="1fbc1-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|
|<span data-ttu-id="1fbc1-149">онбоардингрекуестекспиридатетиме</span><span class="sxs-lookup"><span data-stu-id="1fbc1-149">onboardingRequestExpiryDateTime</span></span>|<span data-ttu-id="1fbc1-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fbc1-150">DateTimeOffset</span></span>|<span data-ttu-id="1fbc1-151">Когда свойства onboardingstatus является входящей миграцией, это дата и время истечения срока действия запроса на приподключение.</span><span class="sxs-lookup"><span data-stu-id="1fbc1-151">When the OnboardingStatus is Onboarding, This is the date time when the onboarding request expires.</span></span>|



## <a name="response"></a><span data-ttu-id="1fbc1-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fbc1-152">Response</span></span>
<span data-ttu-id="1fbc1-153">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1fbc1-153">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fbc1-154">Пример</span><span class="sxs-lookup"><span data-stu-id="1fbc1-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fbc1-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fbc1-155">Request</span></span>
<span data-ttu-id="1fbc1-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1fbc1-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
Content-type: application/json
Content-length: 341

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "onboardingRequestExpiryDateTime": "2017-01-01T00:02:07.7573274-08:00"
}
```

### <a name="response"></a><span data-ttu-id="1fbc1-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fbc1-157">Response</span></span>
<span data-ttu-id="1fbc1-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1fbc1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 390

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "onboardingRequestExpiryDateTime": "2017-01-01T00:02:07.7573274-08:00"
}
```






