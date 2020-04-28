---
title: Действие searchExistingIdentities
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7c3204c972cb1fdc9a08e8b1f0a48e539d3c2c69
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451021"
---
# <a name="searchexistingidentities-action"></a><span data-ttu-id="a2392-103">Действие searchExistingIdentities</span><span class="sxs-lookup"><span data-stu-id="a2392-103">searchExistingIdentities action</span></span>

<span data-ttu-id="a2392-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2392-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2392-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2392-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2392-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2392-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2392-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a2392-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2392-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a2392-108">Prerequisites</span></span>
<span data-ttu-id="a2392-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2392-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2392-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2392-111">Permission type</span></span>|<span data-ttu-id="a2392-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2392-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2392-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2392-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2392-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2392-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a2392-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2392-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2392-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2392-116">Not supported.</span></span>|
|<span data-ttu-id="a2392-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2392-117">Application</span></span>|<span data-ttu-id="a2392-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2392-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2392-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2392-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities/searchExistingIdentities
```

## <a name="request-headers"></a><span data-ttu-id="a2392-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a2392-120">Request headers</span></span>
|<span data-ttu-id="a2392-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2392-121">Header</span></span>|<span data-ttu-id="a2392-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a2392-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2392-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2392-123">Authorization</span></span>|<span data-ttu-id="a2392-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2392-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2392-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a2392-125">Accept</span></span>|<span data-ttu-id="a2392-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2392-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2392-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a2392-127">Request body</span></span>
<span data-ttu-id="a2392-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2392-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a2392-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a2392-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a2392-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2392-130">Property</span></span>|<span data-ttu-id="a2392-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a2392-131">Type</span></span>|<span data-ttu-id="a2392-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a2392-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2392-133">импортеддевицеидентитиес</span><span class="sxs-lookup"><span data-stu-id="a2392-133">importedDeviceIdentities</span></span>|<span data-ttu-id="a2392-134">Коллекция [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="a2392-134">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="a2392-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a2392-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a2392-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2392-136">Response</span></span>
<span data-ttu-id="a2392-137">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a2392-137">If successful, this action returns a `200 OK` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2392-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a2392-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2392-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2392-139">Request</span></span>
<span data-ttu-id="a2392-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2392-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/searchExistingIdentities

Content-type: application/json
Content-length: 596

{
  "importedDeviceIdentities": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentity",
      "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="a2392-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2392-141">Response</span></span>
<span data-ttu-id="a2392-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2392-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 577

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentity",
      "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios"
    }
  ]
}
```



