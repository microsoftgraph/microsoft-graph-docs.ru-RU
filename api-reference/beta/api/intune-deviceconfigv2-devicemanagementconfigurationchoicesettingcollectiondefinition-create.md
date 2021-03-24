---
title: Создание deviceManagementConfigurationChoiceSettingCollectionDefinition
description: Создание нового объекта deviceManagementConfigurationChoiceSettingCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1f9f09675c6c5274c82a4adcf246cfdd977dcc3b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136820"
---
# <a name="create-devicemanagementconfigurationchoicesettingcollectiondefinition"></a><span data-ttu-id="86b6f-103">Создание deviceManagementConfigurationChoiceSettingCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="86b6f-103">Create deviceManagementConfigurationChoiceSettingCollectionDefinition</span></span>

<span data-ttu-id="86b6f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86b6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86b6f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86b6f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86b6f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86b6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86b6f-107">Создание нового [объекта deviceManagementConfigurationChoiceSettingCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-107">Create a new [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86b6f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="86b6f-108">Prerequisites</span></span>
<span data-ttu-id="86b6f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86b6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86b6f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86b6f-111">Permission type</span></span>|<span data-ttu-id="86b6f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86b6f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86b6f-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86b6f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86b6f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86b6f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86b6f-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86b6f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86b6f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86b6f-116">Not supported.</span></span>|
|<span data-ttu-id="86b6f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="86b6f-117">Application</span></span>|<span data-ttu-id="86b6f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86b6f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86b6f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86b6f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="86b6f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="86b6f-120">Request headers</span></span>
|<span data-ttu-id="86b6f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86b6f-121">Header</span></span>|<span data-ttu-id="86b6f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="86b6f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86b6f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="86b6f-123">Authorization</span></span>|<span data-ttu-id="86b6f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86b6f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86b6f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="86b6f-125">Accept</span></span>|<span data-ttu-id="86b6f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86b6f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86b6f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86b6f-127">Request body</span></span>
<span data-ttu-id="86b6f-128">В теле запроса поставляем представление JSON для объекта deviceManagementConfigurationChoiceSettingCollectionDefinition.</span><span class="sxs-lookup"><span data-stu-id="86b6f-128">In the request body, supply a JSON representation for the deviceManagementConfigurationChoiceSettingCollectionDefinition object.</span></span>

<span data-ttu-id="86b6f-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementConfigurationChoiceSettingCollectionDefinition.</span><span class="sxs-lookup"><span data-stu-id="86b6f-129">The following table shows the properties that are required when you create the deviceManagementConfigurationChoiceSettingCollectionDefinition.</span></span>

|<span data-ttu-id="86b6f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="86b6f-130">Property</span></span>|<span data-ttu-id="86b6f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="86b6f-131">Type</span></span>|<span data-ttu-id="86b6f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="86b6f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86b6f-133">применимость</span><span class="sxs-lookup"><span data-stu-id="86b6f-133">applicability</span></span>|[<span data-ttu-id="86b6f-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="86b6f-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="86b6f-135">Сведения о том, какие параметры устройства применимы к унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="86b6f-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="86b6f-136">accessTypes</span></span>|[<span data-ttu-id="86b6f-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="86b6f-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="86b6f-138">Режим доступа к режиму чтения и записи параметров, унаследованных от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="86b6f-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="86b6f-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="86b6f-140">keywords</span><span class="sxs-lookup"><span data-stu-id="86b6f-140">keywords</span></span>|<span data-ttu-id="86b6f-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="86b6f-141">String collection</span></span>|<span data-ttu-id="86b6f-142">Маркеры для поиска параметров на унаследованных от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="86b6f-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="86b6f-143">infoUrls</span></span>|<span data-ttu-id="86b6f-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="86b6f-144">String collection</span></span>|<span data-ttu-id="86b6f-145">Список ссылок, дополнительные сведения о параметре можно найти на сайте Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="86b6f-146">возникновение</span><span class="sxs-lookup"><span data-stu-id="86b6f-146">occurrence</span></span>|[<span data-ttu-id="86b6f-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="86b6f-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="86b6f-148">Указывает, требуется ли параметр или не наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="86b6f-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="86b6f-149">baseUri</span></span>|<span data-ttu-id="86b6f-150">Строка</span><span class="sxs-lookup"><span data-stu-id="86b6f-150">String</span></span>|<span data-ttu-id="86b6f-151">Базовый путь CSP, унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="86b6f-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="86b6f-152">offsetUri</span></span>|<span data-ttu-id="86b6f-153">Строка</span><span class="sxs-lookup"><span data-stu-id="86b6f-153">String</span></span>|<span data-ttu-id="86b6f-154">Смещение пути CSP из базы, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="86b6f-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="86b6f-155">rootDefinitionId</span></span>|<span data-ttu-id="86b6f-156">Строка</span><span class="sxs-lookup"><span data-stu-id="86b6f-156">String</span></span>|<span data-ttu-id="86b6f-157">Определение корневого параметра, если это параметр ребенка.</span><span class="sxs-lookup"><span data-stu-id="86b6f-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="86b6f-158">Унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="86b6f-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="86b6f-159">categoryId</span></span>|<span data-ttu-id="86b6f-160">Строка</span><span class="sxs-lookup"><span data-stu-id="86b6f-160">String</span></span>|<span data-ttu-id="86b6f-161">Указывает группу области, в которой параметр настроен в указанном поставщике служб конфигурации (CSP), унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="86b6f-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="86b6f-162">settingUsage</span></span>|[<span data-ttu-id="86b6f-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="86b6f-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="86b6f-164">Тип настройки, например конфигурация и соответствие требованиям, унаследованные от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="86b6f-165">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="86b6f-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="86b6f-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="86b6f-166">uxBehavior</span></span>|[<span data-ttu-id="86b6f-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="86b6f-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="86b6f-168">Настройка представления типа управления в UX, унаследованной от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="86b6f-169">Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="86b6f-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="86b6f-170">visibility</span><span class="sxs-lookup"><span data-stu-id="86b6f-170">visibility</span></span>|[<span data-ttu-id="86b6f-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="86b6f-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="86b6f-172">Настройка области видимости для UX, унаследованной от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="86b6f-173">Возможные значения: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="86b6f-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="86b6f-174">id</span><span class="sxs-lookup"><span data-stu-id="86b6f-174">id</span></span>|<span data-ttu-id="86b6f-175">Строка</span><span class="sxs-lookup"><span data-stu-id="86b6f-175">String</span></span>|<span data-ttu-id="86b6f-176">Идентификатор элемента, унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-176">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="86b6f-177">description</span><span class="sxs-lookup"><span data-stu-id="86b6f-177">description</span></span>|<span data-ttu-id="86b6f-178">Строка</span><span class="sxs-lookup"><span data-stu-id="86b6f-178">String</span></span>|<span data-ttu-id="86b6f-179">Описание элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-179">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="86b6f-180">helpText</span><span class="sxs-lookup"><span data-stu-id="86b6f-180">helpText</span></span>|<span data-ttu-id="86b6f-181">Строка</span><span class="sxs-lookup"><span data-stu-id="86b6f-181">String</span></span>|<span data-ttu-id="86b6f-182">Справка текста элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-182">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="86b6f-183">name</span><span class="sxs-lookup"><span data-stu-id="86b6f-183">name</span></span>|<span data-ttu-id="86b6f-184">String</span><span class="sxs-lookup"><span data-stu-id="86b6f-184">String</span></span>|<span data-ttu-id="86b6f-185">Имя элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-185">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="86b6f-186">displayName</span><span class="sxs-lookup"><span data-stu-id="86b6f-186">displayName</span></span>|<span data-ttu-id="86b6f-187">Строка</span><span class="sxs-lookup"><span data-stu-id="86b6f-187">String</span></span>|<span data-ttu-id="86b6f-188">Отображение имени элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-188">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="86b6f-189">version</span><span class="sxs-lookup"><span data-stu-id="86b6f-189">version</span></span>|<span data-ttu-id="86b6f-190">String</span><span class="sxs-lookup"><span data-stu-id="86b6f-190">String</span></span>|<span data-ttu-id="86b6f-191">Версия элемента, унаследована от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-191">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="86b6f-192">options</span><span class="sxs-lookup"><span data-stu-id="86b6f-192">options</span></span>|<span data-ttu-id="86b6f-193">[коллекция deviceManagementConfigurationOptionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-193">[deviceManagementConfigurationOptionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinition.md) collection</span></span>|<span data-ttu-id="86b6f-194">Параметры для параметра, который можно выбрать наследуется из [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-194">Options for the setting that can be selected Inherited from [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span></span>|
|<span data-ttu-id="86b6f-195">defaultOptionId</span><span class="sxs-lookup"><span data-stu-id="86b6f-195">defaultOptionId</span></span>|<span data-ttu-id="86b6f-196">Строка</span><span class="sxs-lookup"><span data-stu-id="86b6f-196">String</span></span>|<span data-ttu-id="86b6f-197">Параметр по умолчанию для выбора параметра Inherited from [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="86b6f-197">Default option for choice setting Inherited from [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span></span>|
|<span data-ttu-id="86b6f-198">maximumCount</span><span class="sxs-lookup"><span data-stu-id="86b6f-198">maximumCount</span></span>|<span data-ttu-id="86b6f-199">Int32</span><span class="sxs-lookup"><span data-stu-id="86b6f-199">Int32</span></span>|<span data-ttu-id="86b6f-200">Максимальное количество вариантов в коллекции.</span><span class="sxs-lookup"><span data-stu-id="86b6f-200">Maximum number of choices in the collection.</span></span> <span data-ttu-id="86b6f-201">Допустимые значения от 1 до 100</span><span class="sxs-lookup"><span data-stu-id="86b6f-201">Valid values 1 to 100</span></span>|
|<span data-ttu-id="86b6f-202">minimumCount</span><span class="sxs-lookup"><span data-stu-id="86b6f-202">minimumCount</span></span>|<span data-ttu-id="86b6f-203">Int32</span><span class="sxs-lookup"><span data-stu-id="86b6f-203">Int32</span></span>|<span data-ttu-id="86b6f-204">Минимальное количество вариантов в коллекции.</span><span class="sxs-lookup"><span data-stu-id="86b6f-204">Minimum number of choices in the collection.</span></span> <span data-ttu-id="86b6f-205">Допустимые значения от 1 до 100</span><span class="sxs-lookup"><span data-stu-id="86b6f-205">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="86b6f-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="86b6f-206">Response</span></span>
<span data-ttu-id="86b6f-207">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="86b6f-207">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86b6f-208">Пример</span><span class="sxs-lookup"><span data-stu-id="86b6f-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="86b6f-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="86b6f-209">Request</span></span>
<span data-ttu-id="86b6f-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86b6f-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 9998

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingCollectionDefinition",
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
  "options": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinition",
      "optionValue": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValue",
        "children": [
          {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
            "settingDefinitionId": "Setting Definition Id value",
            "choiceSettingValue": {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
              "value": "Value value",
              "children": [
                {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                  "settingDefinitionId": "Setting Definition Id value",
                  "choiceSettingValue": {
                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                    "value": "Value value",
                    "children": [
                      {
                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                        "settingDefinitionId": "Setting Definition Id value",
                        "choiceSettingValue": {
                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                          "value": "Value value",
                          "children": [
                            {
                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                              "settingDefinitionId": "Setting Definition Id value",
                              "choiceSettingValue": {
                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                "value": "Value value",
                                "children": [
                                  {
                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                    "settingDefinitionId": "Setting Definition Id value",
                                    "choiceSettingValue": {
                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                      "value": "Value value",
                                      "children": [
                                        {
                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                          "settingDefinitionId": "Setting Definition Id value",
                                          "choiceSettingValue": {
                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                            "value": "Value value",
                                            "children": [
                                              {
                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                "settingDefinitionId": "Setting Definition Id value",
                                                "choiceSettingValue": {
                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                  "value": "Value value",
                                                  "children": [
                                                    {
                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                      "settingDefinitionId": "Setting Definition Id value",
                                                      "choiceSettingValue": {
                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                        "value": "Value value",
                                                        "children": [
                                                          {
                                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                            "settingDefinitionId": "Setting Definition Id value",
                                                            "choiceSettingValue": {
                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                              "value": "Value value",
                                                              "children": [
                                                                {
                                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                  "settingDefinitionId": "Setting Definition Id value",
                                                                  "choiceSettingValue": {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                    "value": "Value value",
                                                                    "children": [
                                                                      {
                                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                        "settingDefinitionId": "Setting Definition Id value",
                                                                        "choiceSettingValue": {
                                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                          "value": "Value value",
                                                                          "children": null
                                                                        }
                                                                      }
                                                                    ]
                                                                  }
                                                                }
                                                              ]
                                                            }
                                                          }
                                                        ]
                                                      }
                                                    }
                                                  ]
                                                }
                                              }
                                            ]
                                          }
                                        }
                                      ]
                                    }
                                  }
                                ]
                              }
                            }
                          ]
                        }
                      }
                    ]
                  }
                }
              ]
            }
          }
        ]
      },
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
      ],
      "itemId": "Item Id value",
      "description": "Description value",
      "helpText": "Help Text value",
      "name": "Name value",
      "displayName": "Display Name value"
    }
  ],
  "defaultOptionId": "Default Option Id value",
  "maximumCount": 12,
  "minimumCount": 12
}
```

### <a name="response"></a><span data-ttu-id="86b6f-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="86b6f-211">Response</span></span>
<span data-ttu-id="86b6f-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86b6f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 10047

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingCollectionDefinition",
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
  "id": "eb03fdca-fdca-eb03-cafd-03ebcafd03eb",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value",
  "options": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinition",
      "optionValue": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValue",
        "children": [
          {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
            "settingDefinitionId": "Setting Definition Id value",
            "choiceSettingValue": {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
              "value": "Value value",
              "children": [
                {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                  "settingDefinitionId": "Setting Definition Id value",
                  "choiceSettingValue": {
                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                    "value": "Value value",
                    "children": [
                      {
                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                        "settingDefinitionId": "Setting Definition Id value",
                        "choiceSettingValue": {
                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                          "value": "Value value",
                          "children": [
                            {
                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                              "settingDefinitionId": "Setting Definition Id value",
                              "choiceSettingValue": {
                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                "value": "Value value",
                                "children": [
                                  {
                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                    "settingDefinitionId": "Setting Definition Id value",
                                    "choiceSettingValue": {
                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                      "value": "Value value",
                                      "children": [
                                        {
                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                          "settingDefinitionId": "Setting Definition Id value",
                                          "choiceSettingValue": {
                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                            "value": "Value value",
                                            "children": [
                                              {
                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                "settingDefinitionId": "Setting Definition Id value",
                                                "choiceSettingValue": {
                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                  "value": "Value value",
                                                  "children": [
                                                    {
                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                      "settingDefinitionId": "Setting Definition Id value",
                                                      "choiceSettingValue": {
                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                        "value": "Value value",
                                                        "children": [
                                                          {
                                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                            "settingDefinitionId": "Setting Definition Id value",
                                                            "choiceSettingValue": {
                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                              "value": "Value value",
                                                              "children": [
                                                                {
                                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                  "settingDefinitionId": "Setting Definition Id value",
                                                                  "choiceSettingValue": {
                                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                    "value": "Value value",
                                                                    "children": [
                                                                      {
                                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                        "settingDefinitionId": "Setting Definition Id value",
                                                                        "choiceSettingValue": {
                                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                          "value": "Value value",
                                                                          "children": null
                                                                        }
                                                                      }
                                                                    ]
                                                                  }
                                                                }
                                                              ]
                                                            }
                                                          }
                                                        ]
                                                      }
                                                    }
                                                  ]
                                                }
                                              }
                                            ]
                                          }
                                        }
                                      ]
                                    }
                                  }
                                ]
                              }
                            }
                          ]
                        }
                      }
                    ]
                  }
                }
              ]
            }
          }
        ]
      },
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
      ],
      "itemId": "Item Id value",
      "description": "Description value",
      "helpText": "Help Text value",
      "name": "Name value",
      "displayName": "Display Name value"
    }
  ],
  "defaultOptionId": "Default Option Id value",
  "maximumCount": 12,
  "minimumCount": 12
}
```




