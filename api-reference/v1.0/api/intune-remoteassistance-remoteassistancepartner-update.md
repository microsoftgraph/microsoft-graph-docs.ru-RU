---
title: Обновление объекта remoteAssistancePartner
description: Обновление свойств объекта remoteAssistancePartner.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 40a21ce7c0e5cf8ad525dfa44ffc8a6657c7cf13
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512141"
---
# <a name="update-remoteassistancepartner"></a><span data-ttu-id="81ae7-103">Обновление объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="81ae7-103">Update remoteAssistancePartner</span></span>

<span data-ttu-id="81ae7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81ae7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81ae7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81ae7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81ae7-106">Обновление свойств объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="81ae7-106">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81ae7-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="81ae7-107">Prerequisites</span></span>
<span data-ttu-id="81ae7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81ae7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81ae7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81ae7-110">Permission type</span></span>|<span data-ttu-id="81ae7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="81ae7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81ae7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81ae7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="81ae7-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81ae7-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="81ae7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81ae7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81ae7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81ae7-115">Not supported.</span></span>|
|<span data-ttu-id="81ae7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81ae7-116">Application</span></span>|<span data-ttu-id="81ae7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81ae7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81ae7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81ae7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="81ae7-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="81ae7-119">Request headers</span></span>
|<span data-ttu-id="81ae7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="81ae7-120">Header</span></span>|<span data-ttu-id="81ae7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="81ae7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81ae7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="81ae7-122">Authorization</span></span>|<span data-ttu-id="81ae7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81ae7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81ae7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="81ae7-124">Accept</span></span>|<span data-ttu-id="81ae7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="81ae7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81ae7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81ae7-126">Request body</span></span>
<span data-ttu-id="81ae7-127">В теле запроса добавьте представление объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81ae7-127">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="81ae7-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="81ae7-128">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

|<span data-ttu-id="81ae7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="81ae7-129">Property</span></span>|<span data-ttu-id="81ae7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="81ae7-130">Type</span></span>|<span data-ttu-id="81ae7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="81ae7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81ae7-132">id</span><span class="sxs-lookup"><span data-stu-id="81ae7-132">id</span></span>|<span data-ttu-id="81ae7-133">String</span><span class="sxs-lookup"><span data-stu-id="81ae7-133">String</span></span>|<span data-ttu-id="81ae7-134">Уникальный идентификатор партнера.</span><span class="sxs-lookup"><span data-stu-id="81ae7-134">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="81ae7-135">displayName</span><span class="sxs-lookup"><span data-stu-id="81ae7-135">displayName</span></span>|<span data-ttu-id="81ae7-136">Строка</span><span class="sxs-lookup"><span data-stu-id="81ae7-136">String</span></span>|<span data-ttu-id="81ae7-137">Отображаемое имя партнера.</span><span class="sxs-lookup"><span data-stu-id="81ae7-137">Display name of the partner.</span></span>|
|<span data-ttu-id="81ae7-138">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="81ae7-138">onboardingUrl</span></span>|<span data-ttu-id="81ae7-139">String</span><span class="sxs-lookup"><span data-stu-id="81ae7-139">String</span></span>|<span data-ttu-id="81ae7-140">URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="81ae7-140">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="81ae7-141">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="81ae7-141">onboardingStatus</span></span>|[<span data-ttu-id="81ae7-142">ремотеассистанцеонбоардингстатус</span><span class="sxs-lookup"><span data-stu-id="81ae7-142">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="81ae7-143">Подлежит определению.</span><span class="sxs-lookup"><span data-stu-id="81ae7-143">TBD.</span></span> <span data-ttu-id="81ae7-144">Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="81ae7-144">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="81ae7-145">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="81ae7-145">lastConnectionDateTime</span></span>|<span data-ttu-id="81ae7-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81ae7-146">DateTimeOffset</span></span>|<span data-ttu-id="81ae7-147">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="81ae7-147">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="81ae7-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="81ae7-148">Response</span></span>
<span data-ttu-id="81ae7-149">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="81ae7-149">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81ae7-150">Пример</span><span class="sxs-lookup"><span data-stu-id="81ae7-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="81ae7-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="81ae7-151">Request</span></span>
<span data-ttu-id="81ae7-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81ae7-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="81ae7-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="81ae7-153">Response</span></span>
<span data-ttu-id="81ae7-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="81ae7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 315

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```




