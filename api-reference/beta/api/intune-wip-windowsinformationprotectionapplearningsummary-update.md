---
title: Обновление объекта windowsInformationProtectionAppLearningSummary
description: Обновление свойств объекта windowsInformationProtectionAppLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 400bb44f1398a14f6b41a36b9ef2a785631643d6
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "43451942"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="e9a82-103">Обновление объекта windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="e9a82-103">Update windowsInformationProtectionAppLearningSummary</span></span>

<span data-ttu-id="e9a82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9a82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9a82-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9a82-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9a82-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e9a82-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9a82-107">Обновление свойств объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="e9a82-107">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9a82-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e9a82-108">Prerequisites</span></span>
<span data-ttu-id="e9a82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9a82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9a82-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9a82-111">Permission type</span></span>|<span data-ttu-id="e9a82-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9a82-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9a82-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9a82-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9a82-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9a82-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e9a82-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9a82-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9a82-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9a82-116">Not supported.</span></span>|
|<span data-ttu-id="e9a82-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9a82-117">Application</span></span>|<span data-ttu-id="e9a82-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9a82-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9a82-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9a82-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="e9a82-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e9a82-120">Request headers</span></span>
|<span data-ttu-id="e9a82-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e9a82-121">Header</span></span>|<span data-ttu-id="e9a82-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e9a82-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9a82-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9a82-123">Authorization</span></span>|<span data-ttu-id="e9a82-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9a82-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9a82-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e9a82-125">Accept</span></span>|<span data-ttu-id="e9a82-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9a82-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9a82-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9a82-127">Request body</span></span>
<span data-ttu-id="e9a82-128">В теле запроса укажите представление объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9a82-128">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="e9a82-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="e9a82-129">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="e9a82-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9a82-130">Property</span></span>|<span data-ttu-id="e9a82-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e9a82-131">Type</span></span>|<span data-ttu-id="e9a82-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e9a82-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9a82-133">id</span><span class="sxs-lookup"><span data-stu-id="e9a82-133">id</span></span>|<span data-ttu-id="e9a82-134">String</span><span class="sxs-lookup"><span data-stu-id="e9a82-134">String</span></span>|<span data-ttu-id="e9a82-135">Уникальный идентификатор объекта WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="e9a82-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="e9a82-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="e9a82-136">applicationName</span></span>|<span data-ttu-id="e9a82-137">String</span><span class="sxs-lookup"><span data-stu-id="e9a82-137">String</span></span>|<span data-ttu-id="e9a82-138">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="e9a82-138">Application Name</span></span>|
|<span data-ttu-id="e9a82-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="e9a82-139">applicationType</span></span>|[<span data-ttu-id="e9a82-140">аппликатионтипе</span><span class="sxs-lookup"><span data-stu-id="e9a82-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="e9a82-141">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="e9a82-141">Application Type.</span></span> <span data-ttu-id="e9a82-142">Возможные значения: `universal`, `desktop`.</span><span class="sxs-lookup"><span data-stu-id="e9a82-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="e9a82-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="e9a82-143">deviceCount</span></span>|<span data-ttu-id="e9a82-144">Int32</span><span class="sxs-lookup"><span data-stu-id="e9a82-144">Int32</span></span>|<span data-ttu-id="e9a82-145">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="e9a82-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="e9a82-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9a82-146">Response</span></span>
<span data-ttu-id="e9a82-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e9a82-147">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9a82-148">Пример</span><span class="sxs-lookup"><span data-stu-id="e9a82-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9a82-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9a82-149">Request</span></span>
<span data-ttu-id="e9a82-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9a82-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="e9a82-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9a82-151">Response</span></span>
<span data-ttu-id="e9a82-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9a82-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



