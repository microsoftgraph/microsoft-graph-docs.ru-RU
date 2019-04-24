---
title: Создание объекта remoteAssistancePartner
description: Создание объекта remoteAssistancePartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f387750fcd06bc2520479b511c24b4ac7ce333dd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585267"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="8d21e-103">Создание объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="8d21e-103">Create remoteAssistancePartner</span></span>

> <span data-ttu-id="8d21e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d21e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d21e-105">Создание объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="8d21e-105">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d21e-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8d21e-106">Prerequisites</span></span>
<span data-ttu-id="8d21e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d21e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d21e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d21e-109">Permission type</span></span>|<span data-ttu-id="8d21e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d21e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d21e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d21e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8d21e-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d21e-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8d21e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d21e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d21e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d21e-114">Not supported.</span></span>|
|<span data-ttu-id="8d21e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d21e-115">Application</span></span>|<span data-ttu-id="8d21e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d21e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d21e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d21e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="8d21e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d21e-118">Request headers</span></span>
|<span data-ttu-id="8d21e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d21e-119">Header</span></span>|<span data-ttu-id="8d21e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8d21e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d21e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d21e-121">Authorization</span></span>|<span data-ttu-id="8d21e-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d21e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d21e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8d21e-123">Accept</span></span>|<span data-ttu-id="8d21e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8d21e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d21e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d21e-125">Request body</span></span>
<span data-ttu-id="8d21e-126">В теле запроса добавьте представление объекта remoteAssistancePartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d21e-126">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="8d21e-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта remoteAssistancePartner.</span><span class="sxs-lookup"><span data-stu-id="8d21e-127">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="8d21e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d21e-128">Property</span></span>|<span data-ttu-id="8d21e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8d21e-129">Type</span></span>|<span data-ttu-id="8d21e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8d21e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d21e-131">id</span><span class="sxs-lookup"><span data-stu-id="8d21e-131">id</span></span>|<span data-ttu-id="8d21e-132">String</span><span class="sxs-lookup"><span data-stu-id="8d21e-132">String</span></span>|<span data-ttu-id="8d21e-133">Уникальный идентификатор партнера.</span><span class="sxs-lookup"><span data-stu-id="8d21e-133">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="8d21e-134">displayName</span><span class="sxs-lookup"><span data-stu-id="8d21e-134">displayName</span></span>|<span data-ttu-id="8d21e-135">Строка</span><span class="sxs-lookup"><span data-stu-id="8d21e-135">String</span></span>|<span data-ttu-id="8d21e-136">Отображаемое имя партнера.</span><span class="sxs-lookup"><span data-stu-id="8d21e-136">Display name of the partner.</span></span>|
|<span data-ttu-id="8d21e-137">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="8d21e-137">onboardingUrl</span></span>|<span data-ttu-id="8d21e-138">String</span><span class="sxs-lookup"><span data-stu-id="8d21e-138">String</span></span>|<span data-ttu-id="8d21e-139">URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="8d21e-139">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="8d21e-140">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="8d21e-140">onboardingStatus</span></span>|[<span data-ttu-id="8d21e-141">Ремотеассистанцеонбоардингстатус</span><span class="sxs-lookup"><span data-stu-id="8d21e-141">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="8d21e-142">Подлежит определению.</span><span class="sxs-lookup"><span data-stu-id="8d21e-142">TBD.</span></span> <span data-ttu-id="8d21e-143">Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="8d21e-143">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="8d21e-144">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="8d21e-144">lastConnectionDateTime</span></span>|<span data-ttu-id="8d21e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d21e-145">DateTimeOffset</span></span>|<span data-ttu-id="8d21e-146">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="8d21e-146">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="8d21e-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d21e-147">Response</span></span>
<span data-ttu-id="8d21e-148">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8d21e-148">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d21e-149">Пример</span><span class="sxs-lookup"><span data-stu-id="8d21e-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d21e-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d21e-150">Request</span></span>
<span data-ttu-id="8d21e-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d21e-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8d21e-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d21e-152">Response</span></span>
<span data-ttu-id="8d21e-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d21e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



