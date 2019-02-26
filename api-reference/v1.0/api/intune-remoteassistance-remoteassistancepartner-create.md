---
title: Создание объекта remoteAssistancePartner
description: Создание объекта remoteAssistancePartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 38fe6f752c231e89d3fee9cc4ef9eb4f40121e15
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263772"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="f0f77-103">Создание объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="f0f77-103">Create remoteAssistancePartner</span></span>

> <span data-ttu-id="f0f77-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0f77-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0f77-105">Создание объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="f0f77-105">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0f77-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f0f77-106">Prerequisites</span></span>
<span data-ttu-id="f0f77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f0f77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f0f77-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0f77-109">Permission type</span></span>|<span data-ttu-id="f0f77-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0f77-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0f77-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0f77-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f0f77-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0f77-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f0f77-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0f77-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0f77-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0f77-114">Not supported.</span></span>|
|<span data-ttu-id="f0f77-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0f77-115">Application</span></span>|<span data-ttu-id="f0f77-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0f77-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0f77-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0f77-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="f0f77-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0f77-118">Request headers</span></span>
|<span data-ttu-id="f0f77-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0f77-119">Header</span></span>|<span data-ttu-id="f0f77-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f0f77-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0f77-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0f77-121">Authorization</span></span>|<span data-ttu-id="f0f77-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f0f77-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0f77-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f0f77-123">Accept</span></span>|<span data-ttu-id="f0f77-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f0f77-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0f77-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f0f77-125">Request body</span></span>
<span data-ttu-id="f0f77-126">В теле запроса добавьте представление объекта remoteAssistancePartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0f77-126">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="f0f77-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта remoteAssistancePartner.</span><span class="sxs-lookup"><span data-stu-id="f0f77-127">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="f0f77-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0f77-128">Property</span></span>|<span data-ttu-id="f0f77-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f0f77-129">Type</span></span>|<span data-ttu-id="f0f77-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f0f77-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0f77-131">id</span><span class="sxs-lookup"><span data-stu-id="f0f77-131">id</span></span>|<span data-ttu-id="f0f77-132">Строка</span><span class="sxs-lookup"><span data-stu-id="f0f77-132">String</span></span>|<span data-ttu-id="f0f77-133">Уникальный идентификатор партнера.</span><span class="sxs-lookup"><span data-stu-id="f0f77-133">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="f0f77-134">displayName</span><span class="sxs-lookup"><span data-stu-id="f0f77-134">displayName</span></span>|<span data-ttu-id="f0f77-135">String</span><span class="sxs-lookup"><span data-stu-id="f0f77-135">String</span></span>|<span data-ttu-id="f0f77-136">Отображаемое имя партнера.</span><span class="sxs-lookup"><span data-stu-id="f0f77-136">Display name of the partner.</span></span>|
|<span data-ttu-id="f0f77-137">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="f0f77-137">onboardingUrl</span></span>|<span data-ttu-id="f0f77-138">String</span><span class="sxs-lookup"><span data-stu-id="f0f77-138">String</span></span>|<span data-ttu-id="f0f77-139">URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="f0f77-139">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="f0f77-140">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="f0f77-140">onboardingStatus</span></span>|[<span data-ttu-id="f0f77-141">Ремотеассистанцеонбоардингстатус</span><span class="sxs-lookup"><span data-stu-id="f0f77-141">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="f0f77-142">Подлежит определению.</span><span class="sxs-lookup"><span data-stu-id="f0f77-142">TBD.</span></span> <span data-ttu-id="f0f77-143">Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="f0f77-143">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="f0f77-144">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="f0f77-144">lastConnectionDateTime</span></span>|<span data-ttu-id="f0f77-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0f77-145">DateTimeOffset</span></span>|<span data-ttu-id="f0f77-146">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="f0f77-146">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="f0f77-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0f77-147">Response</span></span>
<span data-ttu-id="f0f77-148">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f0f77-148">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0f77-149">Пример</span><span class="sxs-lookup"><span data-stu-id="f0f77-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0f77-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0f77-150">Request</span></span>
<span data-ttu-id="f0f77-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0f77-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f0f77-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0f77-152">Response</span></span>
<span data-ttu-id="f0f77-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f0f77-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



