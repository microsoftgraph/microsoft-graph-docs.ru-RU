---
title: Действие importAppleDeviceIdentityList
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 75a40be8d2ea3ddafadb78f95662dcadf7a9ac01
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890603"
---
# <a name="importappledeviceidentitylist-action"></a><span data-ttu-id="4355a-103">Действие importAppleDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="4355a-103">importAppleDeviceIdentityList action</span></span>

> <span data-ttu-id="4355a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4355a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4355a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4355a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4355a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4355a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4355a-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4355a-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4355a-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4355a-108">Prerequisites</span></span>
<span data-ttu-id="4355a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4355a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4355a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4355a-111">Permission type</span></span>|<span data-ttu-id="4355a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4355a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4355a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4355a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4355a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4355a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4355a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4355a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4355a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4355a-116">Not supported.</span></span>|
|<span data-ttu-id="4355a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4355a-117">Application</span></span>|<span data-ttu-id="4355a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4355a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4355a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4355a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="4355a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4355a-120">Request headers</span></span>
|<span data-ttu-id="4355a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4355a-121">Header</span></span>|<span data-ttu-id="4355a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4355a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4355a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4355a-123">Authorization</span></span>|<span data-ttu-id="4355a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4355a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4355a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4355a-125">Accept</span></span>|<span data-ttu-id="4355a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4355a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4355a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4355a-127">Request body</span></span>
<span data-ttu-id="4355a-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4355a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4355a-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4355a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4355a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4355a-130">Property</span></span>|<span data-ttu-id="4355a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4355a-131">Type</span></span>|<span data-ttu-id="4355a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4355a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4355a-133">importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="4355a-133">importedAppleDeviceIdentities</span></span>|<span data-ttu-id="4355a-134">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="4355a-134">[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) collection</span></span>|<span data-ttu-id="4355a-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4355a-135">Not yet documented</span></span>|
|<span data-ttu-id="4355a-136">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="4355a-136">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="4355a-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="4355a-137">Boolean</span></span>|<span data-ttu-id="4355a-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4355a-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4355a-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="4355a-139">Response</span></span>
<span data-ttu-id="4355a-140">Если успешно завершена, это действие возвращает `200 OK` код ответа и семейства [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4355a-140">If successful, this action returns a `200 OK` response code and a [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4355a-141">Пример</span><span class="sxs-lookup"><span data-stu-id="4355a-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="4355a-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="4355a-142">Request</span></span>
<span data-ttu-id="4355a-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4355a-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4355a-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="4355a-144">Response</span></span>
<span data-ttu-id="4355a-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4355a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





