---
title: Создание объекта windowsInformationProtectionAppLearningSummary
description: Создание объекта windowsInformationProtectionAppLearningSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 21d501e2edaf70bfc46ceeded315f7b65ac47634
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457386"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="4fb32-103">Создание объекта windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="4fb32-103">Create windowsInformationProtectionAppLearningSummary</span></span>

<span data-ttu-id="4fb32-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4fb32-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4fb32-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fb32-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fb32-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4fb32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fb32-107">Создание объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="4fb32-107">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fb32-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4fb32-108">Prerequisites</span></span>
<span data-ttu-id="4fb32-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fb32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fb32-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4fb32-111">Permission type</span></span>|<span data-ttu-id="4fb32-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4fb32-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fb32-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4fb32-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4fb32-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb32-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4fb32-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4fb32-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fb32-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fb32-116">Not supported.</span></span>|
|<span data-ttu-id="4fb32-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4fb32-117">Application</span></span>|<span data-ttu-id="4fb32-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb32-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fb32-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4fb32-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="4fb32-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4fb32-120">Request headers</span></span>
|<span data-ttu-id="4fb32-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4fb32-121">Header</span></span>|<span data-ttu-id="4fb32-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4fb32-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fb32-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fb32-123">Authorization</span></span>|<span data-ttu-id="4fb32-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4fb32-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fb32-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4fb32-125">Accept</span></span>|<span data-ttu-id="4fb32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4fb32-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fb32-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4fb32-127">Request body</span></span>
<span data-ttu-id="4fb32-128">В теле запроса укажите представление объекта windowsInformationProtectionAppLearningSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4fb32-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="4fb32-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="4fb32-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="4fb32-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4fb32-130">Property</span></span>|<span data-ttu-id="4fb32-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4fb32-131">Type</span></span>|<span data-ttu-id="4fb32-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4fb32-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fb32-133">id</span><span class="sxs-lookup"><span data-stu-id="4fb32-133">id</span></span>|<span data-ttu-id="4fb32-134">String</span><span class="sxs-lookup"><span data-stu-id="4fb32-134">String</span></span>|<span data-ttu-id="4fb32-135">Уникальный идентификатор объекта WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="4fb32-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="4fb32-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="4fb32-136">applicationName</span></span>|<span data-ttu-id="4fb32-137">String</span><span class="sxs-lookup"><span data-stu-id="4fb32-137">String</span></span>|<span data-ttu-id="4fb32-138">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="4fb32-138">Application Name</span></span>|
|<span data-ttu-id="4fb32-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="4fb32-139">applicationType</span></span>|[<span data-ttu-id="4fb32-140">аппликатионтипе</span><span class="sxs-lookup"><span data-stu-id="4fb32-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="4fb32-141">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="4fb32-141">Application Type.</span></span> <span data-ttu-id="4fb32-142">Возможные значения: `universal`, `desktop`.</span><span class="sxs-lookup"><span data-stu-id="4fb32-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="4fb32-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="4fb32-143">deviceCount</span></span>|<span data-ttu-id="4fb32-144">Int32</span><span class="sxs-lookup"><span data-stu-id="4fb32-144">Int32</span></span>|<span data-ttu-id="4fb32-145">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="4fb32-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="4fb32-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fb32-146">Response</span></span>
<span data-ttu-id="4fb32-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4fb32-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fb32-148">Пример</span><span class="sxs-lookup"><span data-stu-id="4fb32-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fb32-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="4fb32-149">Request</span></span>
<span data-ttu-id="4fb32-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4fb32-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="4fb32-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fb32-151">Response</span></span>
<span data-ttu-id="4fb32-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4fb32-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





