---
title: Обновление объекта remoteAssistancePartner
description: Обновление свойств объекта remoteAssistancePartner.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a34c6ec097bfae38a7e2d5bc7a51b0bfd6489e12
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983409"
---
# <a name="update-remoteassistancepartner"></a><span data-ttu-id="82f11-103">Обновление объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="82f11-103">Update remoteAssistancePartner</span></span>

> <span data-ttu-id="82f11-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82f11-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82f11-105">Обновление свойств объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="82f11-105">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82f11-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="82f11-106">Prerequisites</span></span>
<span data-ttu-id="82f11-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82f11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82f11-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82f11-109">Permission type</span></span>|<span data-ttu-id="82f11-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82f11-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82f11-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82f11-111">Delegated (work or school account)</span></span>|<span data-ttu-id="82f11-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82f11-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="82f11-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82f11-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82f11-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82f11-114">Not supported.</span></span>|
|<span data-ttu-id="82f11-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82f11-115">Application</span></span>|<span data-ttu-id="82f11-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82f11-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82f11-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82f11-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="82f11-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82f11-118">Request headers</span></span>
|<span data-ttu-id="82f11-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82f11-119">Header</span></span>|<span data-ttu-id="82f11-120">Значение</span><span class="sxs-lookup"><span data-stu-id="82f11-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82f11-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82f11-121">Authorization</span></span>|<span data-ttu-id="82f11-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82f11-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82f11-123">Accept</span><span class="sxs-lookup"><span data-stu-id="82f11-123">Accept</span></span>|<span data-ttu-id="82f11-124">application/json</span><span class="sxs-lookup"><span data-stu-id="82f11-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82f11-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82f11-125">Request body</span></span>
<span data-ttu-id="82f11-126">В теле запроса добавьте представление объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82f11-126">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="82f11-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="82f11-127">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

|<span data-ttu-id="82f11-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="82f11-128">Property</span></span>|<span data-ttu-id="82f11-129">Тип</span><span class="sxs-lookup"><span data-stu-id="82f11-129">Type</span></span>|<span data-ttu-id="82f11-130">Описание</span><span class="sxs-lookup"><span data-stu-id="82f11-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82f11-131">id</span><span class="sxs-lookup"><span data-stu-id="82f11-131">id</span></span>|<span data-ttu-id="82f11-132">String</span><span class="sxs-lookup"><span data-stu-id="82f11-132">String</span></span>|<span data-ttu-id="82f11-133">Уникальный идентификатор партнера.</span><span class="sxs-lookup"><span data-stu-id="82f11-133">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="82f11-134">displayName</span><span class="sxs-lookup"><span data-stu-id="82f11-134">displayName</span></span>|<span data-ttu-id="82f11-135">Строка</span><span class="sxs-lookup"><span data-stu-id="82f11-135">String</span></span>|<span data-ttu-id="82f11-136">Отображаемое имя партнера.</span><span class="sxs-lookup"><span data-stu-id="82f11-136">Display name of the partner.</span></span>|
|<span data-ttu-id="82f11-137">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="82f11-137">onboardingUrl</span></span>|<span data-ttu-id="82f11-138">String</span><span class="sxs-lookup"><span data-stu-id="82f11-138">String</span></span>|<span data-ttu-id="82f11-139">URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="82f11-139">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="82f11-140">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="82f11-140">onboardingStatus</span></span>|[<span data-ttu-id="82f11-141">Ремотеассистанцеонбоардингстатус</span><span class="sxs-lookup"><span data-stu-id="82f11-141">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="82f11-142">Подлежит определению.</span><span class="sxs-lookup"><span data-stu-id="82f11-142">TBD.</span></span> <span data-ttu-id="82f11-143">Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="82f11-143">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="82f11-144">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="82f11-144">lastConnectionDateTime</span></span>|<span data-ttu-id="82f11-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82f11-145">DateTimeOffset</span></span>|<span data-ttu-id="82f11-146">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="82f11-146">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="82f11-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="82f11-147">Response</span></span>
<span data-ttu-id="82f11-148">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="82f11-148">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82f11-149">Пример</span><span class="sxs-lookup"><span data-stu-id="82f11-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="82f11-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="82f11-150">Request</span></span>
<span data-ttu-id="82f11-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82f11-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="82f11-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="82f11-152">Response</span></span>
<span data-ttu-id="82f11-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82f11-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



