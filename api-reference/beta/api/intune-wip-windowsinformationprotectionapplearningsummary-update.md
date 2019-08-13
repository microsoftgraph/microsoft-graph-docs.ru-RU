---
title: Обновление объекта windowsInformationProtectionAppLearningSummary
description: Обновление свойств объекта windowsInformationProtectionAppLearningSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 372e99c3557022c4e1856c496fc6068e59ba8169
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343029"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="ddbeb-103">Обновление объекта windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="ddbeb-103">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="ddbeb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddbeb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddbeb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ddbeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddbeb-106">Обновление свойств объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="ddbeb-106">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddbeb-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ddbeb-107">Prerequisites</span></span>
<span data-ttu-id="ddbeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddbeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddbeb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddbeb-110">Permission type</span></span>|<span data-ttu-id="ddbeb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddbeb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddbeb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddbeb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ddbeb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddbeb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ddbeb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddbeb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddbeb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddbeb-115">Not supported.</span></span>|
|<span data-ttu-id="ddbeb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ddbeb-116">Application</span></span>|<span data-ttu-id="ddbeb-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddbeb-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddbeb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddbeb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="ddbeb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ddbeb-119">Request headers</span></span>
|<span data-ttu-id="ddbeb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ddbeb-120">Header</span></span>|<span data-ttu-id="ddbeb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ddbeb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddbeb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ddbeb-122">Authorization</span></span>|<span data-ttu-id="ddbeb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddbeb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddbeb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ddbeb-124">Accept</span></span>|<span data-ttu-id="ddbeb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ddbeb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddbeb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ddbeb-126">Request body</span></span>
<span data-ttu-id="ddbeb-127">В теле запроса укажите представление объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ddbeb-127">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="ddbeb-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="ddbeb-128">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="ddbeb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ddbeb-129">Property</span></span>|<span data-ttu-id="ddbeb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ddbeb-130">Type</span></span>|<span data-ttu-id="ddbeb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ddbeb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddbeb-132">id</span><span class="sxs-lookup"><span data-stu-id="ddbeb-132">id</span></span>|<span data-ttu-id="ddbeb-133">String</span><span class="sxs-lookup"><span data-stu-id="ddbeb-133">String</span></span>|<span data-ttu-id="ddbeb-134">Уникальный идентификатор объекта WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="ddbeb-134">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="ddbeb-135">applicationName</span><span class="sxs-lookup"><span data-stu-id="ddbeb-135">applicationName</span></span>|<span data-ttu-id="ddbeb-136">String</span><span class="sxs-lookup"><span data-stu-id="ddbeb-136">String</span></span>|<span data-ttu-id="ddbeb-137">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="ddbeb-137">Application Name</span></span>|
|<span data-ttu-id="ddbeb-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="ddbeb-138">applicationType</span></span>|[<span data-ttu-id="ddbeb-139">аппликатионтипе</span><span class="sxs-lookup"><span data-stu-id="ddbeb-139">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="ddbeb-140">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="ddbeb-140">Application Type.</span></span> <span data-ttu-id="ddbeb-141">Возможные значения: `universal`, `desktop`.</span><span class="sxs-lookup"><span data-stu-id="ddbeb-141">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="ddbeb-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="ddbeb-142">deviceCount</span></span>|<span data-ttu-id="ddbeb-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ddbeb-143">Int32</span></span>|<span data-ttu-id="ddbeb-144">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="ddbeb-144">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="ddbeb-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddbeb-145">Response</span></span>
<span data-ttu-id="ddbeb-146">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ddbeb-146">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddbeb-147">Пример</span><span class="sxs-lookup"><span data-stu-id="ddbeb-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddbeb-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddbeb-148">Request</span></span>
<span data-ttu-id="ddbeb-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddbeb-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ddbeb-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddbeb-150">Response</span></span>
<span data-ttu-id="ddbeb-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ddbeb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






