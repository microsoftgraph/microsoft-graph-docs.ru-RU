---
title: Обновление Девицеманажементабстракткомплекссеттингинстанце
description: Обновление свойств объекта Девицеманажементабстракткомплекссеттингинстанце.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 331854a1f04e6a42db904f9a7f66d12dde7b7cee
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49290401"
---
# <a name="update-devicemanagementabstractcomplexsettinginstance"></a><span data-ttu-id="958fa-103">Обновление Девицеманажементабстракткомплекссеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="958fa-103">Update deviceManagementAbstractComplexSettingInstance</span></span>

<span data-ttu-id="958fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="958fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="958fa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="958fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="958fa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="958fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="958fa-107">Обновление свойств объекта [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="958fa-107">Update the properties of a [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="958fa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="958fa-108">Prerequisites</span></span>
<span data-ttu-id="958fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="958fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="958fa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="958fa-111">Permission type</span></span>|<span data-ttu-id="958fa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="958fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="958fa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="958fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="958fa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="958fa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="958fa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="958fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="958fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="958fa-116">Not supported.</span></span>|
|<span data-ttu-id="958fa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="958fa-117">Application</span></span>|<span data-ttu-id="958fa-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="958fa-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="958fa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="958fa-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="958fa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="958fa-120">Request headers</span></span>
|<span data-ttu-id="958fa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="958fa-121">Header</span></span>|<span data-ttu-id="958fa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="958fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="958fa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="958fa-123">Authorization</span></span>|<span data-ttu-id="958fa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="958fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="958fa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="958fa-125">Accept</span></span>|<span data-ttu-id="958fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="958fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="958fa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="958fa-127">Request body</span></span>
<span data-ttu-id="958fa-128">В тексте запроса добавьте представление объекта [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="958fa-128">In the request body, supply a JSON representation for the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

<span data-ttu-id="958fa-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md).</span><span class="sxs-lookup"><span data-stu-id="958fa-129">The following table shows the properties that are required when you create the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md).</span></span>

|<span data-ttu-id="958fa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="958fa-130">Property</span></span>|<span data-ttu-id="958fa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="958fa-131">Type</span></span>|<span data-ttu-id="958fa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="958fa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="958fa-133">id</span><span class="sxs-lookup"><span data-stu-id="958fa-133">id</span></span>|<span data-ttu-id="958fa-134">String</span><span class="sxs-lookup"><span data-stu-id="958fa-134">String</span></span>|<span data-ttu-id="958fa-135">Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="958fa-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="958fa-136">дефинитионид</span><span class="sxs-lookup"><span data-stu-id="958fa-136">definitionId</span></span>|<span data-ttu-id="958fa-137">String</span><span class="sxs-lookup"><span data-stu-id="958fa-137">String</span></span>|<span data-ttu-id="958fa-138">Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="958fa-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="958fa-139">валуежсон</span><span class="sxs-lookup"><span data-stu-id="958fa-139">valueJson</span></span>|<span data-ttu-id="958fa-140">String</span><span class="sxs-lookup"><span data-stu-id="958fa-140">String</span></span>|<span data-ttu-id="958fa-141">Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="958fa-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="958fa-142">имплементатионид</span><span class="sxs-lookup"><span data-stu-id="958fa-142">implementationId</span></span>|<span data-ttu-id="958fa-143">String</span><span class="sxs-lookup"><span data-stu-id="958fa-143">String</span></span>|<span data-ttu-id="958fa-144">Идентификатор определения для выбранной реализации этого сложного параметра</span><span class="sxs-lookup"><span data-stu-id="958fa-144">The definition ID for the chosen implementation of this complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="958fa-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="958fa-145">Response</span></span>
<span data-ttu-id="958fa-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="958fa-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="958fa-147">Пример</span><span class="sxs-lookup"><span data-stu-id="958fa-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="958fa-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="958fa-148">Request</span></span>
<span data-ttu-id="958fa-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="958fa-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="958fa-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="958fa-150">Response</span></span>
<span data-ttu-id="958fa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="958fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




