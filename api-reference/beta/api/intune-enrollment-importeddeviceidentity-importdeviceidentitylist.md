---
title: Действие importDeviceIdentityList
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b42964ad5bbb2424167f449859eec911466ba97b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908310"
---
# <a name="importdeviceidentitylist-action"></a><span data-ttu-id="0cd42-103">Действие importDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="0cd42-103">importDeviceIdentityList action</span></span>

> <span data-ttu-id="0cd42-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cd42-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cd42-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0cd42-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cd42-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0cd42-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cd42-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0cd42-107">Prerequisites</span></span>
<span data-ttu-id="0cd42-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cd42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cd42-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0cd42-110">Permission type</span></span>|<span data-ttu-id="0cd42-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0cd42-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cd42-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0cd42-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0cd42-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cd42-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0cd42-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0cd42-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cd42-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cd42-115">Not supported.</span></span>|
|<span data-ttu-id="0cd42-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0cd42-116">Application</span></span>|<span data-ttu-id="0cd42-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cd42-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cd42-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0cd42-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities/importDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="0cd42-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0cd42-119">Request headers</span></span>
|<span data-ttu-id="0cd42-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0cd42-120">Header</span></span>|<span data-ttu-id="0cd42-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0cd42-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cd42-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0cd42-122">Authorization</span></span>|<span data-ttu-id="0cd42-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0cd42-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cd42-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0cd42-124">Accept</span></span>|<span data-ttu-id="0cd42-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0cd42-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cd42-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0cd42-126">Request body</span></span>
<span data-ttu-id="0cd42-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cd42-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0cd42-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="0cd42-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0cd42-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cd42-129">Property</span></span>|<span data-ttu-id="0cd42-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0cd42-130">Type</span></span>|<span data-ttu-id="0cd42-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0cd42-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cd42-132">Импортеддевицеидентитиес</span><span class="sxs-lookup"><span data-stu-id="0cd42-132">importedDeviceIdentities</span></span>|<span data-ttu-id="0cd42-133">Коллекция [импортеддевицеидентити](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="0cd42-133">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="0cd42-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0cd42-134">Not yet documented</span></span>|
|<span data-ttu-id="0cd42-135">Овервритеимпортеддевицеидентитиес</span><span class="sxs-lookup"><span data-stu-id="0cd42-135">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="0cd42-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cd42-136">Boolean</span></span>|<span data-ttu-id="0cd42-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0cd42-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0cd42-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="0cd42-138">Response</span></span>
<span data-ttu-id="0cd42-139">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [импортеддевицеидентитиресулт](../resources/intune-enrollment-importeddeviceidentityresult.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0cd42-139">If successful, this action returns a `200 OK` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cd42-140">Пример</span><span class="sxs-lookup"><span data-stu-id="0cd42-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cd42-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="0cd42-141">Request</span></span>
<span data-ttu-id="0cd42-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0cd42-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0cd42-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="0cd42-143">Response</span></span>
<span data-ttu-id="0cd42-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0cd42-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




