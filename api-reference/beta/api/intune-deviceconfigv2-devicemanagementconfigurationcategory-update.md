---
title: Обновление Девицеманажементконфигуратионкатегори
description: Обновление свойств объекта Девицеманажементконфигуратионкатегори.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e695f9935905d781d7d6ca3e8a8e36f1cfc36c74
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242151"
---
# <a name="update-devicemanagementconfigurationcategory"></a><span data-ttu-id="decc4-103">Обновление Девицеманажементконфигуратионкатегори</span><span class="sxs-lookup"><span data-stu-id="decc4-103">Update deviceManagementConfigurationCategory</span></span>

<span data-ttu-id="decc4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="decc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="decc4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="decc4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="decc4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="decc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="decc4-107">Обновление свойств объекта [девицеманажементконфигуратионкатегори](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="decc4-107">Update the properties of a [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="decc4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="decc4-108">Prerequisites</span></span>
<span data-ttu-id="decc4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="decc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="decc4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="decc4-111">Permission type</span></span>|<span data-ttu-id="decc4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="decc4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="decc4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="decc4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="decc4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="decc4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="decc4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="decc4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="decc4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="decc4-116">Not supported.</span></span>|
|<span data-ttu-id="decc4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="decc4-117">Application</span></span>|<span data-ttu-id="decc4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="decc4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="decc4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="decc4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationCategories/{deviceManagementConfigurationCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="decc4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="decc4-120">Request headers</span></span>
|<span data-ttu-id="decc4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="decc4-121">Header</span></span>|<span data-ttu-id="decc4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="decc4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="decc4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="decc4-123">Authorization</span></span>|<span data-ttu-id="decc4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="decc4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="decc4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="decc4-125">Accept</span></span>|<span data-ttu-id="decc4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="decc4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="decc4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="decc4-127">Request body</span></span>
<span data-ttu-id="decc4-128">В тексте запроса добавьте представление объекта [девицеманажементконфигуратионкатегори](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="decc4-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object.</span></span>

<span data-ttu-id="decc4-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементконфигуратионкатегори](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md).</span><span class="sxs-lookup"><span data-stu-id="decc4-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md).</span></span>

|<span data-ttu-id="decc4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="decc4-130">Property</span></span>|<span data-ttu-id="decc4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="decc4-131">Type</span></span>|<span data-ttu-id="decc4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="decc4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="decc4-133">id</span><span class="sxs-lookup"><span data-stu-id="decc4-133">id</span></span>|<span data-ttu-id="decc4-134">String</span><span class="sxs-lookup"><span data-stu-id="decc4-134">String</span></span>|<span data-ttu-id="decc4-135">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="decc4-135">Identifier for item</span></span>|
|<span data-ttu-id="decc4-136">description</span><span class="sxs-lookup"><span data-stu-id="decc4-136">description</span></span>|<span data-ttu-id="decc4-137">String</span><span class="sxs-lookup"><span data-stu-id="decc4-137">String</span></span>|<span data-ttu-id="decc4-138">Описание элемента</span><span class="sxs-lookup"><span data-stu-id="decc4-138">Description of the item</span></span>|
|<span data-ttu-id="decc4-139">helpText</span><span class="sxs-lookup"><span data-stu-id="decc4-139">helpText</span></span>|<span data-ttu-id="decc4-140">String</span><span class="sxs-lookup"><span data-stu-id="decc4-140">String</span></span>|<span data-ttu-id="decc4-141">Текст справки элемента</span><span class="sxs-lookup"><span data-stu-id="decc4-141">Help text of the item</span></span>|
|<span data-ttu-id="decc4-142">name</span><span class="sxs-lookup"><span data-stu-id="decc4-142">name</span></span>|<span data-ttu-id="decc4-143">String</span><span class="sxs-lookup"><span data-stu-id="decc4-143">String</span></span>|<span data-ttu-id="decc4-144">Имя элемента</span><span class="sxs-lookup"><span data-stu-id="decc4-144">Name of the item</span></span>|
|<span data-ttu-id="decc4-145">displayName</span><span class="sxs-lookup"><span data-stu-id="decc4-145">displayName</span></span>|<span data-ttu-id="decc4-146">String</span><span class="sxs-lookup"><span data-stu-id="decc4-146">String</span></span>|<span data-ttu-id="decc4-147">Отображаемое имя элемента</span><span class="sxs-lookup"><span data-stu-id="decc4-147">Display name of the item</span></span>|
|<span data-ttu-id="decc4-148">Embedded</span><span class="sxs-lookup"><span data-stu-id="decc4-148">platforms</span></span>|[<span data-ttu-id="decc4-149">девицеманажементконфигуратионплатформс</span><span class="sxs-lookup"><span data-stu-id="decc4-149">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="decc4-150">Типы платформ, которые имеют параметры в категории.</span><span class="sxs-lookup"><span data-stu-id="decc4-150">Platforms types, which settings in the category have.</span></span> <span data-ttu-id="decc4-151">Возможные значения: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="decc4-151">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="decc4-152">технологически</span><span class="sxs-lookup"><span data-stu-id="decc4-152">technologies</span></span>|[<span data-ttu-id="decc4-153">девицеманажементконфигуратионтечнологиес</span><span class="sxs-lookup"><span data-stu-id="decc4-153">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="decc4-154">Типы технологий, которые имеют параметры в категории.</span><span class="sxs-lookup"><span data-stu-id="decc4-154">Technologies types, which settings in the category have.</span></span> <span data-ttu-id="decc4-155">Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="decc4-155">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|



## <a name="response"></a><span data-ttu-id="decc4-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="decc4-156">Response</span></span>
<span data-ttu-id="decc4-157">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементконфигуратионкатегори](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="decc4-157">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="decc4-158">Пример</span><span class="sxs-lookup"><span data-stu-id="decc4-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="decc4-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="decc4-159">Request</span></span>
<span data-ttu-id="decc4-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="decc4-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationCategories/{deviceManagementConfigurationCategoryId}
Content-type: application/json
Content-length: 268

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "platforms": "macOS",
  "technologies": "mdm"
}
```

### <a name="response"></a><span data-ttu-id="decc4-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="decc4-161">Response</span></span>
<span data-ttu-id="decc4-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="decc4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "id": "cff34dd2-4dd2-cff3-d24d-f3cfd24df3cf",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "platforms": "macOS",
  "technologies": "mdm"
}
```




