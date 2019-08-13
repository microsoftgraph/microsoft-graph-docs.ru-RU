---
title: Действие searchExistingIdentities
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1d526c2a9c1b3b9dff3cd69af676b1a2fc7f1be8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356370"
---
# <a name="searchexistingidentities-action"></a><span data-ttu-id="e735d-103">Действие searchExistingIdentities</span><span class="sxs-lookup"><span data-stu-id="e735d-103">searchExistingIdentities action</span></span>

> <span data-ttu-id="e735d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e735d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e735d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e735d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e735d-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="e735d-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e735d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e735d-107">Prerequisites</span></span>
<span data-ttu-id="e735d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e735d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e735d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e735d-110">Permission type</span></span>|<span data-ttu-id="e735d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e735d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e735d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e735d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e735d-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e735d-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e735d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e735d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e735d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e735d-115">Not supported.</span></span>|
|<span data-ttu-id="e735d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e735d-116">Application</span></span>|<span data-ttu-id="e735d-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e735d-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e735d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e735d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities/searchExistingIdentities
```

## <a name="request-headers"></a><span data-ttu-id="e735d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e735d-119">Request headers</span></span>
|<span data-ttu-id="e735d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e735d-120">Header</span></span>|<span data-ttu-id="e735d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e735d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e735d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e735d-122">Authorization</span></span>|<span data-ttu-id="e735d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e735d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e735d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e735d-124">Accept</span></span>|<span data-ttu-id="e735d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e735d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e735d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e735d-126">Request body</span></span>
<span data-ttu-id="e735d-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e735d-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e735d-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="e735d-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e735d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e735d-129">Property</span></span>|<span data-ttu-id="e735d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e735d-130">Type</span></span>|<span data-ttu-id="e735d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e735d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e735d-132">импортеддевицеидентитиес</span><span class="sxs-lookup"><span data-stu-id="e735d-132">importedDeviceIdentities</span></span>|<span data-ttu-id="e735d-133">Коллекция [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="e735d-133">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="e735d-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e735d-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e735d-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="e735d-135">Response</span></span>
<span data-ttu-id="e735d-136">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e735d-136">If successful, this action returns a `200 OK` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e735d-137">Пример</span><span class="sxs-lookup"><span data-stu-id="e735d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="e735d-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="e735d-138">Request</span></span>
<span data-ttu-id="e735d-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e735d-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e735d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="e735d-140">Response</span></span>
<span data-ttu-id="e735d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e735d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






