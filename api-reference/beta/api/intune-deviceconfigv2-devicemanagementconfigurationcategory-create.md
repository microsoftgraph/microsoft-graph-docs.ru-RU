---
title: Создание deviceManagementConfigurationCategory
description: Создание нового объекта deviceManagementConfigurationCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 454c6070f01fef3a23a1ddf8ab49e3f7a1db9e07
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866288"
---
# <a name="create-devicemanagementconfigurationcategory"></a><span data-ttu-id="77200-103">Создание deviceManagementConfigurationCategory</span><span class="sxs-lookup"><span data-stu-id="77200-103">Create deviceManagementConfigurationCategory</span></span>

<span data-ttu-id="77200-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77200-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77200-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77200-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77200-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77200-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77200-107">Создание нового [объекта deviceManagementConfigurationCategory.](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="77200-107">Create a new [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77200-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="77200-108">Prerequisites</span></span>
<span data-ttu-id="77200-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77200-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77200-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77200-111">Permission type</span></span>|<span data-ttu-id="77200-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77200-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77200-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77200-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77200-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77200-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77200-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77200-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77200-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77200-116">Not supported.</span></span>|
|<span data-ttu-id="77200-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="77200-117">Application</span></span>|<span data-ttu-id="77200-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77200-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77200-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77200-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationCategories
```

## <a name="request-headers"></a><span data-ttu-id="77200-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="77200-120">Request headers</span></span>
|<span data-ttu-id="77200-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77200-121">Header</span></span>|<span data-ttu-id="77200-122">Значение</span><span class="sxs-lookup"><span data-stu-id="77200-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77200-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77200-123">Authorization</span></span>|<span data-ttu-id="77200-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77200-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77200-125">Accept</span><span class="sxs-lookup"><span data-stu-id="77200-125">Accept</span></span>|<span data-ttu-id="77200-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77200-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77200-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77200-127">Request body</span></span>
<span data-ttu-id="77200-128">В теле запроса поставляем представление JSON для объекта deviceManagementConfigurationCategory.</span><span class="sxs-lookup"><span data-stu-id="77200-128">In the request body, supply a JSON representation for the deviceManagementConfigurationCategory object.</span></span>

<span data-ttu-id="77200-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementConfigurationCategory.</span><span class="sxs-lookup"><span data-stu-id="77200-129">The following table shows the properties that are required when you create the deviceManagementConfigurationCategory.</span></span>

|<span data-ttu-id="77200-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="77200-130">Property</span></span>|<span data-ttu-id="77200-131">Тип</span><span class="sxs-lookup"><span data-stu-id="77200-131">Type</span></span>|<span data-ttu-id="77200-132">Описание</span><span class="sxs-lookup"><span data-stu-id="77200-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77200-133">id</span><span class="sxs-lookup"><span data-stu-id="77200-133">id</span></span>|<span data-ttu-id="77200-134">String</span><span class="sxs-lookup"><span data-stu-id="77200-134">String</span></span>|<span data-ttu-id="77200-135">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="77200-135">Identifier for item</span></span>|
|<span data-ttu-id="77200-136">description</span><span class="sxs-lookup"><span data-stu-id="77200-136">description</span></span>|<span data-ttu-id="77200-137">String</span><span class="sxs-lookup"><span data-stu-id="77200-137">String</span></span>|<span data-ttu-id="77200-138">Описание элемента</span><span class="sxs-lookup"><span data-stu-id="77200-138">Description of the item</span></span>|
|<span data-ttu-id="77200-139">helpText</span><span class="sxs-lookup"><span data-stu-id="77200-139">helpText</span></span>|<span data-ttu-id="77200-140">String</span><span class="sxs-lookup"><span data-stu-id="77200-140">String</span></span>|<span data-ttu-id="77200-141">Справка текста элемента</span><span class="sxs-lookup"><span data-stu-id="77200-141">Help text of the item</span></span>|
|<span data-ttu-id="77200-142">name</span><span class="sxs-lookup"><span data-stu-id="77200-142">name</span></span>|<span data-ttu-id="77200-143">String</span><span class="sxs-lookup"><span data-stu-id="77200-143">String</span></span>|<span data-ttu-id="77200-144">Имя элемента</span><span class="sxs-lookup"><span data-stu-id="77200-144">Name of the item</span></span>|
|<span data-ttu-id="77200-145">displayName</span><span class="sxs-lookup"><span data-stu-id="77200-145">displayName</span></span>|<span data-ttu-id="77200-146">String</span><span class="sxs-lookup"><span data-stu-id="77200-146">String</span></span>|<span data-ttu-id="77200-147">Отображение имени элемента</span><span class="sxs-lookup"><span data-stu-id="77200-147">Display name of the item</span></span>|
|<span data-ttu-id="77200-148">платформы</span><span class="sxs-lookup"><span data-stu-id="77200-148">platforms</span></span>|[<span data-ttu-id="77200-149">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="77200-149">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="77200-150">Типы платформ, которые имеются в этой категории.</span><span class="sxs-lookup"><span data-stu-id="77200-150">Platforms types, which settings in the category have.</span></span> <span data-ttu-id="77200-151">Возможные значения: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="77200-151">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="77200-152">технологии</span><span class="sxs-lookup"><span data-stu-id="77200-152">technologies</span></span>|[<span data-ttu-id="77200-153">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="77200-153">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="77200-154">Типы технологий, которые имеют параметры в категории.</span><span class="sxs-lookup"><span data-stu-id="77200-154">Technologies types, which settings in the category have.</span></span> <span data-ttu-id="77200-155">Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="77200-155">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|
|<span data-ttu-id="77200-156">settingUsage</span><span class="sxs-lookup"><span data-stu-id="77200-156">settingUsage</span></span>|[<span data-ttu-id="77200-157">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="77200-157">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="77200-158">Указывает, что категория содержит параметры, используемые для соответствия требованиям или конфигурации.</span><span class="sxs-lookup"><span data-stu-id="77200-158">Indicates that the category contains settings that are used for Compliance or Configuration.</span></span> <span data-ttu-id="77200-159">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="77200-159">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="77200-160">parentCategoryId</span><span class="sxs-lookup"><span data-stu-id="77200-160">parentCategoryId</span></span>|<span data-ttu-id="77200-161">String</span><span class="sxs-lookup"><span data-stu-id="77200-161">String</span></span>|<span data-ttu-id="77200-162">Родительский id категории.</span><span class="sxs-lookup"><span data-stu-id="77200-162">Parent id of the category.</span></span>|
|<span data-ttu-id="77200-163">rootCategoryId</span><span class="sxs-lookup"><span data-stu-id="77200-163">rootCategoryId</span></span>|<span data-ttu-id="77200-164">String</span><span class="sxs-lookup"><span data-stu-id="77200-164">String</span></span>|<span data-ttu-id="77200-165">Корневой id категории.</span><span class="sxs-lookup"><span data-stu-id="77200-165">Root id of the category.</span></span>|
|<span data-ttu-id="77200-166">childCategoryIds</span><span class="sxs-lookup"><span data-stu-id="77200-166">childCategoryIds</span></span>|<span data-ttu-id="77200-167">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="77200-167">String collection</span></span>|<span data-ttu-id="77200-168">Список детских ids этой категории.</span><span class="sxs-lookup"><span data-stu-id="77200-168">List of child ids of the category.</span></span>|



## <a name="response"></a><span data-ttu-id="77200-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="77200-169">Response</span></span>
<span data-ttu-id="77200-170">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="77200-170">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77200-171">Пример</span><span class="sxs-lookup"><span data-stu-id="77200-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="77200-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="77200-172">Request</span></span>
<span data-ttu-id="77200-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77200-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="77200-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="77200-174">Response</span></span>
<span data-ttu-id="77200-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77200-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




