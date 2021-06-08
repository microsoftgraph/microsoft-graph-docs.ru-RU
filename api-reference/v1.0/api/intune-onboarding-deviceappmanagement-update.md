---
title: Обновление объекта deviceAppManagement
description: Обновление свойств объекта deviceAppManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cc443e6f6d99a220c9e5b9a3bc88cd4cf30ec013
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759605"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="18dd3-103">Обновление объекта deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="18dd3-103">Update deviceAppManagement</span></span>

<span data-ttu-id="18dd3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18dd3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18dd3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18dd3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18dd3-106">Обновление свойств объекта [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="18dd3-106">Update the properties of a [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18dd3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="18dd3-107">Prerequisites</span></span>
<span data-ttu-id="18dd3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18dd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18dd3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18dd3-110">Permission type</span></span>|<span data-ttu-id="18dd3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18dd3-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18dd3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18dd3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="18dd3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18dd3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="18dd3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18dd3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18dd3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18dd3-115">Not supported.</span></span>|
|<span data-ttu-id="18dd3-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="18dd3-116">Application</span></span>|<span data-ttu-id="18dd3-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18dd3-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18dd3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18dd3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="18dd3-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="18dd3-119">Request headers</span></span>
|<span data-ttu-id="18dd3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18dd3-120">Header</span></span>|<span data-ttu-id="18dd3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="18dd3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18dd3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="18dd3-122">Authorization</span></span>|<span data-ttu-id="18dd3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18dd3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18dd3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="18dd3-124">Accept</span></span>|<span data-ttu-id="18dd3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="18dd3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18dd3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18dd3-126">Request body</span></span>
<span data-ttu-id="18dd3-127">В тексте запроса добавьте представление объекта [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18dd3-127">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="18dd3-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="18dd3-128">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md).</span></span>

|<span data-ttu-id="18dd3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="18dd3-129">Property</span></span>|<span data-ttu-id="18dd3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="18dd3-130">Type</span></span>|<span data-ttu-id="18dd3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="18dd3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18dd3-132">id</span><span class="sxs-lookup"><span data-stu-id="18dd3-132">id</span></span>|<span data-ttu-id="18dd3-133">String</span><span class="sxs-lookup"><span data-stu-id="18dd3-133">String</span></span>|<span data-ttu-id="18dd3-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="18dd3-134">Not yet documented</span></span>|
|<span data-ttu-id="18dd3-135">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="18dd3-135">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="18dd3-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18dd3-136">DateTimeOffset</span></span>|<span data-ttu-id="18dd3-137">Время последней успешной синхронизации приложений из Microsoft Store для бизнеса с учетной записью.</span><span class="sxs-lookup"><span data-stu-id="18dd3-137">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="18dd3-138">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="18dd3-138">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="18dd3-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="18dd3-139">Boolean</span></span>|<span data-ttu-id="18dd3-140">Указывает, включена ли для учетной запись синхронизация приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="18dd3-140">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="18dd3-141">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="18dd3-141">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="18dd3-142">String</span><span class="sxs-lookup"><span data-stu-id="18dd3-142">String</span></span>|<span data-ttu-id="18dd3-143">Сведения о языковом стандарте, используемом для синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="18dd3-143">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="18dd3-144">Региональные параметры, относящиеся к стране или региону.</span><span class="sxs-lookup"><span data-stu-id="18dd3-144">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="18dd3-145">Названия этих региональных параметров соответствуют стандарту RFC 4646 (для Windows Vista и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="18dd3-145">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="18dd3-146">Используется формат <languagecode2>-<страна/код_региона2>, где <languagecode2> — это двухбуквенный код в нижнем регистре, полученный из стандарта ISO 639-1, а <страна/код_регион2> — код из двух прописных букв по стандарту ISO 3166.</span><span class="sxs-lookup"><span data-stu-id="18dd3-146">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="18dd3-147">Например, en-US для английского (США) — это определенный региональный стандарт.</span><span class="sxs-lookup"><span data-stu-id="18dd3-147">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="18dd3-148">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="18dd3-148">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="18dd3-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18dd3-149">DateTimeOffset</span></span>|<span data-ttu-id="18dd3-150">Время последней завершенной синхронизации приложений из Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="18dd3-150">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|



## <a name="response"></a><span data-ttu-id="18dd3-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="18dd3-151">Response</span></span>
<span data-ttu-id="18dd3-152">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18dd3-152">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-onboarding-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18dd3-153">Пример</span><span class="sxs-lookup"><span data-stu-id="18dd3-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="18dd3-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="18dd3-154">Request</span></span>
<span data-ttu-id="18dd3-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18dd3-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 394

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:57:45.2453148-08:00",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:02:00.0421137-08:00"
}
```

### <a name="response"></a><span data-ttu-id="18dd3-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="18dd3-156">Response</span></span>
<span data-ttu-id="18dd3-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18dd3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:57:45.2453148-08:00",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:02:00.0421137-08:00"
}
```




