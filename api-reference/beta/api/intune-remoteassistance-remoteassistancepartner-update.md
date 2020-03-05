---
title: Обновление объекта remoteAssistancePartner
description: Обновление свойств объекта remoteAssistancePartner.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6184bbed2e40dbb7477817d77385209f3d8dd245
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459297"
---
# <a name="update-remoteassistancepartner"></a><span data-ttu-id="0ae4e-103">Обновление объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="0ae4e-103">Update remoteAssistancePartner</span></span>

<span data-ttu-id="0ae4e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0ae4e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ae4e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ae4e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ae4e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ae4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ae4e-107">Обновление свойств объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="0ae4e-107">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ae4e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0ae4e-108">Prerequisites</span></span>
<span data-ttu-id="0ae4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ae4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ae4e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ae4e-111">Permission type</span></span>|<span data-ttu-id="0ae4e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ae4e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ae4e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ae4e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ae4e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ae4e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0ae4e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ae4e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ae4e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ae4e-116">Not supported.</span></span>|
|<span data-ttu-id="0ae4e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ae4e-117">Application</span></span>|<span data-ttu-id="0ae4e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ae4e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ae4e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ae4e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="0ae4e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0ae4e-120">Request headers</span></span>
|<span data-ttu-id="0ae4e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ae4e-121">Header</span></span>|<span data-ttu-id="0ae4e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0ae4e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ae4e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ae4e-123">Authorization</span></span>|<span data-ttu-id="0ae4e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ae4e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ae4e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0ae4e-125">Accept</span></span>|<span data-ttu-id="0ae4e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ae4e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ae4e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ae4e-127">Request body</span></span>
<span data-ttu-id="0ae4e-128">В теле запроса добавьте представление объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ae4e-128">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="0ae4e-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="0ae4e-129">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>

|<span data-ttu-id="0ae4e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ae4e-130">Property</span></span>|<span data-ttu-id="0ae4e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0ae4e-131">Type</span></span>|<span data-ttu-id="0ae4e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0ae4e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ae4e-133">id</span><span class="sxs-lookup"><span data-stu-id="0ae4e-133">id</span></span>|<span data-ttu-id="0ae4e-134">String</span><span class="sxs-lookup"><span data-stu-id="0ae4e-134">String</span></span>|<span data-ttu-id="0ae4e-135">Уникальный идентификатор партнера.</span><span class="sxs-lookup"><span data-stu-id="0ae4e-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="0ae4e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0ae4e-136">displayName</span></span>|<span data-ttu-id="0ae4e-137">Строка</span><span class="sxs-lookup"><span data-stu-id="0ae4e-137">String</span></span>|<span data-ttu-id="0ae4e-138">Отображаемое имя партнера.</span><span class="sxs-lookup"><span data-stu-id="0ae4e-138">Display name of the partner.</span></span>|
|<span data-ttu-id="0ae4e-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="0ae4e-139">onboardingUrl</span></span>|<span data-ttu-id="0ae4e-140">String</span><span class="sxs-lookup"><span data-stu-id="0ae4e-140">String</span></span>|<span data-ttu-id="0ae4e-141">URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="0ae4e-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="0ae4e-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="0ae4e-142">onboardingStatus</span></span>|[<span data-ttu-id="0ae4e-143">ремотеассистанцеонбоардингстатус</span><span class="sxs-lookup"><span data-stu-id="0ae4e-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="0ae4e-144">Понятное описание состояния текущего соединителя TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="0ae4e-144">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="0ae4e-145">Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="0ae4e-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="0ae4e-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="0ae4e-146">lastConnectionDateTime</span></span>|<span data-ttu-id="0ae4e-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ae4e-147">DateTimeOffset</span></span>|<span data-ttu-id="0ae4e-148">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="0ae4e-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="0ae4e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ae4e-149">Response</span></span>
<span data-ttu-id="0ae4e-150">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0ae4e-150">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ae4e-151">Пример</span><span class="sxs-lookup"><span data-stu-id="0ae4e-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ae4e-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ae4e-152">Request</span></span>
<span data-ttu-id="0ae4e-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ae4e-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
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

### <a name="response"></a><span data-ttu-id="0ae4e-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ae4e-154">Response</span></span>
<span data-ttu-id="0ae4e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ae4e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





