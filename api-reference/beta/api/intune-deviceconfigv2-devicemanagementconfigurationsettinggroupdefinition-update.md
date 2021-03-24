---
title: Обновление deviceManagementConfigurationSettingGroupDefinition
description: Обновление свойств объекта deviceManagementConfigurationSettingGroupDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8a3c18fe632d094ecfc7e6a7166ba23b8da7d0bc
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129211"
---
# <a name="update-devicemanagementconfigurationsettinggroupdefinition"></a><span data-ttu-id="cefc0-103">Обновление deviceManagementConfigurationSettingGroupDefinition</span><span class="sxs-lookup"><span data-stu-id="cefc0-103">Update deviceManagementConfigurationSettingGroupDefinition</span></span>

<span data-ttu-id="cefc0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cefc0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cefc0-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cefc0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cefc0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cefc0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cefc0-107">Обновление свойств объекта [deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-107">Update the properties of a [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cefc0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cefc0-108">Prerequisites</span></span>
<span data-ttu-id="cefc0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cefc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cefc0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cefc0-111">Permission type</span></span>|<span data-ttu-id="cefc0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cefc0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cefc0-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cefc0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cefc0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cefc0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cefc0-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cefc0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cefc0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cefc0-116">Not supported.</span></span>|
|<span data-ttu-id="cefc0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cefc0-117">Application</span></span>|<span data-ttu-id="cefc0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cefc0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cefc0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cefc0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="cefc0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cefc0-120">Request headers</span></span>
|<span data-ttu-id="cefc0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cefc0-121">Header</span></span>|<span data-ttu-id="cefc0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cefc0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cefc0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cefc0-123">Authorization</span></span>|<span data-ttu-id="cefc0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cefc0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cefc0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cefc0-125">Accept</span></span>|<span data-ttu-id="cefc0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cefc0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cefc0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cefc0-127">Request body</span></span>
<span data-ttu-id="cefc0-128">В теле запроса поставляем представление JSON для [объекта deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

<span data-ttu-id="cefc0-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md).</span></span>

|<span data-ttu-id="cefc0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cefc0-130">Property</span></span>|<span data-ttu-id="cefc0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cefc0-131">Type</span></span>|<span data-ttu-id="cefc0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cefc0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cefc0-133">применимость</span><span class="sxs-lookup"><span data-stu-id="cefc0-133">applicability</span></span>|[<span data-ttu-id="cefc0-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="cefc0-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="cefc0-135">Сведения о том, какие параметры устройства применимы к унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="cefc0-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="cefc0-136">accessTypes</span></span>|[<span data-ttu-id="cefc0-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="cefc0-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="cefc0-138">Режим доступа к режиму чтения и записи параметров, унаследованных от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="cefc0-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="cefc0-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="cefc0-140">keywords</span><span class="sxs-lookup"><span data-stu-id="cefc0-140">keywords</span></span>|<span data-ttu-id="cefc0-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cefc0-141">String collection</span></span>|<span data-ttu-id="cefc0-142">Маркеры для поиска параметров на унаследованных от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="cefc0-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="cefc0-143">infoUrls</span></span>|<span data-ttu-id="cefc0-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cefc0-144">String collection</span></span>|<span data-ttu-id="cefc0-145">Список ссылок, дополнительные сведения о параметре можно найти на сайте Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="cefc0-146">возникновение</span><span class="sxs-lookup"><span data-stu-id="cefc0-146">occurrence</span></span>|[<span data-ttu-id="cefc0-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="cefc0-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="cefc0-148">Указывает, требуется ли параметр или не наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="cefc0-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="cefc0-149">baseUri</span></span>|<span data-ttu-id="cefc0-150">Строка</span><span class="sxs-lookup"><span data-stu-id="cefc0-150">String</span></span>|<span data-ttu-id="cefc0-151">Базовый путь CSP, унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="cefc0-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="cefc0-152">offsetUri</span></span>|<span data-ttu-id="cefc0-153">Строка</span><span class="sxs-lookup"><span data-stu-id="cefc0-153">String</span></span>|<span data-ttu-id="cefc0-154">Смещение пути CSP из базы, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="cefc0-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="cefc0-155">rootDefinitionId</span></span>|<span data-ttu-id="cefc0-156">Строка</span><span class="sxs-lookup"><span data-stu-id="cefc0-156">String</span></span>|<span data-ttu-id="cefc0-157">Определение корневого параметра, если это параметр ребенка.</span><span class="sxs-lookup"><span data-stu-id="cefc0-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="cefc0-158">Унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="cefc0-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="cefc0-159">categoryId</span></span>|<span data-ttu-id="cefc0-160">Строка</span><span class="sxs-lookup"><span data-stu-id="cefc0-160">String</span></span>|<span data-ttu-id="cefc0-161">Указывает группу области, в которой параметр настроен в указанном поставщике служб конфигурации (CSP), унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="cefc0-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="cefc0-162">settingUsage</span></span>|[<span data-ttu-id="cefc0-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="cefc0-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="cefc0-164">Тип настройки, например конфигурация и соответствие требованиям, унаследованные от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="cefc0-165">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="cefc0-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="cefc0-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="cefc0-166">uxBehavior</span></span>|[<span data-ttu-id="cefc0-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="cefc0-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="cefc0-168">Настройка представления типа управления в UX, унаследованной от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="cefc0-169">Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="cefc0-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="cefc0-170">visibility</span><span class="sxs-lookup"><span data-stu-id="cefc0-170">visibility</span></span>|[<span data-ttu-id="cefc0-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="cefc0-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="cefc0-172">Настройка области видимости для UX, унаследованной от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="cefc0-173">Возможные значения: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="cefc0-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="cefc0-174">id</span><span class="sxs-lookup"><span data-stu-id="cefc0-174">id</span></span>|<span data-ttu-id="cefc0-175">Строка</span><span class="sxs-lookup"><span data-stu-id="cefc0-175">String</span></span>|<span data-ttu-id="cefc0-176">Идентификатор элемента, унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-176">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="cefc0-177">description</span><span class="sxs-lookup"><span data-stu-id="cefc0-177">description</span></span>|<span data-ttu-id="cefc0-178">Строка</span><span class="sxs-lookup"><span data-stu-id="cefc0-178">String</span></span>|<span data-ttu-id="cefc0-179">Описание элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-179">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="cefc0-180">helpText</span><span class="sxs-lookup"><span data-stu-id="cefc0-180">helpText</span></span>|<span data-ttu-id="cefc0-181">Строка</span><span class="sxs-lookup"><span data-stu-id="cefc0-181">String</span></span>|<span data-ttu-id="cefc0-182">Справка текста элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-182">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="cefc0-183">name</span><span class="sxs-lookup"><span data-stu-id="cefc0-183">name</span></span>|<span data-ttu-id="cefc0-184">String</span><span class="sxs-lookup"><span data-stu-id="cefc0-184">String</span></span>|<span data-ttu-id="cefc0-185">Имя элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-185">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="cefc0-186">displayName</span><span class="sxs-lookup"><span data-stu-id="cefc0-186">displayName</span></span>|<span data-ttu-id="cefc0-187">Строка</span><span class="sxs-lookup"><span data-stu-id="cefc0-187">String</span></span>|<span data-ttu-id="cefc0-188">Отображение имени элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-188">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="cefc0-189">version</span><span class="sxs-lookup"><span data-stu-id="cefc0-189">version</span></span>|<span data-ttu-id="cefc0-190">String</span><span class="sxs-lookup"><span data-stu-id="cefc0-190">String</span></span>|<span data-ttu-id="cefc0-191">Версия элемента, унаследована от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-191">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="cefc0-192">childIds</span><span class="sxs-lookup"><span data-stu-id="cefc0-192">childIds</span></span>|<span data-ttu-id="cefc0-193">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cefc0-193">String collection</span></span>|<span data-ttu-id="cefc0-194">Зависимые параметры ребенка для этой группы параметров</span><span class="sxs-lookup"><span data-stu-id="cefc0-194">Dependent child settings to this group of settings</span></span>|
|<span data-ttu-id="cefc0-195">dependentOn</span><span class="sxs-lookup"><span data-stu-id="cefc0-195">dependentOn</span></span>|<span data-ttu-id="cefc0-196">[коллекция deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-196">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="cefc0-197">Список зависимостей для группы параметров</span><span class="sxs-lookup"><span data-stu-id="cefc0-197">List of Dependencies for the setting group</span></span>|
|<span data-ttu-id="cefc0-198">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="cefc0-198">dependedOnBy</span></span>|<span data-ttu-id="cefc0-199">[коллекция deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="cefc0-199">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="cefc0-200">Список параметров ребенка, которые зависят от этого параметра</span><span class="sxs-lookup"><span data-stu-id="cefc0-200">List of child settings that depend on this setting</span></span>|



## <a name="response"></a><span data-ttu-id="cefc0-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="cefc0-201">Response</span></span>
<span data-ttu-id="cefc0-202">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cefc0-202">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cefc0-203">Пример</span><span class="sxs-lookup"><span data-stu-id="cefc0-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="cefc0-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="cefc0-204">Request</span></span>
<span data-ttu-id="cefc0-205">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cefc0-205">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
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

### <a name="response"></a><span data-ttu-id="cefc0-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="cefc0-206">Response</span></span>
<span data-ttu-id="cefc0-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cefc0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




