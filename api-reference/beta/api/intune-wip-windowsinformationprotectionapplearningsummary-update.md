---
title: Обновление объекта windowsInformationProtectionAppLearningSummary
description: Обновление свойств объекта windowsInformationProtectionAppLearningSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 39a67f1df2e2550613535bcbbea86e971f52bf7d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39938182"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="01670-103">Обновление объекта windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="01670-103">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="01670-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01670-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01670-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01670-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01670-106">Обновление свойств объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="01670-106">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01670-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="01670-107">Prerequisites</span></span>
<span data-ttu-id="01670-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01670-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01670-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01670-110">Permission type</span></span>|<span data-ttu-id="01670-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="01670-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01670-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01670-112">Delegated (work or school account)</span></span>|<span data-ttu-id="01670-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01670-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="01670-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01670-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01670-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01670-115">Not supported.</span></span>|
|<span data-ttu-id="01670-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01670-116">Application</span></span>|<span data-ttu-id="01670-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01670-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01670-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01670-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="01670-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="01670-119">Request headers</span></span>
|<span data-ttu-id="01670-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01670-120">Header</span></span>|<span data-ttu-id="01670-121">Значение</span><span class="sxs-lookup"><span data-stu-id="01670-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01670-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01670-122">Authorization</span></span>|<span data-ttu-id="01670-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01670-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01670-124">Accept</span><span class="sxs-lookup"><span data-stu-id="01670-124">Accept</span></span>|<span data-ttu-id="01670-125">application/json</span><span class="sxs-lookup"><span data-stu-id="01670-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01670-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="01670-126">Request body</span></span>
<span data-ttu-id="01670-127">В теле запроса укажите представление объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01670-127">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="01670-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="01670-128">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="01670-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="01670-129">Property</span></span>|<span data-ttu-id="01670-130">Тип</span><span class="sxs-lookup"><span data-stu-id="01670-130">Type</span></span>|<span data-ttu-id="01670-131">Описание</span><span class="sxs-lookup"><span data-stu-id="01670-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01670-132">id</span><span class="sxs-lookup"><span data-stu-id="01670-132">id</span></span>|<span data-ttu-id="01670-133">Строка</span><span class="sxs-lookup"><span data-stu-id="01670-133">String</span></span>|<span data-ttu-id="01670-134">Уникальный идентификатор объекта WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="01670-134">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="01670-135">applicationName</span><span class="sxs-lookup"><span data-stu-id="01670-135">applicationName</span></span>|<span data-ttu-id="01670-136">String</span><span class="sxs-lookup"><span data-stu-id="01670-136">String</span></span>|<span data-ttu-id="01670-137">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="01670-137">Application Name</span></span>|
|<span data-ttu-id="01670-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="01670-138">applicationType</span></span>|[<span data-ttu-id="01670-139">аппликатионтипе</span><span class="sxs-lookup"><span data-stu-id="01670-139">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="01670-140">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="01670-140">Application Type.</span></span> <span data-ttu-id="01670-141">Возможные значения: `universal`, `desktop`.</span><span class="sxs-lookup"><span data-stu-id="01670-141">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="01670-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="01670-142">deviceCount</span></span>|<span data-ttu-id="01670-143">Int32</span><span class="sxs-lookup"><span data-stu-id="01670-143">Int32</span></span>|<span data-ttu-id="01670-144">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="01670-144">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="01670-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="01670-145">Response</span></span>
<span data-ttu-id="01670-146">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="01670-146">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01670-147">Пример</span><span class="sxs-lookup"><span data-stu-id="01670-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="01670-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="01670-148">Request</span></span>
<span data-ttu-id="01670-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01670-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="01670-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="01670-150">Response</span></span>
<span data-ttu-id="01670-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01670-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





