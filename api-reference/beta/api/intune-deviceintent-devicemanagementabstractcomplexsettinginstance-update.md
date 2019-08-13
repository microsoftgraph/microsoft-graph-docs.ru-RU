---
title: Обновление Девицеманажементабстракткомплекссеттингинстанце
description: Обновление свойств объекта Девицеманажементабстракткомплекссеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9ba2301f7c0df10f20238b44f64d3d22616f27a9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313526"
---
# <a name="update-devicemanagementabstractcomplexsettinginstance"></a><span data-ttu-id="45980-103">Обновление Девицеманажементабстракткомплекссеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="45980-103">Update deviceManagementAbstractComplexSettingInstance</span></span>

> <span data-ttu-id="45980-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45980-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45980-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45980-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45980-106">Обновление свойств объекта [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="45980-106">Update the properties of a [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45980-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="45980-107">Prerequisites</span></span>
<span data-ttu-id="45980-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45980-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45980-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45980-110">Permission type</span></span>|<span data-ttu-id="45980-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45980-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45980-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45980-112">Delegated (work or school account)</span></span>|<span data-ttu-id="45980-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45980-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="45980-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45980-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45980-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45980-115">Not supported.</span></span>|
|<span data-ttu-id="45980-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45980-116">Application</span></span>|<span data-ttu-id="45980-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45980-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45980-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45980-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="45980-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45980-119">Request headers</span></span>
|<span data-ttu-id="45980-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45980-120">Header</span></span>|<span data-ttu-id="45980-121">Значение</span><span class="sxs-lookup"><span data-stu-id="45980-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45980-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45980-122">Authorization</span></span>|<span data-ttu-id="45980-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45980-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45980-124">Accept</span><span class="sxs-lookup"><span data-stu-id="45980-124">Accept</span></span>|<span data-ttu-id="45980-125">application/json</span><span class="sxs-lookup"><span data-stu-id="45980-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45980-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="45980-126">Request body</span></span>
<span data-ttu-id="45980-127">В тексте запроса добавьте представление объекта [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45980-127">In the request body, supply a JSON representation for the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

<span data-ttu-id="45980-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="45980-128">The following table shows the properties that are required when you create the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md).</span></span>

|<span data-ttu-id="45980-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="45980-129">Property</span></span>|<span data-ttu-id="45980-130">Тип</span><span class="sxs-lookup"><span data-stu-id="45980-130">Type</span></span>|<span data-ttu-id="45980-131">Описание</span><span class="sxs-lookup"><span data-stu-id="45980-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45980-132">id</span><span class="sxs-lookup"><span data-stu-id="45980-132">id</span></span>|<span data-ttu-id="45980-133">String</span><span class="sxs-lookup"><span data-stu-id="45980-133">String</span></span>|<span data-ttu-id="45980-134">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="45980-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="45980-135">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="45980-135">definitionId</span></span>|<span data-ttu-id="45980-136">String</span><span class="sxs-lookup"><span data-stu-id="45980-136">String</span></span>|<span data-ttu-id="45980-137">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="45980-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="45980-138">валуежсон</span><span class="sxs-lookup"><span data-stu-id="45980-138">valueJson</span></span>|<span data-ttu-id="45980-139">String</span><span class="sxs-lookup"><span data-stu-id="45980-139">String</span></span>|<span data-ttu-id="45980-140">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="45980-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="45980-141">имплементатионид</span><span class="sxs-lookup"><span data-stu-id="45980-141">implementationId</span></span>|<span data-ttu-id="45980-142">String</span><span class="sxs-lookup"><span data-stu-id="45980-142">String</span></span>|<span data-ttu-id="45980-143">Идентификатор определения для выбранной реализации этого сложного параметра</span><span class="sxs-lookup"><span data-stu-id="45980-143">The definition ID for the chosen implementation of this complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="45980-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="45980-144">Response</span></span>
<span data-ttu-id="45980-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="45980-145">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45980-146">Пример</span><span class="sxs-lookup"><span data-stu-id="45980-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="45980-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="45980-147">Request</span></span>
<span data-ttu-id="45980-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45980-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="45980-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="45980-149">Response</span></span>
<span data-ttu-id="45980-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45980-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






