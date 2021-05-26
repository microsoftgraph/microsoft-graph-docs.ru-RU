---
title: Обновление deviceManagementConfigurationSettingGroupDefinition
description: Обновление свойств объекта deviceManagementConfigurationSettingGroupDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 68338b0fe37a9f93911218298f07042e7a879c83
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665443"
---
# <a name="update-devicemanagementconfigurationsettinggroupdefinition"></a><span data-ttu-id="7c986-103">Обновление deviceManagementConfigurationSettingGroupDefinition</span><span class="sxs-lookup"><span data-stu-id="7c986-103">Update deviceManagementConfigurationSettingGroupDefinition</span></span>

<span data-ttu-id="7c986-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c986-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c986-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c986-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c986-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c986-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c986-107">Обновление свойств объекта [deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-107">Update the properties of a [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c986-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7c986-108">Prerequisites</span></span>
<span data-ttu-id="7c986-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c986-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c986-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c986-111">Permission type</span></span>|<span data-ttu-id="7c986-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c986-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c986-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c986-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c986-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c986-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7c986-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c986-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c986-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c986-116">Not supported.</span></span>|
|<span data-ttu-id="7c986-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7c986-117">Application</span></span>|<span data-ttu-id="7c986-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c986-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c986-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c986-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reusableSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates/{deviceManagementConfigurationSettingTemplateId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="7c986-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7c986-120">Request headers</span></span>
|<span data-ttu-id="7c986-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c986-121">Header</span></span>|<span data-ttu-id="7c986-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7c986-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c986-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c986-123">Authorization</span></span>|<span data-ttu-id="7c986-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c986-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c986-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7c986-125">Accept</span></span>|<span data-ttu-id="7c986-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c986-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c986-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c986-127">Request body</span></span>
<span data-ttu-id="7c986-128">В теле запроса поставляем представление JSON для [объекта deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

<span data-ttu-id="7c986-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md).</span></span>

|<span data-ttu-id="7c986-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c986-130">Property</span></span>|<span data-ttu-id="7c986-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7c986-131">Type</span></span>|<span data-ttu-id="7c986-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7c986-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c986-133">применимость</span><span class="sxs-lookup"><span data-stu-id="7c986-133">applicability</span></span>|[<span data-ttu-id="7c986-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="7c986-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="7c986-135">Сведения о том, какие параметры устройства применимы к унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7c986-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="7c986-136">accessTypes</span></span>|[<span data-ttu-id="7c986-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="7c986-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="7c986-138">Режим доступа к режиму чтения и записи параметров, унаследованных от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="7c986-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="7c986-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="7c986-140">keywords</span><span class="sxs-lookup"><span data-stu-id="7c986-140">keywords</span></span>|<span data-ttu-id="7c986-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7c986-141">String collection</span></span>|<span data-ttu-id="7c986-142">Маркеры для поиска параметров на унаследованных от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7c986-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="7c986-143">infoUrls</span></span>|<span data-ttu-id="7c986-144">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7c986-144">String collection</span></span>|<span data-ttu-id="7c986-145">Список ссылок, дополнительные сведения о параметре можно найти на сайте Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7c986-146">возникновение</span><span class="sxs-lookup"><span data-stu-id="7c986-146">occurrence</span></span>|[<span data-ttu-id="7c986-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="7c986-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="7c986-148">Указывает, требуется ли параметр или не наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7c986-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="7c986-149">baseUri</span></span>|<span data-ttu-id="7c986-150">Строка</span><span class="sxs-lookup"><span data-stu-id="7c986-150">String</span></span>|<span data-ttu-id="7c986-151">Базовый путь CSP, унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7c986-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="7c986-152">offsetUri</span></span>|<span data-ttu-id="7c986-153">Строка</span><span class="sxs-lookup"><span data-stu-id="7c986-153">String</span></span>|<span data-ttu-id="7c986-154">Смещение пути CSP из базы, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7c986-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7c986-155">rootDefinitionId</span></span>|<span data-ttu-id="7c986-156">Строка</span><span class="sxs-lookup"><span data-stu-id="7c986-156">String</span></span>|<span data-ttu-id="7c986-157">Определение корневого параметра, если это параметр ребенка.</span><span class="sxs-lookup"><span data-stu-id="7c986-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="7c986-158">Унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7c986-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="7c986-159">categoryId</span></span>|<span data-ttu-id="7c986-160">Строка</span><span class="sxs-lookup"><span data-stu-id="7c986-160">String</span></span>|<span data-ttu-id="7c986-161">Указывает группу области, в которой параметр настроен в указанном поставщике служб конфигурации (CSP), унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7c986-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="7c986-162">settingUsage</span></span>|[<span data-ttu-id="7c986-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="7c986-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="7c986-164">Тип настройки, например конфигурация и соответствие требованиям, унаследованные от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="7c986-165">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="7c986-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="7c986-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="7c986-166">uxBehavior</span></span>|[<span data-ttu-id="7c986-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="7c986-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="7c986-168">Настройка представления типа управления в UX, унаследованной от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="7c986-169">Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="7c986-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="7c986-170">visibility</span><span class="sxs-lookup"><span data-stu-id="7c986-170">visibility</span></span>|[<span data-ttu-id="7c986-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="7c986-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="7c986-172">Настройка области видимости для UX, унаследованной от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="7c986-173">Возможные значения: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="7c986-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="7c986-174">referredSettingInformationList</span><span class="sxs-lookup"><span data-stu-id="7c986-174">referredSettingInformationList</span></span>|<span data-ttu-id="7c986-175">[коллекция deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-175">[deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md) collection</span></span>|<span data-ttu-id="7c986-176">Список переданных сведений о параметрах.</span><span class="sxs-lookup"><span data-stu-id="7c986-176">List of referred setting information.</span></span> <span data-ttu-id="7c986-177">Унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-177">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7c986-178">id</span><span class="sxs-lookup"><span data-stu-id="7c986-178">id</span></span>|<span data-ttu-id="7c986-179">Строка</span><span class="sxs-lookup"><span data-stu-id="7c986-179">String</span></span>|<span data-ttu-id="7c986-180">Идентификатор элемента, унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-180">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7c986-181">description</span><span class="sxs-lookup"><span data-stu-id="7c986-181">description</span></span>|<span data-ttu-id="7c986-182">Строка</span><span class="sxs-lookup"><span data-stu-id="7c986-182">String</span></span>|<span data-ttu-id="7c986-183">Описание элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-183">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7c986-184">helpText</span><span class="sxs-lookup"><span data-stu-id="7c986-184">helpText</span></span>|<span data-ttu-id="7c986-185">Строка</span><span class="sxs-lookup"><span data-stu-id="7c986-185">String</span></span>|<span data-ttu-id="7c986-186">Справка текста элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-186">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7c986-187">name</span><span class="sxs-lookup"><span data-stu-id="7c986-187">name</span></span>|<span data-ttu-id="7c986-188">String</span><span class="sxs-lookup"><span data-stu-id="7c986-188">String</span></span>|<span data-ttu-id="7c986-189">Имя элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-189">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7c986-190">displayName</span><span class="sxs-lookup"><span data-stu-id="7c986-190">displayName</span></span>|<span data-ttu-id="7c986-191">Строка</span><span class="sxs-lookup"><span data-stu-id="7c986-191">String</span></span>|<span data-ttu-id="7c986-192">Отображение имени элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-192">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7c986-193">version</span><span class="sxs-lookup"><span data-stu-id="7c986-193">version</span></span>|<span data-ttu-id="7c986-194">String</span><span class="sxs-lookup"><span data-stu-id="7c986-194">String</span></span>|<span data-ttu-id="7c986-195">Версия элемента, унаследована от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-195">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="7c986-196">childIds</span><span class="sxs-lookup"><span data-stu-id="7c986-196">childIds</span></span>|<span data-ttu-id="7c986-197">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7c986-197">String collection</span></span>|<span data-ttu-id="7c986-198">Зависимые параметры ребенка для этой группы параметров</span><span class="sxs-lookup"><span data-stu-id="7c986-198">Dependent child settings to this group of settings</span></span>|
|<span data-ttu-id="7c986-199">dependentOn</span><span class="sxs-lookup"><span data-stu-id="7c986-199">dependentOn</span></span>|<span data-ttu-id="7c986-200">[коллекция deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-200">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="7c986-201">Список зависимостей для группы параметров</span><span class="sxs-lookup"><span data-stu-id="7c986-201">List of Dependencies for the setting group</span></span>|
|<span data-ttu-id="7c986-202">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="7c986-202">dependedOnBy</span></span>|<span data-ttu-id="7c986-203">[коллекция deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="7c986-203">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="7c986-204">Список параметров ребенка, которые зависят от этого параметра</span><span class="sxs-lookup"><span data-stu-id="7c986-204">List of child settings that depend on this setting</span></span>|



## <a name="response"></a><span data-ttu-id="7c986-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c986-205">Response</span></span>
<span data-ttu-id="7c986-206">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7c986-206">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c986-207">Пример</span><span class="sxs-lookup"><span data-stu-id="7c986-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c986-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c986-208">Request</span></span>
<span data-ttu-id="7c986-209">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c986-209">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reusableSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 1729

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
  "referredSettingInformationList": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
      "settingDefinitionId": "Setting Definition Id value"
    }
  ],
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

### <a name="response"></a><span data-ttu-id="7c986-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c986-210">Response</span></span>
<span data-ttu-id="7c986-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c986-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1778

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
  "referredSettingInformationList": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
      "settingDefinitionId": "Setting Definition Id value"
    }
  ],
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




