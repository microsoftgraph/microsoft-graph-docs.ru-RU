---
title: Создание объекта windowsInformationProtectionAppLearningSummary
description: Создание объекта windowsInformationProtectionAppLearningSummary.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a31dc75af3b8ea00e41fade55f744acfedbd1fe8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451741"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="7004c-103">Создание объекта windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="7004c-103">Create windowsInformationProtectionAppLearningSummary</span></span>

<span data-ttu-id="7004c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7004c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7004c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7004c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7004c-106">Создание объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="7004c-106">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7004c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7004c-107">Prerequisites</span></span>
<span data-ttu-id="7004c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7004c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7004c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7004c-110">Permission type</span></span>|<span data-ttu-id="7004c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7004c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7004c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7004c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7004c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7004c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7004c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7004c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7004c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7004c-115">Not supported.</span></span>|
|<span data-ttu-id="7004c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7004c-116">Application</span></span>|<span data-ttu-id="7004c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7004c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7004c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7004c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="7004c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7004c-119">Request headers</span></span>
|<span data-ttu-id="7004c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7004c-120">Header</span></span>|<span data-ttu-id="7004c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7004c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7004c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7004c-122">Authorization</span></span>|<span data-ttu-id="7004c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7004c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7004c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7004c-124">Accept</span></span>|<span data-ttu-id="7004c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7004c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7004c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7004c-126">Request body</span></span>
<span data-ttu-id="7004c-127">В теле запроса укажите представление объекта windowsInformationProtectionAppLearningSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7004c-127">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="7004c-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="7004c-128">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="7004c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7004c-129">Property</span></span>|<span data-ttu-id="7004c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7004c-130">Type</span></span>|<span data-ttu-id="7004c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7004c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7004c-132">id</span><span class="sxs-lookup"><span data-stu-id="7004c-132">id</span></span>|<span data-ttu-id="7004c-133">String</span><span class="sxs-lookup"><span data-stu-id="7004c-133">String</span></span>|<span data-ttu-id="7004c-134">Уникальный идентификатор объекта WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="7004c-134">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="7004c-135">applicationName</span><span class="sxs-lookup"><span data-stu-id="7004c-135">applicationName</span></span>|<span data-ttu-id="7004c-136">String</span><span class="sxs-lookup"><span data-stu-id="7004c-136">String</span></span>|<span data-ttu-id="7004c-137">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="7004c-137">Application Name</span></span>|
|<span data-ttu-id="7004c-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="7004c-138">applicationType</span></span>|[<span data-ttu-id="7004c-139">аппликатионтипе</span><span class="sxs-lookup"><span data-stu-id="7004c-139">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="7004c-140">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="7004c-140">Application Type.</span></span> <span data-ttu-id="7004c-141">Возможные значения: `universal`, `desktop`.</span><span class="sxs-lookup"><span data-stu-id="7004c-141">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="7004c-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="7004c-142">deviceCount</span></span>|<span data-ttu-id="7004c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="7004c-143">Int32</span></span>|<span data-ttu-id="7004c-144">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="7004c-144">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="7004c-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="7004c-145">Response</span></span>
<span data-ttu-id="7004c-146">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7004c-146">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7004c-147">Пример</span><span class="sxs-lookup"><span data-stu-id="7004c-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="7004c-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="7004c-148">Request</span></span>
<span data-ttu-id="7004c-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7004c-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7004c-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="7004c-150">Response</span></span>
<span data-ttu-id="7004c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7004c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






