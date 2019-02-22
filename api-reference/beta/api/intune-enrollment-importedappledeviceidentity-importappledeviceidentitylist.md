---
title: Действие importAppleDeviceIdentityList
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 714459b7ee5ab1dd65bb274ad2315e832ce56436
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141484"
---
# <a name="importappledeviceidentitylist-action"></a><span data-ttu-id="66642-103">Действие importAppleDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="66642-103">importAppleDeviceIdentityList action</span></span>

> <span data-ttu-id="66642-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66642-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66642-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66642-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66642-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="66642-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66642-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="66642-107">Prerequisites</span></span>
<span data-ttu-id="66642-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="66642-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="66642-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66642-110">Permission type</span></span>|<span data-ttu-id="66642-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="66642-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66642-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66642-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66642-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66642-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="66642-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66642-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66642-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66642-115">Not supported.</span></span>|
|<span data-ttu-id="66642-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66642-116">Application</span></span>|<span data-ttu-id="66642-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66642-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66642-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66642-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="66642-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66642-119">Request headers</span></span>
|<span data-ttu-id="66642-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="66642-120">Header</span></span>|<span data-ttu-id="66642-121">Значение</span><span class="sxs-lookup"><span data-stu-id="66642-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66642-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="66642-122">Authorization</span></span>|<span data-ttu-id="66642-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="66642-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66642-124">Accept</span><span class="sxs-lookup"><span data-stu-id="66642-124">Accept</span></span>|<span data-ttu-id="66642-125">application/json</span><span class="sxs-lookup"><span data-stu-id="66642-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66642-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66642-126">Request body</span></span>
<span data-ttu-id="66642-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66642-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="66642-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="66642-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="66642-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="66642-129">Property</span></span>|<span data-ttu-id="66642-130">Тип</span><span class="sxs-lookup"><span data-stu-id="66642-130">Type</span></span>|<span data-ttu-id="66642-131">Описание</span><span class="sxs-lookup"><span data-stu-id="66642-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66642-132">importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="66642-132">importedAppleDeviceIdentities</span></span>|<span data-ttu-id="66642-133">Коллекция [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="66642-133">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="66642-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="66642-134">Not yet documented</span></span>|
|<span data-ttu-id="66642-135">Овервритеимпортеддевицеидентитиес</span><span class="sxs-lookup"><span data-stu-id="66642-135">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="66642-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="66642-136">Boolean</span></span>|<span data-ttu-id="66642-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="66642-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="66642-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="66642-138">Response</span></span>
<span data-ttu-id="66642-139">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="66642-139">If successful, this action returns a `200 OK` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66642-140">Пример</span><span class="sxs-lookup"><span data-stu-id="66642-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="66642-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="66642-141">Request</span></span>
<span data-ttu-id="66642-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66642-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList

Content-type: application/json
Content-length: 756

{
  "importedAppleDeviceIdentities": [
    {
      "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
      "id": "352e3c2f-3c2f-352e-2f3c-2e352f3c2e35",
      "serialNumber": "Serial Number value",
      "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
      "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
      "isSupervised": true,
      "discoverySource": "adminImport",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios"
    }
  ],
  "overwriteImportedDeviceIdentities": true
}
```

### <a name="response"></a><span data-ttu-id="66642-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="66642-143">Response</span></span>
<span data-ttu-id="66642-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66642-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 715

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
      "id": "557cfb4a-fb4a-557c-4afb-7c554afb7c55",
      "serialNumber": "Serial Number value",
      "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
      "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
      "isSupervised": true,
      "discoverySource": "adminImport",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios",
      "status": true
    }
  ]
}
```




