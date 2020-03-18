---
title: Обновление Девицеманажементабстракткомплекссеттингинстанце
description: Обновление свойств объекта Девицеманажементабстракткомплекссеттингинстанце.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6a132f0b1097b22c9fa57f924d9deebd71e8ccf4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42731147"
---
# <a name="update-devicemanagementabstractcomplexsettinginstance"></a><span data-ttu-id="0eda4-103">Обновление Девицеманажементабстракткомплекссеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="0eda4-103">Update deviceManagementAbstractComplexSettingInstance</span></span>

> <span data-ttu-id="0eda4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0eda4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0eda4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0eda4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0eda4-106">Обновление свойств объекта [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="0eda4-106">Update the properties of a [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0eda4-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0eda4-107">Prerequisites</span></span>
<span data-ttu-id="0eda4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0eda4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0eda4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0eda4-110">Permission type</span></span>|<span data-ttu-id="0eda4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0eda4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0eda4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0eda4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0eda4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eda4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0eda4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0eda4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0eda4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0eda4-115">Not supported.</span></span>|
|<span data-ttu-id="0eda4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0eda4-116">Application</span></span>|<span data-ttu-id="0eda4-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eda4-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0eda4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0eda4-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="0eda4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0eda4-119">Request headers</span></span>
|<span data-ttu-id="0eda4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0eda4-120">Header</span></span>|<span data-ttu-id="0eda4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0eda4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0eda4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0eda4-122">Authorization</span></span>|<span data-ttu-id="0eda4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0eda4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0eda4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0eda4-124">Accept</span></span>|<span data-ttu-id="0eda4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0eda4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0eda4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0eda4-126">Request body</span></span>
<span data-ttu-id="0eda4-127">В тексте запроса добавьте представление объекта [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0eda4-127">In the request body, supply a JSON representation for the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

<span data-ttu-id="0eda4-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="0eda4-128">The following table shows the properties that are required when you create the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md).</span></span>

|<span data-ttu-id="0eda4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0eda4-129">Property</span></span>|<span data-ttu-id="0eda4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0eda4-130">Type</span></span>|<span data-ttu-id="0eda4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0eda4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0eda4-132">id</span><span class="sxs-lookup"><span data-stu-id="0eda4-132">id</span></span>|<span data-ttu-id="0eda4-133">String</span><span class="sxs-lookup"><span data-stu-id="0eda4-133">String</span></span>|<span data-ttu-id="0eda4-134">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="0eda4-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="0eda4-135">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="0eda4-135">definitionId</span></span>|<span data-ttu-id="0eda4-136">String</span><span class="sxs-lookup"><span data-stu-id="0eda4-136">String</span></span>|<span data-ttu-id="0eda4-137">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="0eda4-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="0eda4-138">валуежсон</span><span class="sxs-lookup"><span data-stu-id="0eda4-138">valueJson</span></span>|<span data-ttu-id="0eda4-139">String</span><span class="sxs-lookup"><span data-stu-id="0eda4-139">String</span></span>|<span data-ttu-id="0eda4-140">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="0eda4-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="0eda4-141">имплементатионид</span><span class="sxs-lookup"><span data-stu-id="0eda4-141">implementationId</span></span>|<span data-ttu-id="0eda4-142">String</span><span class="sxs-lookup"><span data-stu-id="0eda4-142">String</span></span>|<span data-ttu-id="0eda4-143">Идентификатор определения для выбранной реализации этого сложного параметра</span><span class="sxs-lookup"><span data-stu-id="0eda4-143">The definition ID for the chosen implementation of this complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="0eda4-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="0eda4-144">Response</span></span>
<span data-ttu-id="0eda4-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0eda4-145">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0eda4-146">Пример</span><span class="sxs-lookup"><span data-stu-id="0eda4-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="0eda4-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="0eda4-147">Request</span></span>
<span data-ttu-id="0eda4-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0eda4-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0eda4-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="0eda4-149">Response</span></span>
<span data-ttu-id="0eda4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0eda4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




