---
title: Обновление Девицеманажементабстракткомплекссеттингинстанце
description: Обновление свойств объекта Девицеманажементабстракткомплекссеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5feb4eccfd8594f7e8264a62a416bca4c8dd8f51
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47974396"
---
# <a name="update-devicemanagementabstractcomplexsettinginstance"></a><span data-ttu-id="40510-103">Обновление Девицеманажементабстракткомплекссеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="40510-103">Update deviceManagementAbstractComplexSettingInstance</span></span>

<span data-ttu-id="40510-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40510-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40510-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40510-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40510-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="40510-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40510-107">Обновление свойств объекта [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="40510-107">Update the properties of a [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40510-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="40510-108">Prerequisites</span></span>
<span data-ttu-id="40510-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40510-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40510-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40510-111">Permission type</span></span>|<span data-ttu-id="40510-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="40510-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40510-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40510-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40510-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40510-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="40510-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40510-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40510-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40510-116">Not supported.</span></span>|
|<span data-ttu-id="40510-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40510-117">Application</span></span>|<span data-ttu-id="40510-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40510-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40510-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40510-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="40510-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="40510-120">Request headers</span></span>
|<span data-ttu-id="40510-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40510-121">Header</span></span>|<span data-ttu-id="40510-122">Значение</span><span class="sxs-lookup"><span data-stu-id="40510-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40510-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="40510-123">Authorization</span></span>|<span data-ttu-id="40510-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40510-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40510-125">Accept</span><span class="sxs-lookup"><span data-stu-id="40510-125">Accept</span></span>|<span data-ttu-id="40510-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40510-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40510-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="40510-127">Request body</span></span>
<span data-ttu-id="40510-128">В тексте запроса добавьте представление объекта [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40510-128">In the request body, supply a JSON representation for the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

<span data-ttu-id="40510-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="40510-129">The following table shows the properties that are required when you create the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md).</span></span>

|<span data-ttu-id="40510-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="40510-130">Property</span></span>|<span data-ttu-id="40510-131">Тип</span><span class="sxs-lookup"><span data-stu-id="40510-131">Type</span></span>|<span data-ttu-id="40510-132">Описание</span><span class="sxs-lookup"><span data-stu-id="40510-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40510-133">id</span><span class="sxs-lookup"><span data-stu-id="40510-133">id</span></span>|<span data-ttu-id="40510-134">String</span><span class="sxs-lookup"><span data-stu-id="40510-134">String</span></span>|<span data-ttu-id="40510-135">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="40510-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="40510-136">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="40510-136">definitionId</span></span>|<span data-ttu-id="40510-137">String</span><span class="sxs-lookup"><span data-stu-id="40510-137">String</span></span>|<span data-ttu-id="40510-138">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="40510-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="40510-139">валуежсон</span><span class="sxs-lookup"><span data-stu-id="40510-139">valueJson</span></span>|<span data-ttu-id="40510-140">String</span><span class="sxs-lookup"><span data-stu-id="40510-140">String</span></span>|<span data-ttu-id="40510-141">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="40510-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="40510-142">имплементатионид</span><span class="sxs-lookup"><span data-stu-id="40510-142">implementationId</span></span>|<span data-ttu-id="40510-143">String</span><span class="sxs-lookup"><span data-stu-id="40510-143">String</span></span>|<span data-ttu-id="40510-144">Идентификатор определения для выбранной реализации этого сложного параметра</span><span class="sxs-lookup"><span data-stu-id="40510-144">The definition ID for the chosen implementation of this complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="40510-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="40510-145">Response</span></span>
<span data-ttu-id="40510-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40510-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40510-147">Пример</span><span class="sxs-lookup"><span data-stu-id="40510-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="40510-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="40510-148">Request</span></span>
<span data-ttu-id="40510-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40510-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 216

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "implementationId": "Implementation Id value"
}
```

### <a name="response"></a><span data-ttu-id="40510-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="40510-150">Response</span></span>
<span data-ttu-id="40510-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40510-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 265

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "id": "433e9565-9565-433e-6595-3e4365953e43",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "implementationId": "Implementation Id value"
}
```






