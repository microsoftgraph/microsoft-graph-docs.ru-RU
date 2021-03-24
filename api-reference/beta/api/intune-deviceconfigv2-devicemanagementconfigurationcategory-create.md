---
title: Создание deviceManagementConfigurationCategory
description: Создание нового объекта deviceManagementConfigurationCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cc4e659b9149347030344d10ecc02a4272c35832
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136897"
---
# <a name="create-devicemanagementconfigurationcategory"></a><span data-ttu-id="7813a-103">Создание deviceManagementConfigurationCategory</span><span class="sxs-lookup"><span data-stu-id="7813a-103">Create deviceManagementConfigurationCategory</span></span>

<span data-ttu-id="7813a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7813a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7813a-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7813a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7813a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7813a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7813a-107">Создание нового [объекта deviceManagementConfigurationCategory.](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="7813a-107">Create a new [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7813a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7813a-108">Prerequisites</span></span>
<span data-ttu-id="7813a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7813a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7813a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7813a-111">Permission type</span></span>|<span data-ttu-id="7813a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7813a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7813a-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7813a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7813a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7813a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7813a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7813a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7813a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7813a-116">Not supported.</span></span>|
|<span data-ttu-id="7813a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7813a-117">Application</span></span>|<span data-ttu-id="7813a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7813a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7813a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7813a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationCategories
```

## <a name="request-headers"></a><span data-ttu-id="7813a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7813a-120">Request headers</span></span>
|<span data-ttu-id="7813a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7813a-121">Header</span></span>|<span data-ttu-id="7813a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7813a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7813a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7813a-123">Authorization</span></span>|<span data-ttu-id="7813a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7813a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7813a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7813a-125">Accept</span></span>|<span data-ttu-id="7813a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7813a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7813a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7813a-127">Request body</span></span>
<span data-ttu-id="7813a-128">В теле запроса поставляем представление JSON для объекта deviceManagementConfigurationCategory.</span><span class="sxs-lookup"><span data-stu-id="7813a-128">In the request body, supply a JSON representation for the deviceManagementConfigurationCategory object.</span></span>

<span data-ttu-id="7813a-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementConfigurationCategory.</span><span class="sxs-lookup"><span data-stu-id="7813a-129">The following table shows the properties that are required when you create the deviceManagementConfigurationCategory.</span></span>

|<span data-ttu-id="7813a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7813a-130">Property</span></span>|<span data-ttu-id="7813a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7813a-131">Type</span></span>|<span data-ttu-id="7813a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7813a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7813a-133">id</span><span class="sxs-lookup"><span data-stu-id="7813a-133">id</span></span>|<span data-ttu-id="7813a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7813a-134">String</span></span>|<span data-ttu-id="7813a-135">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="7813a-135">Identifier for item</span></span>|
|<span data-ttu-id="7813a-136">description</span><span class="sxs-lookup"><span data-stu-id="7813a-136">description</span></span>|<span data-ttu-id="7813a-137">Строка</span><span class="sxs-lookup"><span data-stu-id="7813a-137">String</span></span>|<span data-ttu-id="7813a-138">Описание элемента</span><span class="sxs-lookup"><span data-stu-id="7813a-138">Description of the item</span></span>|
|<span data-ttu-id="7813a-139">helpText</span><span class="sxs-lookup"><span data-stu-id="7813a-139">helpText</span></span>|<span data-ttu-id="7813a-140">Строка</span><span class="sxs-lookup"><span data-stu-id="7813a-140">String</span></span>|<span data-ttu-id="7813a-141">Справка текста элемента</span><span class="sxs-lookup"><span data-stu-id="7813a-141">Help text of the item</span></span>|
|<span data-ttu-id="7813a-142">name</span><span class="sxs-lookup"><span data-stu-id="7813a-142">name</span></span>|<span data-ttu-id="7813a-143">String</span><span class="sxs-lookup"><span data-stu-id="7813a-143">String</span></span>|<span data-ttu-id="7813a-144">Имя элемента</span><span class="sxs-lookup"><span data-stu-id="7813a-144">Name of the item</span></span>|
|<span data-ttu-id="7813a-145">displayName</span><span class="sxs-lookup"><span data-stu-id="7813a-145">displayName</span></span>|<span data-ttu-id="7813a-146">Строка</span><span class="sxs-lookup"><span data-stu-id="7813a-146">String</span></span>|<span data-ttu-id="7813a-147">Отображение имени элемента</span><span class="sxs-lookup"><span data-stu-id="7813a-147">Display name of the item</span></span>|
|<span data-ttu-id="7813a-148">платформы</span><span class="sxs-lookup"><span data-stu-id="7813a-148">platforms</span></span>|[<span data-ttu-id="7813a-149">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="7813a-149">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="7813a-150">Типы платформ, которые имеются в этой категории.</span><span class="sxs-lookup"><span data-stu-id="7813a-150">Platforms types, which settings in the category have.</span></span> <span data-ttu-id="7813a-151">Возможные значения: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="7813a-151">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="7813a-152">технологии</span><span class="sxs-lookup"><span data-stu-id="7813a-152">technologies</span></span>|[<span data-ttu-id="7813a-153">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="7813a-153">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="7813a-154">Типы технологий, которые имеют параметры в категории.</span><span class="sxs-lookup"><span data-stu-id="7813a-154">Technologies types, which settings in the category have.</span></span> <span data-ttu-id="7813a-155">Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="7813a-155">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|
|<span data-ttu-id="7813a-156">settingUsage</span><span class="sxs-lookup"><span data-stu-id="7813a-156">settingUsage</span></span>|[<span data-ttu-id="7813a-157">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="7813a-157">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="7813a-158">Указывает, что категория содержит параметры, используемые для соответствия требованиям или конфигурации.</span><span class="sxs-lookup"><span data-stu-id="7813a-158">Indicates that the category contains settings that are used for Compliance or Configuration.</span></span> <span data-ttu-id="7813a-159">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="7813a-159">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="7813a-160">parentCategoryId</span><span class="sxs-lookup"><span data-stu-id="7813a-160">parentCategoryId</span></span>|<span data-ttu-id="7813a-161">Строка</span><span class="sxs-lookup"><span data-stu-id="7813a-161">String</span></span>|<span data-ttu-id="7813a-162">Родительский id категории.</span><span class="sxs-lookup"><span data-stu-id="7813a-162">Parent id of the category.</span></span>|
|<span data-ttu-id="7813a-163">rootCategoryId</span><span class="sxs-lookup"><span data-stu-id="7813a-163">rootCategoryId</span></span>|<span data-ttu-id="7813a-164">Строка</span><span class="sxs-lookup"><span data-stu-id="7813a-164">String</span></span>|<span data-ttu-id="7813a-165">Корневой id категории.</span><span class="sxs-lookup"><span data-stu-id="7813a-165">Root id of the category.</span></span>|
|<span data-ttu-id="7813a-166">childCategoryIds</span><span class="sxs-lookup"><span data-stu-id="7813a-166">childCategoryIds</span></span>|<span data-ttu-id="7813a-167">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7813a-167">String collection</span></span>|<span data-ttu-id="7813a-168">Список детских ids этой категории.</span><span class="sxs-lookup"><span data-stu-id="7813a-168">List of child ids of the category.</span></span>|



## <a name="response"></a><span data-ttu-id="7813a-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="7813a-169">Response</span></span>
<span data-ttu-id="7813a-170">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7813a-170">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7813a-171">Пример</span><span class="sxs-lookup"><span data-stu-id="7813a-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="7813a-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="7813a-172">Request</span></span>
<span data-ttu-id="7813a-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7813a-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationCategories
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

### <a name="response"></a><span data-ttu-id="7813a-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="7813a-174">Response</span></span>
<span data-ttu-id="7813a-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7813a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




