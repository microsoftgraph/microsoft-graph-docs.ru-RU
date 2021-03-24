---
title: Создание deviceManagementConfigurationSettingGroupDefinition
description: Создание нового объекта deviceManagementConfigurationSettingGroupDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a3a0ea4d784fb91ee237b5bb2de7864dfb1dc5cd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129247"
---
# <a name="create-devicemanagementconfigurationsettinggroupdefinition"></a><span data-ttu-id="47650-103">Создание deviceManagementConfigurationSettingGroupDefinition</span><span class="sxs-lookup"><span data-stu-id="47650-103">Create deviceManagementConfigurationSettingGroupDefinition</span></span>

<span data-ttu-id="47650-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47650-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47650-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47650-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47650-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47650-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47650-107">Создание нового [объекта deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="47650-107">Create a new [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47650-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="47650-108">Prerequisites</span></span>
<span data-ttu-id="47650-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47650-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47650-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47650-111">Permission type</span></span>|<span data-ttu-id="47650-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47650-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47650-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47650-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47650-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47650-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47650-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47650-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47650-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47650-116">Not supported.</span></span>|
|<span data-ttu-id="47650-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="47650-117">Application</span></span>|<span data-ttu-id="47650-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47650-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47650-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47650-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="47650-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="47650-120">Request headers</span></span>
|<span data-ttu-id="47650-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47650-121">Header</span></span>|<span data-ttu-id="47650-122">Значение</span><span class="sxs-lookup"><span data-stu-id="47650-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47650-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="47650-123">Authorization</span></span>|<span data-ttu-id="47650-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47650-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47650-125">Accept</span><span class="sxs-lookup"><span data-stu-id="47650-125">Accept</span></span>|<span data-ttu-id="47650-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47650-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47650-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47650-127">Request body</span></span>
<span data-ttu-id="47650-128">В теле запроса поставляем представление JSON для объекта deviceManagementConfigurationSettingGroupDefinition.</span><span class="sxs-lookup"><span data-stu-id="47650-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingGroupDefinition object.</span></span>

<span data-ttu-id="47650-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementConfigurationSettingGroupDefinition.</span><span class="sxs-lookup"><span data-stu-id="47650-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingGroupDefinition.</span></span>

|<span data-ttu-id="47650-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="47650-130">Property</span></span>|<span data-ttu-id="47650-131">Тип</span><span class="sxs-lookup"><span data-stu-id="47650-131">Type</span></span>|<span data-ttu-id="47650-132">Описание</span><span class="sxs-lookup"><span data-stu-id="47650-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47650-133">применимость</span><span class="sxs-lookup"><span data-stu-id="47650-133">applicability</span></span>|[<span data-ttu-id="47650-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="47650-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="47650-135">Сведения о том, какие параметры устройства применимы к унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="47650-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="47650-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="47650-136">accessTypes</span></span>|[<span data-ttu-id="47650-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="47650-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="47650-138">Режим доступа к режиму чтения и записи параметров, унаследованных от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="47650-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="47650-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="47650-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="47650-140">keywords</span><span class="sxs-lookup"><span data-stu-id="47650-140">keywords</span></span>|<span data-ttu-id="47650-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="47650-141">String collection</span></span>|<span data-ttu-id="47650-142">Маркеры для поиска параметров на унаследованных от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="47650-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="47650-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="47650-143">infoUrls</span></span>|<span data-ttu-id="47650-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="47650-144">String collection</span></span>|<span data-ttu-id="47650-145">Список ссылок, дополнительные сведения о параметре можно найти на сайте Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="47650-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="47650-146">возникновение</span><span class="sxs-lookup"><span data-stu-id="47650-146">occurrence</span></span>|[<span data-ttu-id="47650-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="47650-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="47650-148">Указывает, требуется ли параметр или не наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="47650-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="47650-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="47650-149">baseUri</span></span>|<span data-ttu-id="47650-150">Строка</span><span class="sxs-lookup"><span data-stu-id="47650-150">String</span></span>|<span data-ttu-id="47650-151">Базовый путь CSP, унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="47650-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="47650-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="47650-152">offsetUri</span></span>|<span data-ttu-id="47650-153">Строка</span><span class="sxs-lookup"><span data-stu-id="47650-153">String</span></span>|<span data-ttu-id="47650-154">Смещение пути CSP из базы, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="47650-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="47650-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="47650-155">rootDefinitionId</span></span>|<span data-ttu-id="47650-156">Строка</span><span class="sxs-lookup"><span data-stu-id="47650-156">String</span></span>|<span data-ttu-id="47650-157">Определение корневого параметра, если это параметр ребенка.</span><span class="sxs-lookup"><span data-stu-id="47650-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="47650-158">Унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="47650-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="47650-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="47650-159">categoryId</span></span>|<span data-ttu-id="47650-160">Строка</span><span class="sxs-lookup"><span data-stu-id="47650-160">String</span></span>|<span data-ttu-id="47650-161">Указывает группу области, в которой параметр настроен в указанном поставщике служб конфигурации (CSP), унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="47650-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="47650-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="47650-162">settingUsage</span></span>|[<span data-ttu-id="47650-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="47650-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="47650-164">Тип настройки, например конфигурация и соответствие требованиям, унаследованные от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="47650-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="47650-165">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="47650-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="47650-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="47650-166">uxBehavior</span></span>|[<span data-ttu-id="47650-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="47650-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="47650-168">Настройка представления типа управления в UX, унаследованной от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="47650-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="47650-169">Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="47650-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="47650-170">visibility</span><span class="sxs-lookup"><span data-stu-id="47650-170">visibility</span></span>|[<span data-ttu-id="47650-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="47650-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="47650-172">Настройка области видимости для UX, унаследованной от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="47650-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="47650-173">Возможные значения: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="47650-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="47650-174">id</span><span class="sxs-lookup"><span data-stu-id="47650-174">id</span></span>|<span data-ttu-id="47650-175">Строка</span><span class="sxs-lookup"><span data-stu-id="47650-175">String</span></span>|<span data-ttu-id="47650-176">Идентификатор элемента, унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="47650-176">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="47650-177">description</span><span class="sxs-lookup"><span data-stu-id="47650-177">description</span></span>|<span data-ttu-id="47650-178">Строка</span><span class="sxs-lookup"><span data-stu-id="47650-178">String</span></span>|<span data-ttu-id="47650-179">Описание элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="47650-179">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="47650-180">helpText</span><span class="sxs-lookup"><span data-stu-id="47650-180">helpText</span></span>|<span data-ttu-id="47650-181">Строка</span><span class="sxs-lookup"><span data-stu-id="47650-181">String</span></span>|<span data-ttu-id="47650-182">Справка текста элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="47650-182">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="47650-183">name</span><span class="sxs-lookup"><span data-stu-id="47650-183">name</span></span>|<span data-ttu-id="47650-184">String</span><span class="sxs-lookup"><span data-stu-id="47650-184">String</span></span>|<span data-ttu-id="47650-185">Имя элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="47650-185">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="47650-186">displayName</span><span class="sxs-lookup"><span data-stu-id="47650-186">displayName</span></span>|<span data-ttu-id="47650-187">Строка</span><span class="sxs-lookup"><span data-stu-id="47650-187">String</span></span>|<span data-ttu-id="47650-188">Отображение имени элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="47650-188">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="47650-189">version</span><span class="sxs-lookup"><span data-stu-id="47650-189">version</span></span>|<span data-ttu-id="47650-190">String</span><span class="sxs-lookup"><span data-stu-id="47650-190">String</span></span>|<span data-ttu-id="47650-191">Версия элемента, унаследована от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="47650-191">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="47650-192">childIds</span><span class="sxs-lookup"><span data-stu-id="47650-192">childIds</span></span>|<span data-ttu-id="47650-193">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="47650-193">String collection</span></span>|<span data-ttu-id="47650-194">Зависимые параметры ребенка для этой группы параметров</span><span class="sxs-lookup"><span data-stu-id="47650-194">Dependent child settings to this group of settings</span></span>|
|<span data-ttu-id="47650-195">dependentOn</span><span class="sxs-lookup"><span data-stu-id="47650-195">dependentOn</span></span>|<span data-ttu-id="47650-196">[коллекция deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="47650-196">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="47650-197">Список зависимостей для группы параметров</span><span class="sxs-lookup"><span data-stu-id="47650-197">List of Dependencies for the setting group</span></span>|
|<span data-ttu-id="47650-198">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="47650-198">dependedOnBy</span></span>|<span data-ttu-id="47650-199">[коллекция deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="47650-199">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="47650-200">Список параметров ребенка, которые зависят от этого параметра</span><span class="sxs-lookup"><span data-stu-id="47650-200">List of child settings that depend on this setting</span></span>|



## <a name="response"></a><span data-ttu-id="47650-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="47650-201">Response</span></span>
<span data-ttu-id="47650-202">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="47650-202">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47650-203">Пример</span><span class="sxs-lookup"><span data-stu-id="47650-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="47650-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="47650-204">Request</span></span>
<span data-ttu-id="47650-205">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47650-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 1513

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupDefinition",
  "applicability": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
    "description": "Description value",
    "platform": "macOS",
    "deviceMode": "kiosk",
    "technologies": "mdm"
  },
  "accessTypes": "add",
  "keywords": [
    "Keywords value"
  ],
  "infoUrls": [
    "Info Urls value"
  ],
  "occurrence": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence",
    "minDeviceOccurrence": 3,
    "maxDeviceOccurrence": 3
  },
  "baseUri": "Base Uri value",
  "offsetUri": "Offset Uri value",
  "rootDefinitionId": "Root Definition Id value",
  "categoryId": "Category Id value",
  "settingUsage": "configuration",
  "uxBehavior": "dropdown",
  "visibility": "settingsCatalog",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value",
  "childIds": [
    "Child Ids value"
  ],
  "dependentOn": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn",
      "dependentOn": "Dependent On value",
      "parentSettingId": "Parent Setting Id value"
    }
  ],
  "dependedOnBy": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
      "dependedOnBy": "Depended On By value",
      "required": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="47650-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="47650-206">Response</span></span>
<span data-ttu-id="47650-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47650-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1562

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupDefinition",
  "applicability": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
    "description": "Description value",
    "platform": "macOS",
    "deviceMode": "kiosk",
    "technologies": "mdm"
  },
  "accessTypes": "add",
  "keywords": [
    "Keywords value"
  ],
  "infoUrls": [
    "Info Urls value"
  ],
  "occurrence": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence",
    "minDeviceOccurrence": 3,
    "maxDeviceOccurrence": 3
  },
  "baseUri": "Base Uri value",
  "offsetUri": "Offset Uri value",
  "rootDefinitionId": "Root Definition Id value",
  "categoryId": "Category Id value",
  "settingUsage": "configuration",
  "uxBehavior": "dropdown",
  "visibility": "settingsCatalog",
  "id": "95dc9604-9604-95dc-0496-dc950496dc95",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value",
  "childIds": [
    "Child Ids value"
  ],
  "dependentOn": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn",
      "dependentOn": "Dependent On value",
      "parentSettingId": "Parent Setting Id value"
    }
  ],
  "dependedOnBy": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
      "dependedOnBy": "Depended On By value",
      "required": true
    }
  ]
}
```




