---
title: Обновление объекта windowsInformationProtectionAppLearningSummary
description: Обновление свойств объекта windowsInformationProtectionAppLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c1579eeeabce884bc27dff73607204d18aa65310
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028653"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="f6bbc-103">Обновление объекта windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="f6bbc-103">Update windowsInformationProtectionAppLearningSummary</span></span>

<span data-ttu-id="f6bbc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6bbc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6bbc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6bbc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6bbc-106">Обновление свойств объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="f6bbc-106">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6bbc-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f6bbc-107">Prerequisites</span></span>
<span data-ttu-id="f6bbc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6bbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6bbc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6bbc-110">Permission type</span></span>|<span data-ttu-id="f6bbc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6bbc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6bbc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6bbc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f6bbc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6bbc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f6bbc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6bbc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6bbc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6bbc-115">Not supported.</span></span>|
|<span data-ttu-id="f6bbc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6bbc-116">Application</span></span>|<span data-ttu-id="f6bbc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6bbc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6bbc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6bbc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="f6bbc-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f6bbc-119">Request headers</span></span>
|<span data-ttu-id="f6bbc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6bbc-120">Header</span></span>|<span data-ttu-id="f6bbc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f6bbc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6bbc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6bbc-122">Authorization</span></span>|<span data-ttu-id="f6bbc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6bbc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6bbc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f6bbc-124">Accept</span></span>|<span data-ttu-id="f6bbc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f6bbc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6bbc-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f6bbc-126">Request body</span></span>
<span data-ttu-id="f6bbc-127">В теле запроса укажите представление объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6bbc-127">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="f6bbc-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="f6bbc-128">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="f6bbc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6bbc-129">Property</span></span>|<span data-ttu-id="f6bbc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f6bbc-130">Type</span></span>|<span data-ttu-id="f6bbc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f6bbc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6bbc-132">id</span><span class="sxs-lookup"><span data-stu-id="f6bbc-132">id</span></span>|<span data-ttu-id="f6bbc-133">String</span><span class="sxs-lookup"><span data-stu-id="f6bbc-133">String</span></span>|<span data-ttu-id="f6bbc-134">Уникальный идентификатор объекта WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="f6bbc-134">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="f6bbc-135">applicationName</span><span class="sxs-lookup"><span data-stu-id="f6bbc-135">applicationName</span></span>|<span data-ttu-id="f6bbc-136">String</span><span class="sxs-lookup"><span data-stu-id="f6bbc-136">String</span></span>|<span data-ttu-id="f6bbc-137">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="f6bbc-137">Application Name</span></span>|
|<span data-ttu-id="f6bbc-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="f6bbc-138">applicationType</span></span>|[<span data-ttu-id="f6bbc-139">аппликатионтипе</span><span class="sxs-lookup"><span data-stu-id="f6bbc-139">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="f6bbc-140">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="f6bbc-140">Application Type.</span></span> <span data-ttu-id="f6bbc-141">Возможные значения: `universal`, `desktop`.</span><span class="sxs-lookup"><span data-stu-id="f6bbc-141">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="f6bbc-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="f6bbc-142">deviceCount</span></span>|<span data-ttu-id="f6bbc-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f6bbc-143">Int32</span></span>|<span data-ttu-id="f6bbc-144">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="f6bbc-144">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="f6bbc-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6bbc-145">Response</span></span>
<span data-ttu-id="f6bbc-146">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f6bbc-146">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6bbc-147">Пример</span><span class="sxs-lookup"><span data-stu-id="f6bbc-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6bbc-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6bbc-148">Request</span></span>
<span data-ttu-id="f6bbc-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6bbc-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="f6bbc-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6bbc-150">Response</span></span>
<span data-ttu-id="f6bbc-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6bbc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "063baf50-af50-063b-50af-3b0650af3b06",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```









