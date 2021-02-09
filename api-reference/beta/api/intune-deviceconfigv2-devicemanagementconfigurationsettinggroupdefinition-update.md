---
title: Обновление deviceManagementConfigurationSettingGroupDefinition
description: Обновление свойств объекта deviceManagementConfigurationSettingGroupDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 61c2d97af46e718d31eace72ac2b19c437410bb4
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158921"
---
# <a name="update-devicemanagementconfigurationsettinggroupdefinition"></a><span data-ttu-id="24ccf-103">Обновление deviceManagementConfigurationSettingGroupDefinition</span><span class="sxs-lookup"><span data-stu-id="24ccf-103">Update deviceManagementConfigurationSettingGroupDefinition</span></span>

<span data-ttu-id="24ccf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24ccf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24ccf-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24ccf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24ccf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24ccf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24ccf-107">Обновление свойств объекта [deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-107">Update the properties of a [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24ccf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="24ccf-108">Prerequisites</span></span>
<span data-ttu-id="24ccf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24ccf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24ccf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24ccf-111">Permission type</span></span>|<span data-ttu-id="24ccf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="24ccf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24ccf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24ccf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24ccf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24ccf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="24ccf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24ccf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24ccf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24ccf-116">Not supported.</span></span>|
|<span data-ttu-id="24ccf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24ccf-117">Application</span></span>|<span data-ttu-id="24ccf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24ccf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24ccf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24ccf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="24ccf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="24ccf-120">Request headers</span></span>
|<span data-ttu-id="24ccf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24ccf-121">Header</span></span>|<span data-ttu-id="24ccf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="24ccf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24ccf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24ccf-123">Authorization</span></span>|<span data-ttu-id="24ccf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24ccf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24ccf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="24ccf-125">Accept</span></span>|<span data-ttu-id="24ccf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24ccf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24ccf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24ccf-127">Request body</span></span>
<span data-ttu-id="24ccf-128">В теле запроса предопределение представления объекта [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="24ccf-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

<span data-ttu-id="24ccf-129">В следующей таблице показаны свойства, необходимые при создании [объекта deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md).</span></span>

|<span data-ttu-id="24ccf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="24ccf-130">Property</span></span>|<span data-ttu-id="24ccf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="24ccf-131">Type</span></span>|<span data-ttu-id="24ccf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="24ccf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24ccf-133">применимость</span><span class="sxs-lookup"><span data-stu-id="24ccf-133">applicability</span></span>|[<span data-ttu-id="24ccf-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="24ccf-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="24ccf-135">Сведения о том, какой параметр устройства применим к inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="24ccf-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="24ccf-136">accessTypes</span></span>|[<span data-ttu-id="24ccf-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="24ccf-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="24ccf-138">Режим доступа для чтения и записи параметра. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="24ccf-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="24ccf-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="24ccf-140">keywords</span><span class="sxs-lookup"><span data-stu-id="24ccf-140">keywords</span></span>|<span data-ttu-id="24ccf-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="24ccf-141">String collection</span></span>|<span data-ttu-id="24ccf-142">Маркеры для поиска параметров на унаследованных от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="24ccf-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="24ccf-143">infoUrls</span></span>|<span data-ttu-id="24ccf-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="24ccf-144">String collection</span></span>|<span data-ttu-id="24ccf-145">Список ссылок, дополнительные сведения о параметре можно найти по адресу Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="24ccf-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="24ccf-146">occurrence</span></span>|[<span data-ttu-id="24ccf-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="24ccf-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="24ccf-148">Указывает, требуется ли параметр или не наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="24ccf-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="24ccf-149">baseUri</span></span>|<span data-ttu-id="24ccf-150">String</span><span class="sxs-lookup"><span data-stu-id="24ccf-150">String</span></span>|<span data-ttu-id="24ccf-151">Базовый путь CSP Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="24ccf-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="24ccf-152">offsetUri</span></span>|<span data-ttu-id="24ccf-153">String</span><span class="sxs-lookup"><span data-stu-id="24ccf-153">String</span></span>|<span data-ttu-id="24ccf-154">Смещение пути CSP от Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="24ccf-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="24ccf-155">rootDefinitionId</span></span>|<span data-ttu-id="24ccf-156">String</span><span class="sxs-lookup"><span data-stu-id="24ccf-156">String</span></span>|<span data-ttu-id="24ccf-157">Определение корневого параметра, если этот параметр является параметром-child.</span><span class="sxs-lookup"><span data-stu-id="24ccf-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="24ccf-158">Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="24ccf-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="24ccf-159">categoryId</span></span>|<span data-ttu-id="24ccf-160">String</span><span class="sxs-lookup"><span data-stu-id="24ccf-160">String</span></span>|<span data-ttu-id="24ccf-161">Указывает группу области, в которой настроен параметр в указанном поставщике служб конфигурации (CSP), наследуемом от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="24ccf-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="24ccf-162">settingUsage</span></span>|[<span data-ttu-id="24ccf-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="24ccf-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="24ccf-164">Тип параметра, например конфигурация и соответствие. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="24ccf-165">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="24ccf-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="24ccf-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="24ccf-166">uxBehavior</span></span>|[<span data-ttu-id="24ccf-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="24ccf-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="24ccf-168">Представление типа параметра в UX. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="24ccf-169">Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="24ccf-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="24ccf-170">id</span><span class="sxs-lookup"><span data-stu-id="24ccf-170">id</span></span>|<span data-ttu-id="24ccf-171">String</span><span class="sxs-lookup"><span data-stu-id="24ccf-171">String</span></span>|<span data-ttu-id="24ccf-172">Идентификатор элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-172">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="24ccf-173">description</span><span class="sxs-lookup"><span data-stu-id="24ccf-173">description</span></span>|<span data-ttu-id="24ccf-174">String</span><span class="sxs-lookup"><span data-stu-id="24ccf-174">String</span></span>|<span data-ttu-id="24ccf-175">Описание элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-175">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="24ccf-176">helpText</span><span class="sxs-lookup"><span data-stu-id="24ccf-176">helpText</span></span>|<span data-ttu-id="24ccf-177">String</span><span class="sxs-lookup"><span data-stu-id="24ccf-177">String</span></span>|<span data-ttu-id="24ccf-178">Текст справки для элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-178">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="24ccf-179">name</span><span class="sxs-lookup"><span data-stu-id="24ccf-179">name</span></span>|<span data-ttu-id="24ccf-180">String</span><span class="sxs-lookup"><span data-stu-id="24ccf-180">String</span></span>|<span data-ttu-id="24ccf-181">Имя элемента. Наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-181">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="24ccf-182">displayName</span><span class="sxs-lookup"><span data-stu-id="24ccf-182">displayName</span></span>|<span data-ttu-id="24ccf-183">String</span><span class="sxs-lookup"><span data-stu-id="24ccf-183">String</span></span>|<span data-ttu-id="24ccf-184">Отображающее имя элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-184">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="24ccf-185">version</span><span class="sxs-lookup"><span data-stu-id="24ccf-185">version</span></span>|<span data-ttu-id="24ccf-186">String</span><span class="sxs-lookup"><span data-stu-id="24ccf-186">String</span></span>|<span data-ttu-id="24ccf-187">Версия элемента. Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-187">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="24ccf-188">childIds</span><span class="sxs-lookup"><span data-stu-id="24ccf-188">childIds</span></span>|<span data-ttu-id="24ccf-189">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="24ccf-189">String collection</span></span>|<span data-ttu-id="24ccf-190">Зависимые параметры для этой группы параметров</span><span class="sxs-lookup"><span data-stu-id="24ccf-190">Dependent child settings to this group of settings</span></span>|
|<span data-ttu-id="24ccf-191">dependentOn</span><span class="sxs-lookup"><span data-stu-id="24ccf-191">dependentOn</span></span>|<span data-ttu-id="24ccf-192">[Коллекция deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-192">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="24ccf-193">Список зависимостей для группы параметров</span><span class="sxs-lookup"><span data-stu-id="24ccf-193">List of Dependencies for the setting group</span></span>|
|<span data-ttu-id="24ccf-194">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="24ccf-194">dependedOnBy</span></span>|<span data-ttu-id="24ccf-195">[Коллекция deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="24ccf-195">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="24ccf-196">Список параметров, которые зависят от этого параметра</span><span class="sxs-lookup"><span data-stu-id="24ccf-196">List of child settings that depend on this setting</span></span>|



## <a name="response"></a><span data-ttu-id="24ccf-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="24ccf-197">Response</span></span>
<span data-ttu-id="24ccf-198">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="24ccf-198">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24ccf-199">Пример</span><span class="sxs-lookup"><span data-stu-id="24ccf-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="24ccf-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="24ccf-200">Request</span></span>
<span data-ttu-id="24ccf-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24ccf-201">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 1477

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

### <a name="response"></a><span data-ttu-id="24ccf-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="24ccf-202">Response</span></span>
<span data-ttu-id="24ccf-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24ccf-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1526

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




