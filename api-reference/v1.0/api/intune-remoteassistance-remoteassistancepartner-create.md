---
title: Создание объекта remoteAssistancePartner
description: Создание объекта remoteAssistancePartner.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a7f2f73d0b14f13ab7024bd94adf95966b987d83
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984952"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="b32aa-103">Создание объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="b32aa-103">Create remoteAssistancePartner</span></span>

<span data-ttu-id="b32aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b32aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b32aa-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b32aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b32aa-106">Создание объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="b32aa-106">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b32aa-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b32aa-107">Prerequisites</span></span>
<span data-ttu-id="b32aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b32aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b32aa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b32aa-110">Permission type</span></span>|<span data-ttu-id="b32aa-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b32aa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b32aa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b32aa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b32aa-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b32aa-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b32aa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b32aa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b32aa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b32aa-115">Not supported.</span></span>|
|<span data-ttu-id="b32aa-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b32aa-116">Application</span></span>|<span data-ttu-id="b32aa-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b32aa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b32aa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b32aa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="b32aa-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b32aa-119">Request headers</span></span>
|<span data-ttu-id="b32aa-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b32aa-120">Header</span></span>|<span data-ttu-id="b32aa-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b32aa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b32aa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b32aa-122">Authorization</span></span>|<span data-ttu-id="b32aa-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b32aa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b32aa-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b32aa-124">Accept</span></span>|<span data-ttu-id="b32aa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b32aa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b32aa-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b32aa-126">Request body</span></span>
<span data-ttu-id="b32aa-127">В теле запроса добавьте представление объекта remoteAssistancePartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b32aa-127">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="b32aa-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта remoteAssistancePartner.</span><span class="sxs-lookup"><span data-stu-id="b32aa-128">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="b32aa-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b32aa-129">Property</span></span>|<span data-ttu-id="b32aa-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b32aa-130">Type</span></span>|<span data-ttu-id="b32aa-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b32aa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b32aa-132">id</span><span class="sxs-lookup"><span data-stu-id="b32aa-132">id</span></span>|<span data-ttu-id="b32aa-133">String</span><span class="sxs-lookup"><span data-stu-id="b32aa-133">String</span></span>|<span data-ttu-id="b32aa-134">Уникальный идентификатор партнера.</span><span class="sxs-lookup"><span data-stu-id="b32aa-134">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="b32aa-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b32aa-135">displayName</span></span>|<span data-ttu-id="b32aa-136">String</span><span class="sxs-lookup"><span data-stu-id="b32aa-136">String</span></span>|<span data-ttu-id="b32aa-137">Отображаемое имя партнера.</span><span class="sxs-lookup"><span data-stu-id="b32aa-137">Display name of the partner.</span></span>|
|<span data-ttu-id="b32aa-138">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="b32aa-138">onboardingUrl</span></span>|<span data-ttu-id="b32aa-139">String</span><span class="sxs-lookup"><span data-stu-id="b32aa-139">String</span></span>|<span data-ttu-id="b32aa-140">URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="b32aa-140">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="b32aa-141">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="b32aa-141">onboardingStatus</span></span>|[<span data-ttu-id="b32aa-142">ремотеассистанцеонбоардингстатус</span><span class="sxs-lookup"><span data-stu-id="b32aa-142">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="b32aa-143">Подлежит определению.</span><span class="sxs-lookup"><span data-stu-id="b32aa-143">TBD.</span></span> <span data-ttu-id="b32aa-144">Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="b32aa-144">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="b32aa-145">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="b32aa-145">lastConnectionDateTime</span></span>|<span data-ttu-id="b32aa-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b32aa-146">DateTimeOffset</span></span>|<span data-ttu-id="b32aa-147">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="b32aa-147">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="b32aa-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="b32aa-148">Response</span></span>
<span data-ttu-id="b32aa-149">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b32aa-149">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b32aa-150">Пример</span><span class="sxs-lookup"><span data-stu-id="b32aa-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="b32aa-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="b32aa-151">Request</span></span>
<span data-ttu-id="b32aa-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b32aa-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners
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

### <a name="response"></a><span data-ttu-id="b32aa-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="b32aa-153">Response</span></span>
<span data-ttu-id="b32aa-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b32aa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









