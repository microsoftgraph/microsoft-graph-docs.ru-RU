---
title: Обновление объекта windowsInformationProtectionAppLearningSummary
description: Обновление свойств объекта windowsInformationProtectionAppLearningSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 86d8ab048b81401fd3d4378000af89d06a7fcb5f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541159"
---
# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="e0a71-103">Обновление объекта windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="e0a71-103">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="e0a71-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0a71-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0a71-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0a71-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0a71-106">Обновление свойств объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="e0a71-106">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0a71-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e0a71-107">Prerequisites</span></span>
<span data-ttu-id="e0a71-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0a71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0a71-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0a71-110">Permission type</span></span>|<span data-ttu-id="e0a71-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0a71-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0a71-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0a71-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e0a71-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0a71-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e0a71-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0a71-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0a71-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0a71-115">Not supported.</span></span>|
|<span data-ttu-id="e0a71-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0a71-116">Application</span></span>|<span data-ttu-id="e0a71-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0a71-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0a71-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0a71-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="e0a71-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0a71-119">Request headers</span></span>
|<span data-ttu-id="e0a71-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e0a71-120">Header</span></span>|<span data-ttu-id="e0a71-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e0a71-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0a71-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0a71-122">Authorization</span></span>|<span data-ttu-id="e0a71-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0a71-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0a71-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e0a71-124">Accept</span></span>|<span data-ttu-id="e0a71-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e0a71-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0a71-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e0a71-126">Request body</span></span>
<span data-ttu-id="e0a71-127">В теле запроса укажите представление объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0a71-127">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="e0a71-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span><span class="sxs-lookup"><span data-stu-id="e0a71-128">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="e0a71-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0a71-129">Property</span></span>|<span data-ttu-id="e0a71-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e0a71-130">Type</span></span>|<span data-ttu-id="e0a71-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e0a71-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0a71-132">id</span><span class="sxs-lookup"><span data-stu-id="e0a71-132">id</span></span>|<span data-ttu-id="e0a71-133">String</span><span class="sxs-lookup"><span data-stu-id="e0a71-133">String</span></span>|<span data-ttu-id="e0a71-134">Уникальный идентификатор объекта WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="e0a71-134">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="e0a71-135">applicationName</span><span class="sxs-lookup"><span data-stu-id="e0a71-135">applicationName</span></span>|<span data-ttu-id="e0a71-136">String</span><span class="sxs-lookup"><span data-stu-id="e0a71-136">String</span></span>|<span data-ttu-id="e0a71-137">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="e0a71-137">Application Name</span></span>|
|<span data-ttu-id="e0a71-138">applicationType</span><span class="sxs-lookup"><span data-stu-id="e0a71-138">applicationType</span></span>|[<span data-ttu-id="e0a71-139">Аппликатионтипе</span><span class="sxs-lookup"><span data-stu-id="e0a71-139">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="e0a71-140">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="e0a71-140">Application Type.</span></span> <span data-ttu-id="e0a71-141">Возможные значения: `universal`, `desktop`.</span><span class="sxs-lookup"><span data-stu-id="e0a71-141">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="e0a71-142">deviceCount</span><span class="sxs-lookup"><span data-stu-id="e0a71-142">deviceCount</span></span>|<span data-ttu-id="e0a71-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e0a71-143">Int32</span></span>|<span data-ttu-id="e0a71-144">Количество устройств</span><span class="sxs-lookup"><span data-stu-id="e0a71-144">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="e0a71-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0a71-145">Response</span></span>
<span data-ttu-id="e0a71-146">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e0a71-146">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0a71-147">Пример</span><span class="sxs-lookup"><span data-stu-id="e0a71-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0a71-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0a71-148">Request</span></span>
<span data-ttu-id="e0a71-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0a71-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e0a71-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0a71-150">Response</span></span>
<span data-ttu-id="e0a71-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0a71-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





