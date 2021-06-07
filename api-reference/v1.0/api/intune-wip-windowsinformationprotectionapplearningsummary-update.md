---
title: Обновление объекта windowsInformationProtectionAppLearningSummary
description: Обновление свойств объекта windowsInformationProtectionAppLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ffbdaaf7b56ce93c7380660dc425147057f02aa4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752471"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="b1751-103">Обновление объекта windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="b1751-103">Update windowsInformationProtectionAppLearningSummary</span></span>

<span data-ttu-id="b1751-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1751-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1751-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1751-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1751-106">Обновление свойств объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="b1751-106">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1751-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b1751-107">Prerequisites</span></span>
<span data-ttu-id="b1751-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1751-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1751-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1751-110">Permission type</span></span>|<span data-ttu-id="b1751-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1751-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1751-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1751-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b1751-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1751-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b1751-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1751-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1751-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1751-115">Not supported.</span></span>|
|<span data-ttu-id="b1751-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="b1751-116">Application</span></span>|<span data-ttu-id="b1751-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1751-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1751-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1751-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="b1751-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b1751-119">Request headers</span></span>
|<span data-ttu-id="b1751-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1751-120">Header</span></span>|<span data-ttu-id="b1751-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b1751-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1751-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1751-122">Authorization</span></span>|<span data-ttu-id="b1751-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1751-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1751-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b1751-124">Accept</span></span>|<span data-ttu-id="b1751-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b1751-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1751-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1751-126">Request body</span></span>
<span data-ttu-id="b1751-127">В теле запроса укажите представление объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1751-127">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="b1751-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="b1751-128">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="b1751-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1751-129">Property</span></span>|<span data-ttu-id="b1751-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b1751-130">Type</span></span>|<span data-ttu-id="b1751-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b1751-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1751-132">id</span><span class="sxs-lookup"><span data-stu-id="b1751-132">id</span></span>|<span data-ttu-id="b1751-133">String</span><span class="sxs-lookup"><span data-stu-id="b1751-133">String</span></span>|<span data-ttu-id="b1751-134">Уникальный идентификатор объекта WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="b1751-134">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="b1751-135">applicationName</span><span class="sxs-lookup"><span data-stu-id="b1751-135">applicationName</span></span>|<span data-ttu-id="b1751-136">String</span><span class="sxs-lookup"><span data-stu-id="b1751-136">String</span></span>|<span data-ttu-id="b1751-137">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="b1751-137">Application Name</span></span>|
|<span data-ttu-id="b1751-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="b1751-138">applicationType</span></span>|[<span data-ttu-id="b1751-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="b1751-139">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="b1751-140">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="b1751-140">Application Type.</span></span> <span data-ttu-id="b1751-141">Возможные значения: `universal`, `desktop`.</span><span class="sxs-lookup"><span data-stu-id="b1751-141">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="b1751-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="b1751-142">deviceCount</span></span>|<span data-ttu-id="b1751-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b1751-143">Int32</span></span>|<span data-ttu-id="b1751-144">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="b1751-144">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="b1751-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1751-145">Response</span></span>
<span data-ttu-id="b1751-146">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b1751-146">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1751-147">Пример</span><span class="sxs-lookup"><span data-stu-id="b1751-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1751-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1751-148">Request</span></span>
<span data-ttu-id="b1751-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1751-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b1751-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1751-150">Response</span></span>
<span data-ttu-id="b1751-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1751-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




