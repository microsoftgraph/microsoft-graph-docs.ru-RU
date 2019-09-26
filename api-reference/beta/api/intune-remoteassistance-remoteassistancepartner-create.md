---
title: Создание объекта remoteAssistancePartner
description: Создание объекта remoteAssistancePartner.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a10aade12fcfdbcb1a9b74722c480d52c98aefc1
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194826"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="a7383-103">Создание объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="a7383-103">Create remoteAssistancePartner</span></span>

> <span data-ttu-id="a7383-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7383-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7383-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7383-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7383-106">Создание объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="a7383-106">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7383-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a7383-107">Prerequisites</span></span>
<span data-ttu-id="a7383-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7383-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7383-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7383-110">Permission type</span></span>|<span data-ttu-id="a7383-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7383-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7383-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7383-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a7383-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7383-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a7383-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7383-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7383-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7383-115">Not supported.</span></span>|
|<span data-ttu-id="a7383-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7383-116">Application</span></span>|<span data-ttu-id="a7383-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7383-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7383-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7383-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="a7383-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7383-119">Request headers</span></span>
|<span data-ttu-id="a7383-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7383-120">Header</span></span>|<span data-ttu-id="a7383-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a7383-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7383-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7383-122">Authorization</span></span>|<span data-ttu-id="a7383-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7383-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7383-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a7383-124">Accept</span></span>|<span data-ttu-id="a7383-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a7383-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7383-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a7383-126">Request body</span></span>
<span data-ttu-id="a7383-127">В теле запроса добавьте представление объекта remoteAssistancePartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7383-127">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="a7383-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта remoteAssistancePartner.</span><span class="sxs-lookup"><span data-stu-id="a7383-128">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="a7383-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7383-129">Property</span></span>|<span data-ttu-id="a7383-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a7383-130">Type</span></span>|<span data-ttu-id="a7383-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a7383-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7383-132">id</span><span class="sxs-lookup"><span data-stu-id="a7383-132">id</span></span>|<span data-ttu-id="a7383-133">String</span><span class="sxs-lookup"><span data-stu-id="a7383-133">String</span></span>|<span data-ttu-id="a7383-134">Уникальный идентификатор партнера.</span><span class="sxs-lookup"><span data-stu-id="a7383-134">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="a7383-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a7383-135">displayName</span></span>|<span data-ttu-id="a7383-136">Строка</span><span class="sxs-lookup"><span data-stu-id="a7383-136">String</span></span>|<span data-ttu-id="a7383-137">Отображаемое имя партнера.</span><span class="sxs-lookup"><span data-stu-id="a7383-137">Display name of the partner.</span></span>|
|<span data-ttu-id="a7383-138">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="a7383-138">onboardingUrl</span></span>|<span data-ttu-id="a7383-139">String</span><span class="sxs-lookup"><span data-stu-id="a7383-139">String</span></span>|<span data-ttu-id="a7383-140">URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="a7383-140">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="a7383-141">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="a7383-141">onboardingStatus</span></span>|[<span data-ttu-id="a7383-142">ремотеассистанцеонбоардингстатус</span><span class="sxs-lookup"><span data-stu-id="a7383-142">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="a7383-143">Понятное описание состояния текущего соединителя TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="a7383-143">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="a7383-144">Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="a7383-144">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="a7383-145">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="a7383-145">lastConnectionDateTime</span></span>|<span data-ttu-id="a7383-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7383-146">DateTimeOffset</span></span>|<span data-ttu-id="a7383-147">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="a7383-147">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="a7383-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7383-148">Response</span></span>
<span data-ttu-id="a7383-149">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a7383-149">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7383-150">Пример</span><span class="sxs-lookup"><span data-stu-id="a7383-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7383-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7383-151">Request</span></span>
<span data-ttu-id="a7383-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7383-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners
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

### <a name="response"></a><span data-ttu-id="a7383-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7383-153">Response</span></span>
<span data-ttu-id="a7383-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7383-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




