---
title: Создание объекта remoteAssistancePartner
description: Создание объекта remoteAssistancePartner.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1f9c2b8e701a830ccf9ca4bf1051b6ef2b796eed
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178047"
---
# <a name="create-remoteassistancepartner"></a><span data-ttu-id="df65b-103">Создание объекта remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="df65b-103">Create remoteAssistancePartner</span></span>

<span data-ttu-id="df65b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df65b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df65b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df65b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df65b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="df65b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df65b-107">Создание объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="df65b-107">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df65b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="df65b-108">Prerequisites</span></span>
<span data-ttu-id="df65b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df65b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df65b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df65b-111">Permission type</span></span>|<span data-ttu-id="df65b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="df65b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df65b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df65b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df65b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df65b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="df65b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df65b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df65b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df65b-116">Not supported.</span></span>|
|<span data-ttu-id="df65b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df65b-117">Application</span></span>|<span data-ttu-id="df65b-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df65b-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df65b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df65b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="df65b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="df65b-120">Request headers</span></span>
|<span data-ttu-id="df65b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="df65b-121">Header</span></span>|<span data-ttu-id="df65b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="df65b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df65b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="df65b-123">Authorization</span></span>|<span data-ttu-id="df65b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df65b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df65b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="df65b-125">Accept</span></span>|<span data-ttu-id="df65b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df65b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df65b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df65b-127">Request body</span></span>
<span data-ttu-id="df65b-128">В теле запроса добавьте представление объекта remoteAssistancePartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df65b-128">In the request body, supply a JSON representation for the remoteAssistancePartner object.</span></span>

<span data-ttu-id="df65b-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта remoteAssistancePartner.</span><span class="sxs-lookup"><span data-stu-id="df65b-129">The following table shows the properties that are required when you create the remoteAssistancePartner.</span></span>

|<span data-ttu-id="df65b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="df65b-130">Property</span></span>|<span data-ttu-id="df65b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="df65b-131">Type</span></span>|<span data-ttu-id="df65b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="df65b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df65b-133">id</span><span class="sxs-lookup"><span data-stu-id="df65b-133">id</span></span>|<span data-ttu-id="df65b-134">String</span><span class="sxs-lookup"><span data-stu-id="df65b-134">String</span></span>|<span data-ttu-id="df65b-135">Уникальный идентификатор партнера.</span><span class="sxs-lookup"><span data-stu-id="df65b-135">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="df65b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="df65b-136">displayName</span></span>|<span data-ttu-id="df65b-137">Строка</span><span class="sxs-lookup"><span data-stu-id="df65b-137">String</span></span>|<span data-ttu-id="df65b-138">Отображаемое имя партнера.</span><span class="sxs-lookup"><span data-stu-id="df65b-138">Display name of the partner.</span></span>|
|<span data-ttu-id="df65b-139">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="df65b-139">onboardingUrl</span></span>|<span data-ttu-id="df65b-140">String</span><span class="sxs-lookup"><span data-stu-id="df65b-140">String</span></span>|<span data-ttu-id="df65b-141">URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.</span><span class="sxs-lookup"><span data-stu-id="df65b-141">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="df65b-142">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="df65b-142">onboardingStatus</span></span>|[<span data-ttu-id="df65b-143">ремотеассистанцеонбоардингстатус</span><span class="sxs-lookup"><span data-stu-id="df65b-143">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="df65b-144">Понятное описание состояния текущего соединителя TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="df65b-144">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="df65b-145">Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.</span><span class="sxs-lookup"><span data-stu-id="df65b-145">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="df65b-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="df65b-146">lastConnectionDateTime</span></span>|<span data-ttu-id="df65b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df65b-147">DateTimeOffset</span></span>|<span data-ttu-id="df65b-148">Метка времени последнего запроса, отправленного в службу Intune партнером TEM.</span><span class="sxs-lookup"><span data-stu-id="df65b-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="df65b-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="df65b-149">Response</span></span>
<span data-ttu-id="df65b-150">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="df65b-150">If successful, this method returns a `201 Created` response code and a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df65b-151">Пример</span><span class="sxs-lookup"><span data-stu-id="df65b-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="df65b-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="df65b-152">Request</span></span>
<span data-ttu-id="df65b-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df65b-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="df65b-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="df65b-154">Response</span></span>
<span data-ttu-id="df65b-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df65b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



