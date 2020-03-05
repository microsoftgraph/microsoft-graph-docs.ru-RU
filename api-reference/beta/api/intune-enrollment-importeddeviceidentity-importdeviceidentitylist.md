---
title: Действие importDeviceIdentityList
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c41b74df62ab444b86ad3c8e2f009413d94aa94
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42466628"
---
# <a name="importdeviceidentitylist-action"></a><span data-ttu-id="0c74e-103">Действие importDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="0c74e-103">importDeviceIdentityList action</span></span>

<span data-ttu-id="0c74e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0c74e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c74e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c74e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c74e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c74e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c74e-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0c74e-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c74e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0c74e-108">Prerequisites</span></span>
<span data-ttu-id="0c74e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c74e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c74e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c74e-111">Permission type</span></span>|<span data-ttu-id="0c74e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c74e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c74e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c74e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c74e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c74e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0c74e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c74e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c74e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c74e-116">Not supported.</span></span>|
|<span data-ttu-id="0c74e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c74e-117">Application</span></span>|<span data-ttu-id="0c74e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c74e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c74e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c74e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities/importDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="0c74e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0c74e-120">Request headers</span></span>
|<span data-ttu-id="0c74e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c74e-121">Header</span></span>|<span data-ttu-id="0c74e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0c74e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c74e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c74e-123">Authorization</span></span>|<span data-ttu-id="0c74e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c74e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c74e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0c74e-125">Accept</span></span>|<span data-ttu-id="0c74e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c74e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c74e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c74e-127">Request body</span></span>
<span data-ttu-id="0c74e-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c74e-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0c74e-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="0c74e-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0c74e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c74e-130">Property</span></span>|<span data-ttu-id="0c74e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0c74e-131">Type</span></span>|<span data-ttu-id="0c74e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0c74e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c74e-133">импортеддевицеидентитиес</span><span class="sxs-lookup"><span data-stu-id="0c74e-133">importedDeviceIdentities</span></span>|<span data-ttu-id="0c74e-134">Коллекция [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="0c74e-134">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="0c74e-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0c74e-135">Not yet documented</span></span>|
|<span data-ttu-id="0c74e-136">овервритеимпортеддевицеидентитиес</span><span class="sxs-lookup"><span data-stu-id="0c74e-136">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="0c74e-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c74e-137">Boolean</span></span>|<span data-ttu-id="0c74e-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0c74e-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0c74e-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c74e-139">Response</span></span>
<span data-ttu-id="0c74e-140">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0c74e-140">If successful, this action returns a `200 OK` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c74e-141">Пример</span><span class="sxs-lookup"><span data-stu-id="0c74e-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c74e-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c74e-142">Request</span></span>
<span data-ttu-id="0c74e-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c74e-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/importDeviceIdentityList

Content-type: application/json
Content-length: 642

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
  ],
  "overwriteImportedDeviceIdentities": true
}
```

### <a name="response"></a><span data-ttu-id="0c74e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c74e-144">Response</span></span>
<span data-ttu-id="0c74e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c74e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 606

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
      "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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





