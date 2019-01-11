---
title: Обновление объекта remoteAssistancePartner
description: Обновление свойств объекта remoteAssistancePartner.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 16b7c3f9d3125ca688f08faa22772c4335e02a8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871402"
---
# <a name="update-remoteassistancepartner"></a><span data-ttu-id="3e05a-103">Обновление объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="3e05a-103">Update remoteAssistancePartner</span></span>

> <span data-ttu-id="3e05a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3e05a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e05a-105">Обновление свойств объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="3e05a-105">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3e05a-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3e05a-106">Prerequisites</span></span>
<span data-ttu-id="3e05a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e05a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e05a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e05a-109">Permission type</span></span>|<span data-ttu-id="3e05a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e05a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e05a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e05a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3e05a-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e05a-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3e05a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e05a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e05a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e05a-114">Not supported.</span></span>|
|<span data-ttu-id="3e05a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e05a-115">Application</span></span>|<span data-ttu-id="3e05a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e05a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e05a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e05a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="3e05a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e05a-118">Request headers</span></span>
|<span data-ttu-id="3e05a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e05a-119">Header</span></span>|<span data-ttu-id="3e05a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3e05a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e05a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e05a-121">Authorization</span></span>|<span data-ttu-id="3e05a-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3e05a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e05a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3e05a-123">Accept</span></span>|<span data-ttu-id="3e05a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3e05a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e05a-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3e05a-125">Request body</span></span>
<span data-ttu-id="3e05a-126">В теле запроса добавьте представление объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e05a-126">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="3e05a-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="3e05a-127">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

|<span data-ttu-id="3e05a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e05a-128">Property</span></span>|<span data-ttu-id="3e05a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3e05a-129">Type</span></span>|<span data-ttu-id="3e05a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3e05a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e05a-131">id</span><span class="sxs-lookup"><span data-stu-id="3e05a-131">id</span></span>|<span data-ttu-id="3e05a-132">String</span><span class="sxs-lookup"><span data-stu-id="3e05a-132">String</span></span>|<span data-ttu-id="3e05a-133">Уникальный идентификатор партнера.</span><span class="sxs-lookup"><span data-stu-id="3e05a-133">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="3e05a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="3e05a-134">displayName</span></span>|<span data-ttu-id="3e05a-135">String</span><span class="sxs-lookup"><span data-stu-id="3e05a-135">String</span></span>|<span data-ttu-id="3e05a-136">Отображаемое имя партнера.</span><span class="sxs-lookup"><span data-stu-id="3e05a-136">Display name of the partner.</span></span>|
|<span data-ttu-id="3e05a-137">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="3e05a-137">onboardingUrl</span></span>|<span data-ttu-id="3e05a-138">String</span><span class="sxs-lookup"><span data-stu-id="3e05a-138">String</span></span>|<span data-ttu-id="3e05a-139">URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="3e05a-139">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="3e05a-140">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="3e05a-140">onboardingStatus</span></span>|[<span data-ttu-id="3e05a-141">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="3e05a-141">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="3e05a-142">БУДЕТ ОПРЕДЕЛЕНО ПОЗЖЕ.</span><span class="sxs-lookup"><span data-stu-id="3e05a-142">TBD.</span></span> <span data-ttu-id="3e05a-143">Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="3e05a-143">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="3e05a-144">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="3e05a-144">lastConnectionDateTime</span></span>|<span data-ttu-id="3e05a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e05a-145">DateTimeOffset</span></span>|<span data-ttu-id="3e05a-146">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="3e05a-146">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="3e05a-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e05a-147">Response</span></span>
<span data-ttu-id="3e05a-148">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3e05a-148">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e05a-149">Пример</span><span class="sxs-lookup"><span data-stu-id="3e05a-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="3e05a-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e05a-150">Request</span></span>
<span data-ttu-id="3e05a-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e05a-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3e05a-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e05a-152">Response</span></span>
<span data-ttu-id="3e05a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3e05a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



