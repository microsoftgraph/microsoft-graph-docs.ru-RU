---
title: Создание объекта remoteAssistancePartner
description: Создание объекта remoteAssistancePartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 025d2a0b9d4e882c3f6cb55948eb95625909fcf9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140672"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="12a54-103">Создание объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="12a54-103">Create remoteAssistancePartner</span></span>

> <span data-ttu-id="12a54-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12a54-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12a54-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12a54-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12a54-106">Создание объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="12a54-106">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12a54-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="12a54-107">Prerequisites</span></span>
<span data-ttu-id="12a54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="12a54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="12a54-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12a54-110">Permission type</span></span>|<span data-ttu-id="12a54-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12a54-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12a54-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12a54-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12a54-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12a54-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="12a54-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12a54-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12a54-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12a54-115">Not supported.</span></span>|
|<span data-ttu-id="12a54-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12a54-116">Application</span></span>|<span data-ttu-id="12a54-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12a54-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12a54-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12a54-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="12a54-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12a54-119">Request headers</span></span>
|<span data-ttu-id="12a54-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12a54-120">Header</span></span>|<span data-ttu-id="12a54-121">Значение</span><span class="sxs-lookup"><span data-stu-id="12a54-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12a54-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="12a54-122">Authorization</span></span>|<span data-ttu-id="12a54-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="12a54-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12a54-124">Accept</span><span class="sxs-lookup"><span data-stu-id="12a54-124">Accept</span></span>|<span data-ttu-id="12a54-125">application/json</span><span class="sxs-lookup"><span data-stu-id="12a54-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12a54-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="12a54-126">Request body</span></span>
<span data-ttu-id="12a54-127">В теле запроса добавьте представление объекта remoteAssistancePartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12a54-127">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="12a54-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта remoteAssistancePartner.</span><span class="sxs-lookup"><span data-stu-id="12a54-128">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="12a54-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="12a54-129">Property</span></span>|<span data-ttu-id="12a54-130">Тип</span><span class="sxs-lookup"><span data-stu-id="12a54-130">Type</span></span>|<span data-ttu-id="12a54-131">Описание</span><span class="sxs-lookup"><span data-stu-id="12a54-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12a54-132">id</span><span class="sxs-lookup"><span data-stu-id="12a54-132">id</span></span>|<span data-ttu-id="12a54-133">Строка</span><span class="sxs-lookup"><span data-stu-id="12a54-133">String</span></span>|<span data-ttu-id="12a54-134">Уникальный идентификатор партнера.</span><span class="sxs-lookup"><span data-stu-id="12a54-134">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="12a54-135">displayName</span><span class="sxs-lookup"><span data-stu-id="12a54-135">displayName</span></span>|<span data-ttu-id="12a54-136">String</span><span class="sxs-lookup"><span data-stu-id="12a54-136">String</span></span>|<span data-ttu-id="12a54-137">Отображаемое имя партнера.</span><span class="sxs-lookup"><span data-stu-id="12a54-137">Display name of the partner.</span></span>|
|<span data-ttu-id="12a54-138">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="12a54-138">onboardingUrl</span></span>|<span data-ttu-id="12a54-139">String</span><span class="sxs-lookup"><span data-stu-id="12a54-139">String</span></span>|<span data-ttu-id="12a54-140">URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="12a54-140">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="12a54-141">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="12a54-141">onboardingStatus</span></span>|[<span data-ttu-id="12a54-142">Ремотеассистанцеонбоардингстатус</span><span class="sxs-lookup"><span data-stu-id="12a54-142">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="12a54-143">Подлежит определению.</span><span class="sxs-lookup"><span data-stu-id="12a54-143">TBD.</span></span> <span data-ttu-id="12a54-144">Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="12a54-144">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="12a54-145">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="12a54-145">lastConnectionDateTime</span></span>|<span data-ttu-id="12a54-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12a54-146">DateTimeOffset</span></span>|<span data-ttu-id="12a54-147">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="12a54-147">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="12a54-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="12a54-148">Response</span></span>
<span data-ttu-id="12a54-149">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="12a54-149">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12a54-150">Пример</span><span class="sxs-lookup"><span data-stu-id="12a54-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="12a54-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="12a54-151">Request</span></span>
<span data-ttu-id="12a54-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12a54-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="12a54-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="12a54-153">Response</span></span>
<span data-ttu-id="12a54-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="12a54-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




