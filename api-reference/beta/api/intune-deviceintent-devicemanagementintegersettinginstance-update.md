---
title: Обновление Девицеманажементинтежерсеттингинстанце
description: Обновление свойств объекта Девицеманажементинтежерсеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8588e2f41f2c465547b6163ab6df010c0368b4f1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48047709"
---
# <a name="update-devicemanagementintegersettinginstance"></a><span data-ttu-id="86fcb-103">Обновление Девицеманажементинтежерсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="86fcb-103">Update deviceManagementIntegerSettingInstance</span></span>

<span data-ttu-id="86fcb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86fcb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86fcb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86fcb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86fcb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86fcb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86fcb-107">Обновление свойств объекта [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="86fcb-107">Update the properties of a [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86fcb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="86fcb-108">Prerequisites</span></span>
<span data-ttu-id="86fcb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86fcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86fcb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86fcb-111">Permission type</span></span>|<span data-ttu-id="86fcb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="86fcb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86fcb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86fcb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86fcb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86fcb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86fcb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86fcb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86fcb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86fcb-116">Not supported.</span></span>|
|<span data-ttu-id="86fcb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86fcb-117">Application</span></span>|<span data-ttu-id="86fcb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86fcb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86fcb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86fcb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/settings/{deviceManagementSettingInstanceId}
PATCH /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings/{deviceManagementSettingInstanceId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings/{deviceManagementSettingInstanceId}
```

## <a name="request-headers"></a><span data-ttu-id="86fcb-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="86fcb-120">Request headers</span></span>
|<span data-ttu-id="86fcb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86fcb-121">Header</span></span>|<span data-ttu-id="86fcb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="86fcb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86fcb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="86fcb-123">Authorization</span></span>|<span data-ttu-id="86fcb-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86fcb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86fcb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="86fcb-125">Accept</span></span>|<span data-ttu-id="86fcb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86fcb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86fcb-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="86fcb-127">Request body</span></span>
<span data-ttu-id="86fcb-128">В тексте запроса добавьте представление объекта [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86fcb-128">In the request body, supply a JSON representation for the [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

<span data-ttu-id="86fcb-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="86fcb-129">The following table shows the properties that are required when you create the [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md).</span></span>

|<span data-ttu-id="86fcb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="86fcb-130">Property</span></span>|<span data-ttu-id="86fcb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="86fcb-131">Type</span></span>|<span data-ttu-id="86fcb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="86fcb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86fcb-133">id</span><span class="sxs-lookup"><span data-stu-id="86fcb-133">id</span></span>|<span data-ttu-id="86fcb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="86fcb-134">String</span></span>|<span data-ttu-id="86fcb-135">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="86fcb-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="86fcb-136">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="86fcb-136">definitionId</span></span>|<span data-ttu-id="86fcb-137">Строка</span><span class="sxs-lookup"><span data-stu-id="86fcb-137">String</span></span>|<span data-ttu-id="86fcb-138">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="86fcb-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="86fcb-139">валуежсон</span><span class="sxs-lookup"><span data-stu-id="86fcb-139">valueJson</span></span>|<span data-ttu-id="86fcb-140">Строка</span><span class="sxs-lookup"><span data-stu-id="86fcb-140">String</span></span>|<span data-ttu-id="86fcb-141">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="86fcb-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="86fcb-142">value</span><span class="sxs-lookup"><span data-stu-id="86fcb-142">value</span></span>|<span data-ttu-id="86fcb-143">Int32</span><span class="sxs-lookup"><span data-stu-id="86fcb-143">Int32</span></span>|<span data-ttu-id="86fcb-144">Целое значение</span><span class="sxs-lookup"><span data-stu-id="86fcb-144">The integer value</span></span>|



## <a name="response"></a><span data-ttu-id="86fcb-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="86fcb-145">Response</span></span>
<span data-ttu-id="86fcb-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="86fcb-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86fcb-147">Пример</span><span class="sxs-lookup"><span data-stu-id="86fcb-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="86fcb-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="86fcb-148">Request</span></span>
<span data-ttu-id="86fcb-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86fcb-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="86fcb-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="86fcb-150">Response</span></span>
<span data-ttu-id="86fcb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86fcb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "id": "60468ce7-8ce7-6046-e78c-4660e78c4660",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": 5
}
```






