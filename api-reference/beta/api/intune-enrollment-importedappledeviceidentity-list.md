---
title: Список importedAppleDeviceIdentities
description: Список свойств и связей объектов Импортедаппледевицеидентити.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 491683b9be8b6c280d0f025fcadd7c949559b45d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908471"
---
# <a name="list-importedappledeviceidentities"></a><span data-ttu-id="83e64-103">Список importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="83e64-103">List importedAppleDeviceIdentities</span></span>

> <span data-ttu-id="83e64-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83e64-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83e64-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="83e64-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83e64-106">Список свойств и связей объектов [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="83e64-106">List properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83e64-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="83e64-107">Prerequisites</span></span>
<span data-ttu-id="83e64-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83e64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83e64-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83e64-110">Permission type</span></span>|<span data-ttu-id="83e64-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="83e64-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83e64-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83e64-112">Delegated (work or school account)</span></span>|<span data-ttu-id="83e64-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="83e64-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="83e64-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83e64-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83e64-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83e64-115">Not supported.</span></span>|
|<span data-ttu-id="83e64-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83e64-116">Application</span></span>|<span data-ttu-id="83e64-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83e64-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83e64-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83e64-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="83e64-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83e64-119">Request headers</span></span>
|<span data-ttu-id="83e64-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="83e64-120">Header</span></span>|<span data-ttu-id="83e64-121">Значение</span><span class="sxs-lookup"><span data-stu-id="83e64-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83e64-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="83e64-122">Authorization</span></span>|<span data-ttu-id="83e64-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83e64-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83e64-124">Accept</span><span class="sxs-lookup"><span data-stu-id="83e64-124">Accept</span></span>|<span data-ttu-id="83e64-125">application/json</span><span class="sxs-lookup"><span data-stu-id="83e64-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83e64-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83e64-126">Request body</span></span>
<span data-ttu-id="83e64-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="83e64-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83e64-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="83e64-128">Response</span></span>
<span data-ttu-id="83e64-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [импортедаппледевицеидентити](../resources/intune-enrollment-importedappledeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="83e64-129">If successful, this method returns a `200 OK` response code and a collection of [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83e64-130">Пример</span><span class="sxs-lookup"><span data-stu-id="83e64-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="83e64-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="83e64-131">Request</span></span>
<span data-ttu-id="83e64-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83e64-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="83e64-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="83e64-133">Response</span></span>
<span data-ttu-id="83e64-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="83e64-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 686

{
  "value": [
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
  ]
}
```




