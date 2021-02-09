---
title: Создание deviceManagementConfigurationSettingGroupDefinition
description: Создание объекта deviceManagementConfigurationSettingGroupDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cf8c4d88e032f6a5f388cc62e118791e7cbb8300
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161322"
---
# <a name="create-devicemanagementconfigurationsettinggroupdefinition"></a><span data-ttu-id="c0eec-103">Создание deviceManagementConfigurationSettingGroupDefinition</span><span class="sxs-lookup"><span data-stu-id="c0eec-103">Create deviceManagementConfigurationSettingGroupDefinition</span></span>

<span data-ttu-id="c0eec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0eec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0eec-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0eec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0eec-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0eec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0eec-107">Создание объекта [deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0eec-107">Create a new [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0eec-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c0eec-108">Prerequisites</span></span>
<span data-ttu-id="c0eec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0eec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0eec-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0eec-111">Permission type</span></span>|<span data-ttu-id="c0eec-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0eec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0eec-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0eec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0eec-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0eec-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c0eec-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0eec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0eec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0eec-116">Not supported.</span></span>|
|<span data-ttu-id="c0eec-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0eec-117">Application</span></span>|<span data-ttu-id="c0eec-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0eec-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0eec-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0eec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="c0eec-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c0eec-120">Request headers</span></span>
|<span data-ttu-id="c0eec-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c0eec-121">Header</span></span>|<span data-ttu-id="c0eec-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c0eec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0eec-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0eec-123">Authorization</span></span>|<span data-ttu-id="c0eec-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0eec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0eec-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c0eec-125">Accept</span></span>|<span data-ttu-id="c0eec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0eec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0eec-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0eec-127">Request body</span></span>
<span data-ttu-id="c0eec-128">В теле запроса предопределение представления объекта deviceManagementConfigurationSettingGroupDefinition в JSON.</span><span class="sxs-lookup"><span data-stu-id="c0eec-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingGroupDefinition object.</span></span>

<span data-ttu-id="c0eec-129">В следующей таблице показаны свойства, необходимые при создании объекта deviceManagementConfigurationSettingGroupDefinition.</span><span class="sxs-lookup"><span data-stu-id="c0eec-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingGroupDefinition.</span></span>

|<span data-ttu-id="c0eec-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0eec-130">Property</span></span>|<span data-ttu-id="c0eec-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c0eec-131">Type</span></span>|<span data-ttu-id="c0eec-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c0eec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0eec-133">применимость</span><span class="sxs-lookup"><span data-stu-id="c0eec-133">applicability</span></span>|[<span data-ttu-id="c0eec-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="c0eec-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="c0eec-135">Сведения о том, какой параметр устройства применим к inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0eec-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="c0eec-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="c0eec-136">accessTypes</span></span>|[<span data-ttu-id="c0eec-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="c0eec-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="c0eec-138">Режим доступа для чтения и записи параметра. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0eec-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="c0eec-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="c0eec-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="c0eec-140">keywords</span><span class="sxs-lookup"><span data-stu-id="c0eec-140">keywords</span></span>|<span data-ttu-id="c0eec-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c0eec-141">String collection</span></span>|<span data-ttu-id="c0eec-142">Маркеры для поиска параметров на унаследованных от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0eec-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="c0eec-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="c0eec-143">infoUrls</span></span>|<span data-ttu-id="c0eec-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c0eec-144">String collection</span></span>|<span data-ttu-id="c0eec-145">Список ссылок, дополнительные сведения о параметре можно найти по адресу Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0eec-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="c0eec-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="c0eec-146">occurrence</span></span>|[<span data-ttu-id="c0eec-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="c0eec-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="c0eec-148">Указывает, требуется ли параметр или не наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0eec-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="c0eec-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="c0eec-149">baseUri</span></span>|<span data-ttu-id="c0eec-150">String</span><span class="sxs-lookup"><span data-stu-id="c0eec-150">String</span></span>|<span data-ttu-id="c0eec-151">Базовый путь CSP Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0eec-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="c0eec-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="c0eec-152">offsetUri</span></span>|<span data-ttu-id="c0eec-153">String</span><span class="sxs-lookup"><span data-stu-id="c0eec-153">String</span></span>|<span data-ttu-id="c0eec-154">Смещение пути CSP от Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0eec-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="c0eec-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c0eec-155">rootDefinitionId</span></span>|<span data-ttu-id="c0eec-156">String</span><span class="sxs-lookup"><span data-stu-id="c0eec-156">String</span></span>|<span data-ttu-id="c0eec-157">Определение корневого параметра, если этот параметр является параметром-child.</span><span class="sxs-lookup"><span data-stu-id="c0eec-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="c0eec-158">Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0eec-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="c0eec-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="c0eec-159">categoryId</span></span>|<span data-ttu-id="c0eec-160">String</span><span class="sxs-lookup"><span data-stu-id="c0eec-160">String</span></span>|<span data-ttu-id="c0eec-161">Указывает группу области, в которой настроен параметр в указанном поставщике служб конфигурации (CSP), наследуемом от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0eec-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="c0eec-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="c0eec-162">settingUsage</span></span>|[<span data-ttu-id="c0eec-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="c0eec-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="c0eec-164">Тип параметра, например конфигурация и соответствие. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0eec-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="c0eec-165">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="c0eec-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="c0eec-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="c0eec-166">uxBehavior</span></span>|[<span data-ttu-id="c0eec-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="c0eec-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="c0eec-168">Представление типа параметра в UX. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0eec-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="c0eec-169">Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="c0eec-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="c0eec-170">id</span><span class="sxs-lookup"><span data-stu-id="c0eec-170">id</span></span>|<span data-ttu-id="c0eec-171">String</span><span class="sxs-lookup"><span data-stu-id="c0eec-171">String</span></span>|<span data-ttu-id="c0eec-172">Идентификатор элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0eec-172">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="c0eec-173">description</span><span class="sxs-lookup"><span data-stu-id="c0eec-173">description</span></span>|<span data-ttu-id="c0eec-174">String</span><span class="sxs-lookup"><span data-stu-id="c0eec-174">String</span></span>|<span data-ttu-id="c0eec-175">Описание элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0eec-175">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="c0eec-176">helpText</span><span class="sxs-lookup"><span data-stu-id="c0eec-176">helpText</span></span>|<span data-ttu-id="c0eec-177">String</span><span class="sxs-lookup"><span data-stu-id="c0eec-177">String</span></span>|<span data-ttu-id="c0eec-178">Текст справки для элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0eec-178">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="c0eec-179">name</span><span class="sxs-lookup"><span data-stu-id="c0eec-179">name</span></span>|<span data-ttu-id="c0eec-180">String</span><span class="sxs-lookup"><span data-stu-id="c0eec-180">String</span></span>|<span data-ttu-id="c0eec-181">Имя элемента. Наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0eec-181">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="c0eec-182">displayName</span><span class="sxs-lookup"><span data-stu-id="c0eec-182">displayName</span></span>|<span data-ttu-id="c0eec-183">String</span><span class="sxs-lookup"><span data-stu-id="c0eec-183">String</span></span>|<span data-ttu-id="c0eec-184">Отображающее имя элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0eec-184">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="c0eec-185">version</span><span class="sxs-lookup"><span data-stu-id="c0eec-185">version</span></span>|<span data-ttu-id="c0eec-186">String</span><span class="sxs-lookup"><span data-stu-id="c0eec-186">String</span></span>|<span data-ttu-id="c0eec-187">Версия элемента. Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0eec-187">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="c0eec-188">childIds</span><span class="sxs-lookup"><span data-stu-id="c0eec-188">childIds</span></span>|<span data-ttu-id="c0eec-189">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c0eec-189">String collection</span></span>|<span data-ttu-id="c0eec-190">Зависимые параметры для этой группы параметров</span><span class="sxs-lookup"><span data-stu-id="c0eec-190">Dependent child settings to this group of settings</span></span>|
|<span data-ttu-id="c0eec-191">dependentOn</span><span class="sxs-lookup"><span data-stu-id="c0eec-191">dependentOn</span></span>|<span data-ttu-id="c0eec-192">[Коллекция deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="c0eec-192">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="c0eec-193">Список зависимостей для группы параметров</span><span class="sxs-lookup"><span data-stu-id="c0eec-193">List of Dependencies for the setting group</span></span>|
|<span data-ttu-id="c0eec-194">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="c0eec-194">dependedOnBy</span></span>|<span data-ttu-id="c0eec-195">[Коллекция deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="c0eec-195">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="c0eec-196">Список параметров, которые зависят от этого параметра</span><span class="sxs-lookup"><span data-stu-id="c0eec-196">List of child settings that depend on this setting</span></span>|



## <a name="response"></a><span data-ttu-id="c0eec-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0eec-197">Response</span></span>
<span data-ttu-id="c0eec-198">В случае успешного выполнения этот метод возвращает код отклика и объект `201 Created` [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c0eec-198">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0eec-199">Пример</span><span class="sxs-lookup"><span data-stu-id="c0eec-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0eec-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0eec-200">Request</span></span>
<span data-ttu-id="c0eec-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0eec-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
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

### <a name="response"></a><span data-ttu-id="c0eec-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0eec-202">Response</span></span>
<span data-ttu-id="c0eec-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c0eec-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




