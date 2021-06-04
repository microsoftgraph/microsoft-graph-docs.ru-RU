---
title: Создание объекта windowsInformationProtectionAppLearningSummary
description: Создание объекта windowsInformationProtectionAppLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9a4145594557f526ea9dfaf70736529cd83eee5b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52743065"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="1a0e7-103">Создание объекта windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="1a0e7-103">Create windowsInformationProtectionAppLearningSummary</span></span>

<span data-ttu-id="1a0e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a0e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a0e7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a0e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a0e7-106">Создание объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="1a0e7-106">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a0e7-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1a0e7-107">Prerequisites</span></span>
<span data-ttu-id="1a0e7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a0e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a0e7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a0e7-110">Permission type</span></span>|<span data-ttu-id="1a0e7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a0e7-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a0e7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a0e7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1a0e7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a0e7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1a0e7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a0e7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a0e7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a0e7-115">Not supported.</span></span>|
|<span data-ttu-id="1a0e7-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="1a0e7-116">Application</span></span>|<span data-ttu-id="1a0e7-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a0e7-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a0e7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a0e7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="1a0e7-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1a0e7-119">Request headers</span></span>
|<span data-ttu-id="1a0e7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1a0e7-120">Header</span></span>|<span data-ttu-id="1a0e7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1a0e7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a0e7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a0e7-122">Authorization</span></span>|<span data-ttu-id="1a0e7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a0e7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a0e7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1a0e7-124">Accept</span></span>|<span data-ttu-id="1a0e7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1a0e7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a0e7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1a0e7-126">Request body</span></span>
<span data-ttu-id="1a0e7-127">В теле запроса укажите представление объекта windowsInformationProtectionAppLearningSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a0e7-127">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="1a0e7-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="1a0e7-128">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="1a0e7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a0e7-129">Property</span></span>|<span data-ttu-id="1a0e7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1a0e7-130">Type</span></span>|<span data-ttu-id="1a0e7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1a0e7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a0e7-132">id</span><span class="sxs-lookup"><span data-stu-id="1a0e7-132">id</span></span>|<span data-ttu-id="1a0e7-133">String</span><span class="sxs-lookup"><span data-stu-id="1a0e7-133">String</span></span>|<span data-ttu-id="1a0e7-134">Уникальный идентификатор объекта WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="1a0e7-134">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="1a0e7-135">applicationName</span><span class="sxs-lookup"><span data-stu-id="1a0e7-135">applicationName</span></span>|<span data-ttu-id="1a0e7-136">String</span><span class="sxs-lookup"><span data-stu-id="1a0e7-136">String</span></span>|<span data-ttu-id="1a0e7-137">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="1a0e7-137">Application Name</span></span>|
|<span data-ttu-id="1a0e7-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="1a0e7-138">applicationType</span></span>|[<span data-ttu-id="1a0e7-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="1a0e7-139">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="1a0e7-140">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="1a0e7-140">Application Type.</span></span> <span data-ttu-id="1a0e7-141">Возможные значения: `universal`, `desktop`.</span><span class="sxs-lookup"><span data-stu-id="1a0e7-141">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="1a0e7-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="1a0e7-142">deviceCount</span></span>|<span data-ttu-id="1a0e7-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1a0e7-143">Int32</span></span>|<span data-ttu-id="1a0e7-144">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="1a0e7-144">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="1a0e7-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a0e7-145">Response</span></span>
<span data-ttu-id="1a0e7-146">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1a0e7-146">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a0e7-147">Пример</span><span class="sxs-lookup"><span data-stu-id="1a0e7-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a0e7-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a0e7-148">Request</span></span>
<span data-ttu-id="1a0e7-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a0e7-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="1a0e7-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a0e7-150">Response</span></span>
<span data-ttu-id="1a0e7-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a0e7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




