---
title: Обновление Девицеманажементабстракткомплекссеттингинстанце
description: Обновление свойств объекта Девицеманажементабстракткомплекссеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e9fa9188e829931cf25d27e2ca972bd03e364e23
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43330453"
---
# <a name="update-devicemanagementabstractcomplexsettinginstance"></a><span data-ttu-id="ae1e5-103">Обновление Девицеманажементабстракткомплекссеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="ae1e5-103">Update deviceManagementAbstractComplexSettingInstance</span></span>

<span data-ttu-id="ae1e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae1e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae1e5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae1e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae1e5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae1e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae1e5-107">Обновление свойств объекта [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="ae1e5-107">Update the properties of a [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae1e5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ae1e5-108">Prerequisites</span></span>
<span data-ttu-id="ae1e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae1e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae1e5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae1e5-111">Permission type</span></span>|<span data-ttu-id="ae1e5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae1e5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae1e5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae1e5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae1e5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae1e5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae1e5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae1e5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae1e5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae1e5-116">Not supported.</span></span>|
|<span data-ttu-id="ae1e5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae1e5-117">Application</span></span>|<span data-ttu-id="ae1e5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae1e5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae1e5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae1e5-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="ae1e5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ae1e5-120">Request headers</span></span>
|<span data-ttu-id="ae1e5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ae1e5-121">Header</span></span>|<span data-ttu-id="ae1e5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ae1e5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae1e5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae1e5-123">Authorization</span></span>|<span data-ttu-id="ae1e5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae1e5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae1e5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ae1e5-125">Accept</span></span>|<span data-ttu-id="ae1e5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae1e5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae1e5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ae1e5-127">Request body</span></span>
<span data-ttu-id="ae1e5-128">В тексте запроса добавьте представление объекта [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae1e5-128">In the request body, supply a JSON representation for the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

<span data-ttu-id="ae1e5-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="ae1e5-129">The following table shows the properties that are required when you create the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md).</span></span>

|<span data-ttu-id="ae1e5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae1e5-130">Property</span></span>|<span data-ttu-id="ae1e5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ae1e5-131">Type</span></span>|<span data-ttu-id="ae1e5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ae1e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae1e5-133">id</span><span class="sxs-lookup"><span data-stu-id="ae1e5-133">id</span></span>|<span data-ttu-id="ae1e5-134">String</span><span class="sxs-lookup"><span data-stu-id="ae1e5-134">String</span></span>|<span data-ttu-id="ae1e5-135">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="ae1e5-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="ae1e5-136">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="ae1e5-136">definitionId</span></span>|<span data-ttu-id="ae1e5-137">String</span><span class="sxs-lookup"><span data-stu-id="ae1e5-137">String</span></span>|<span data-ttu-id="ae1e5-138">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="ae1e5-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="ae1e5-139">валуежсон</span><span class="sxs-lookup"><span data-stu-id="ae1e5-139">valueJson</span></span>|<span data-ttu-id="ae1e5-140">String</span><span class="sxs-lookup"><span data-stu-id="ae1e5-140">String</span></span>|<span data-ttu-id="ae1e5-141">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="ae1e5-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="ae1e5-142">имплементатионид</span><span class="sxs-lookup"><span data-stu-id="ae1e5-142">implementationId</span></span>|<span data-ttu-id="ae1e5-143">String</span><span class="sxs-lookup"><span data-stu-id="ae1e5-143">String</span></span>|<span data-ttu-id="ae1e5-144">Идентификатор определения для выбранной реализации этого сложного параметра</span><span class="sxs-lookup"><span data-stu-id="ae1e5-144">The definition ID for the chosen implementation of this complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="ae1e5-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="ae1e5-145">Response</span></span>
<span data-ttu-id="ae1e5-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ae1e5-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae1e5-147">Пример</span><span class="sxs-lookup"><span data-stu-id="ae1e5-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae1e5-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae1e5-148">Request</span></span>
<span data-ttu-id="ae1e5-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae1e5-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ae1e5-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae1e5-150">Response</span></span>
<span data-ttu-id="ae1e5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae1e5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



