---
title: Обновление deviceManagementConfigurationCategory
description: Обновление свойств объекта deviceManagementConfigurationCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40d253fdfd0756a7bca7045a758be95404bde594
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441575"
---
# <a name="update-devicemanagementconfigurationcategory"></a><span data-ttu-id="901a5-103">Обновление deviceManagementConfigurationCategory</span><span class="sxs-lookup"><span data-stu-id="901a5-103">Update deviceManagementConfigurationCategory</span></span>

<span data-ttu-id="901a5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="901a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="901a5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="901a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="901a5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="901a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="901a5-107">Обновление свойств объекта [deviceManagementConfigurationCategory.](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="901a5-107">Update the properties of a [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="901a5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="901a5-108">Prerequisites</span></span>
<span data-ttu-id="901a5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="901a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="901a5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="901a5-111">Permission type</span></span>|<span data-ttu-id="901a5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="901a5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="901a5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="901a5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="901a5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="901a5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="901a5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="901a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="901a5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="901a5-116">Not supported.</span></span>|
|<span data-ttu-id="901a5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="901a5-117">Application</span></span>|<span data-ttu-id="901a5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="901a5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="901a5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="901a5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationCategories/{deviceManagementConfigurationCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="901a5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="901a5-120">Request headers</span></span>
|<span data-ttu-id="901a5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="901a5-121">Header</span></span>|<span data-ttu-id="901a5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="901a5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="901a5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="901a5-123">Authorization</span></span>|<span data-ttu-id="901a5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="901a5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="901a5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="901a5-125">Accept</span></span>|<span data-ttu-id="901a5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="901a5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="901a5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="901a5-127">Request body</span></span>
<span data-ttu-id="901a5-128">В теле запроса поставляем представление JSON для [объекта deviceManagementConfigurationCategory.](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="901a5-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object.</span></span>

<span data-ttu-id="901a5-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementConfigurationCategory.](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="901a5-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md).</span></span>

|<span data-ttu-id="901a5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="901a5-130">Property</span></span>|<span data-ttu-id="901a5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="901a5-131">Type</span></span>|<span data-ttu-id="901a5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="901a5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="901a5-133">id</span><span class="sxs-lookup"><span data-stu-id="901a5-133">id</span></span>|<span data-ttu-id="901a5-134">String</span><span class="sxs-lookup"><span data-stu-id="901a5-134">String</span></span>|<span data-ttu-id="901a5-135">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="901a5-135">Identifier for item</span></span>|
|<span data-ttu-id="901a5-136">description</span><span class="sxs-lookup"><span data-stu-id="901a5-136">description</span></span>|<span data-ttu-id="901a5-137">String</span><span class="sxs-lookup"><span data-stu-id="901a5-137">String</span></span>|<span data-ttu-id="901a5-138">Описание элемента</span><span class="sxs-lookup"><span data-stu-id="901a5-138">Description of the item</span></span>|
|<span data-ttu-id="901a5-139">helpText</span><span class="sxs-lookup"><span data-stu-id="901a5-139">helpText</span></span>|<span data-ttu-id="901a5-140">String</span><span class="sxs-lookup"><span data-stu-id="901a5-140">String</span></span>|<span data-ttu-id="901a5-141">Справка текста элемента</span><span class="sxs-lookup"><span data-stu-id="901a5-141">Help text of the item</span></span>|
|<span data-ttu-id="901a5-142">name</span><span class="sxs-lookup"><span data-stu-id="901a5-142">name</span></span>|<span data-ttu-id="901a5-143">String</span><span class="sxs-lookup"><span data-stu-id="901a5-143">String</span></span>|<span data-ttu-id="901a5-144">Имя элемента</span><span class="sxs-lookup"><span data-stu-id="901a5-144">Name of the item</span></span>|
|<span data-ttu-id="901a5-145">displayName</span><span class="sxs-lookup"><span data-stu-id="901a5-145">displayName</span></span>|<span data-ttu-id="901a5-146">String</span><span class="sxs-lookup"><span data-stu-id="901a5-146">String</span></span>|<span data-ttu-id="901a5-147">Отображение имени элемента</span><span class="sxs-lookup"><span data-stu-id="901a5-147">Display name of the item</span></span>|
|<span data-ttu-id="901a5-148">платформы</span><span class="sxs-lookup"><span data-stu-id="901a5-148">platforms</span></span>|[<span data-ttu-id="901a5-149">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="901a5-149">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="901a5-150">Типы платформ, которые имеются в этой категории.</span><span class="sxs-lookup"><span data-stu-id="901a5-150">Platforms types, which settings in the category have.</span></span> <span data-ttu-id="901a5-151">Возможные значения: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="901a5-151">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="901a5-152">технологии</span><span class="sxs-lookup"><span data-stu-id="901a5-152">technologies</span></span>|[<span data-ttu-id="901a5-153">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="901a5-153">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="901a5-154">Типы технологий, которые имеют параметры в категории.</span><span class="sxs-lookup"><span data-stu-id="901a5-154">Technologies types, which settings in the category have.</span></span> <span data-ttu-id="901a5-155">Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="901a5-155">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|
|<span data-ttu-id="901a5-156">settingUsage</span><span class="sxs-lookup"><span data-stu-id="901a5-156">settingUsage</span></span>|[<span data-ttu-id="901a5-157">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="901a5-157">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="901a5-158">Указывает, что категория содержит параметры, используемые для соответствия требованиям или конфигурации.</span><span class="sxs-lookup"><span data-stu-id="901a5-158">Indicates that the category contains settings that are used for Compliance or Configuration.</span></span> <span data-ttu-id="901a5-159">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="901a5-159">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="901a5-160">parentCategoryId</span><span class="sxs-lookup"><span data-stu-id="901a5-160">parentCategoryId</span></span>|<span data-ttu-id="901a5-161">String</span><span class="sxs-lookup"><span data-stu-id="901a5-161">String</span></span>|<span data-ttu-id="901a5-162">Родительский id категории.</span><span class="sxs-lookup"><span data-stu-id="901a5-162">Parent id of the category.</span></span>|
|<span data-ttu-id="901a5-163">rootCategoryId</span><span class="sxs-lookup"><span data-stu-id="901a5-163">rootCategoryId</span></span>|<span data-ttu-id="901a5-164">String</span><span class="sxs-lookup"><span data-stu-id="901a5-164">String</span></span>|<span data-ttu-id="901a5-165">Корневой id категории.</span><span class="sxs-lookup"><span data-stu-id="901a5-165">Root id of the category.</span></span>|
|<span data-ttu-id="901a5-166">childCategoryIds</span><span class="sxs-lookup"><span data-stu-id="901a5-166">childCategoryIds</span></span>|<span data-ttu-id="901a5-167">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="901a5-167">String collection</span></span>|<span data-ttu-id="901a5-168">Список детских ids этой категории.</span><span class="sxs-lookup"><span data-stu-id="901a5-168">List of child ids of the category.</span></span>|



## <a name="response"></a><span data-ttu-id="901a5-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="901a5-169">Response</span></span>
<span data-ttu-id="901a5-170">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="901a5-170">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="901a5-171">Пример</span><span class="sxs-lookup"><span data-stu-id="901a5-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="901a5-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="901a5-172">Request</span></span>
<span data-ttu-id="901a5-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="901a5-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationCategories/{deviceManagementConfigurationCategoryId}
Content-type: application/json
Content-length: 465

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "platforms": "macOS",
  "technologies": "mdm",
  "settingUsage": "configuration",
  "parentCategoryId": "Parent Category Id value",
  "rootCategoryId": "Root Category Id value",
  "childCategoryIds": [
    "Child Category Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="901a5-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="901a5-174">Response</span></span>
<span data-ttu-id="901a5-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="901a5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 514

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "id": "cff34dd2-4dd2-cff3-d24d-f3cfd24df3cf",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "platforms": "macOS",
  "technologies": "mdm",
  "settingUsage": "configuration",
  "parentCategoryId": "Parent Category Id value",
  "rootCategoryId": "Root Category Id value",
  "childCategoryIds": [
    "Child Category Ids value"
  ]
}
```




