---
title: Действие importAppleDeviceIdentityList
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f558de302a1401c575d2832389e9277b4fb32401
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48685655"
---
# <a name="importappledeviceidentitylist-action"></a><span data-ttu-id="771fe-103">Действие importAppleDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="771fe-103">importAppleDeviceIdentityList action</span></span>

<span data-ttu-id="771fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="771fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="771fe-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="771fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="771fe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="771fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="771fe-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="771fe-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="771fe-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="771fe-108">Prerequisites</span></span>
<span data-ttu-id="771fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="771fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="771fe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="771fe-111">Permission type</span></span>|<span data-ttu-id="771fe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="771fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="771fe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="771fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="771fe-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="771fe-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="771fe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="771fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="771fe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="771fe-116">Not supported.</span></span>|
|<span data-ttu-id="771fe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="771fe-117">Application</span></span>|<span data-ttu-id="771fe-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="771fe-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="771fe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="771fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="771fe-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="771fe-120">Request headers</span></span>
|<span data-ttu-id="771fe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="771fe-121">Header</span></span>|<span data-ttu-id="771fe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="771fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="771fe-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="771fe-123">Authorization</span></span>|<span data-ttu-id="771fe-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="771fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="771fe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="771fe-125">Accept</span></span>|<span data-ttu-id="771fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="771fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="771fe-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="771fe-127">Request body</span></span>
<span data-ttu-id="771fe-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="771fe-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="771fe-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="771fe-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="771fe-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="771fe-130">Property</span></span>|<span data-ttu-id="771fe-131">Тип</span><span class="sxs-lookup"><span data-stu-id="771fe-131">Type</span></span>|<span data-ttu-id="771fe-132">Описание</span><span class="sxs-lookup"><span data-stu-id="771fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="771fe-133">importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="771fe-133">importedAppleDeviceIdentities</span></span>|<span data-ttu-id="771fe-134">Коллекция [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="771fe-134">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="771fe-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="771fe-135">Not yet documented</span></span>|
|<span data-ttu-id="771fe-136">овервритеимпортеддевицеидентитиес</span><span class="sxs-lookup"><span data-stu-id="771fe-136">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="771fe-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="771fe-137">Boolean</span></span>|<span data-ttu-id="771fe-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="771fe-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="771fe-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="771fe-139">Response</span></span>
<span data-ttu-id="771fe-140">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [импортедаппледевицеидентитиресулт](../resources/intune-enrollment-importedappledeviceidentityresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="771fe-140">If successful, this action returns a `200 OK` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="771fe-141">Пример</span><span class="sxs-lookup"><span data-stu-id="771fe-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="771fe-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="771fe-142">Request</span></span>
<span data-ttu-id="771fe-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="771fe-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList

Content-type: application/json
Content-length: 782

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
      "isDeleted": true,
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

### <a name="response"></a><span data-ttu-id="771fe-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="771fe-144">Response</span></span>
<span data-ttu-id="771fe-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="771fe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 741

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
      "isDeleted": true,
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





