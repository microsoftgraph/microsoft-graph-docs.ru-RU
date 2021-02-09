---
title: Создание deviceManagementConfigurationSettingGroupCollectionDefinition
description: Создание объекта deviceManagementConfigurationSettingGroupCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0eb43368c20fda197a6449db31ad29ec7f296b10
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156548"
---
# <a name="create-devicemanagementconfigurationsettinggroupcollectiondefinition"></a><span data-ttu-id="dbb09-103">Создание deviceManagementConfigurationSettingGroupCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="dbb09-103">Create deviceManagementConfigurationSettingGroupCollectionDefinition</span></span>

<span data-ttu-id="dbb09-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbb09-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dbb09-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbb09-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dbb09-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dbb09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbb09-107">Создание объекта [deviceManagementConfigurationSettingGroupCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-107">Create a new [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dbb09-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dbb09-108">Prerequisites</span></span>
<span data-ttu-id="dbb09-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbb09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbb09-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dbb09-111">Permission type</span></span>|<span data-ttu-id="dbb09-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dbb09-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbb09-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dbb09-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dbb09-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbb09-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dbb09-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dbb09-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbb09-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbb09-116">Not supported.</span></span>|
|<span data-ttu-id="dbb09-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dbb09-117">Application</span></span>|<span data-ttu-id="dbb09-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dbb09-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbb09-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dbb09-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="dbb09-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dbb09-120">Request headers</span></span>
|<span data-ttu-id="dbb09-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dbb09-121">Header</span></span>|<span data-ttu-id="dbb09-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dbb09-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbb09-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dbb09-123">Authorization</span></span>|<span data-ttu-id="dbb09-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dbb09-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbb09-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dbb09-125">Accept</span></span>|<span data-ttu-id="dbb09-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dbb09-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbb09-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dbb09-127">Request body</span></span>
<span data-ttu-id="dbb09-128">В теле запроса предопределение представления объекта deviceManagementConfigurationSettingGroupCollectionDefinition в JSON.</span><span class="sxs-lookup"><span data-stu-id="dbb09-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingGroupCollectionDefinition object.</span></span>

<span data-ttu-id="dbb09-129">В следующей таблице показаны свойства, необходимые при создании объекта deviceManagementConfigurationSettingGroupCollectionDefinition.</span><span class="sxs-lookup"><span data-stu-id="dbb09-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingGroupCollectionDefinition.</span></span>

|<span data-ttu-id="dbb09-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dbb09-130">Property</span></span>|<span data-ttu-id="dbb09-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dbb09-131">Type</span></span>|<span data-ttu-id="dbb09-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dbb09-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbb09-133">применимость</span><span class="sxs-lookup"><span data-stu-id="dbb09-133">applicability</span></span>|[<span data-ttu-id="dbb09-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="dbb09-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="dbb09-135">Сведения о том, какой параметр устройства применим к inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="dbb09-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="dbb09-136">accessTypes</span></span>|[<span data-ttu-id="dbb09-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="dbb09-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="dbb09-138">Режим доступа для чтения и записи параметра. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="dbb09-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="dbb09-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="dbb09-140">keywords</span><span class="sxs-lookup"><span data-stu-id="dbb09-140">keywords</span></span>|<span data-ttu-id="dbb09-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dbb09-141">String collection</span></span>|<span data-ttu-id="dbb09-142">Маркеры для поиска параметров на унаследованных от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="dbb09-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="dbb09-143">infoUrls</span></span>|<span data-ttu-id="dbb09-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dbb09-144">String collection</span></span>|<span data-ttu-id="dbb09-145">Список ссылок, дополнительные сведения о параметре можно найти по адресу Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="dbb09-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="dbb09-146">occurrence</span></span>|[<span data-ttu-id="dbb09-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="dbb09-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="dbb09-148">Указывает, требуется ли параметр или не наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="dbb09-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="dbb09-149">baseUri</span></span>|<span data-ttu-id="dbb09-150">String</span><span class="sxs-lookup"><span data-stu-id="dbb09-150">String</span></span>|<span data-ttu-id="dbb09-151">Базовый путь CSP Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="dbb09-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="dbb09-152">offsetUri</span></span>|<span data-ttu-id="dbb09-153">String</span><span class="sxs-lookup"><span data-stu-id="dbb09-153">String</span></span>|<span data-ttu-id="dbb09-154">Смещение пути CSP от Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="dbb09-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="dbb09-155">rootDefinitionId</span></span>|<span data-ttu-id="dbb09-156">String</span><span class="sxs-lookup"><span data-stu-id="dbb09-156">String</span></span>|<span data-ttu-id="dbb09-157">Определение корневого параметра, если этот параметр является параметром-child.</span><span class="sxs-lookup"><span data-stu-id="dbb09-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="dbb09-158">Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="dbb09-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="dbb09-159">categoryId</span></span>|<span data-ttu-id="dbb09-160">String</span><span class="sxs-lookup"><span data-stu-id="dbb09-160">String</span></span>|<span data-ttu-id="dbb09-161">Указывает группу области, в которой настроен параметр в указанном поставщике служб конфигурации (CSP), наследуемом от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="dbb09-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="dbb09-162">settingUsage</span></span>|[<span data-ttu-id="dbb09-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="dbb09-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="dbb09-164">Тип параметра, например конфигурация и соответствие. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="dbb09-165">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="dbb09-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="dbb09-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="dbb09-166">uxBehavior</span></span>|[<span data-ttu-id="dbb09-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="dbb09-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="dbb09-168">Представление типа параметра в UX. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="dbb09-169">Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="dbb09-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="dbb09-170">id</span><span class="sxs-lookup"><span data-stu-id="dbb09-170">id</span></span>|<span data-ttu-id="dbb09-171">String</span><span class="sxs-lookup"><span data-stu-id="dbb09-171">String</span></span>|<span data-ttu-id="dbb09-172">Идентификатор элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-172">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="dbb09-173">description</span><span class="sxs-lookup"><span data-stu-id="dbb09-173">description</span></span>|<span data-ttu-id="dbb09-174">String</span><span class="sxs-lookup"><span data-stu-id="dbb09-174">String</span></span>|<span data-ttu-id="dbb09-175">Описание элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-175">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="dbb09-176">helpText</span><span class="sxs-lookup"><span data-stu-id="dbb09-176">helpText</span></span>|<span data-ttu-id="dbb09-177">String</span><span class="sxs-lookup"><span data-stu-id="dbb09-177">String</span></span>|<span data-ttu-id="dbb09-178">Текст справки для элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-178">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="dbb09-179">name</span><span class="sxs-lookup"><span data-stu-id="dbb09-179">name</span></span>|<span data-ttu-id="dbb09-180">String</span><span class="sxs-lookup"><span data-stu-id="dbb09-180">String</span></span>|<span data-ttu-id="dbb09-181">Имя элемента. Наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-181">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="dbb09-182">displayName</span><span class="sxs-lookup"><span data-stu-id="dbb09-182">displayName</span></span>|<span data-ttu-id="dbb09-183">String</span><span class="sxs-lookup"><span data-stu-id="dbb09-183">String</span></span>|<span data-ttu-id="dbb09-184">Отображающее имя элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-184">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="dbb09-185">version</span><span class="sxs-lookup"><span data-stu-id="dbb09-185">version</span></span>|<span data-ttu-id="dbb09-186">String</span><span class="sxs-lookup"><span data-stu-id="dbb09-186">String</span></span>|<span data-ttu-id="dbb09-187">Версия элемента. Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-187">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="dbb09-188">childIds</span><span class="sxs-lookup"><span data-stu-id="dbb09-188">childIds</span></span>|<span data-ttu-id="dbb09-189">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dbb09-189">String collection</span></span>|<span data-ttu-id="dbb09-190">Зависимые параметры для этой группы параметров. Наследуется от [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-190">Dependent child settings to this group of settings Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="dbb09-191">dependentOn</span><span class="sxs-lookup"><span data-stu-id="dbb09-191">dependentOn</span></span>|<span data-ttu-id="dbb09-192">[Коллекция deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-192">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="dbb09-193">Список зависимостей для группы параметров Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-193">List of Dependencies for the setting group Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="dbb09-194">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="dbb09-194">dependedOnBy</span></span>|<span data-ttu-id="dbb09-195">[Коллекция deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-195">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="dbb09-196">Список параметров, которые зависят от этого параметра. Наследуется от [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dbb09-196">List of child settings that depend on this setting Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="dbb09-197">maximumCount</span><span class="sxs-lookup"><span data-stu-id="dbb09-197">maximumCount</span></span>|<span data-ttu-id="dbb09-198">Int32</span><span class="sxs-lookup"><span data-stu-id="dbb09-198">Int32</span></span>|<span data-ttu-id="dbb09-199">Максимальное количество параметров в коллекции.</span><span class="sxs-lookup"><span data-stu-id="dbb09-199">Maximum number of setting group count in the collection.</span></span> <span data-ttu-id="dbb09-200">Допустимые значения: от 1 до 100</span><span class="sxs-lookup"><span data-stu-id="dbb09-200">Valid values 1 to 100</span></span>|
|<span data-ttu-id="dbb09-201">minimumCount</span><span class="sxs-lookup"><span data-stu-id="dbb09-201">minimumCount</span></span>|<span data-ttu-id="dbb09-202">Int32</span><span class="sxs-lookup"><span data-stu-id="dbb09-202">Int32</span></span>|<span data-ttu-id="dbb09-203">Минимальное количество параметров в коллекции.</span><span class="sxs-lookup"><span data-stu-id="dbb09-203">Minimum number of setting group count in the collection.</span></span> <span data-ttu-id="dbb09-204">Допустимые значения: от 1 до 100</span><span class="sxs-lookup"><span data-stu-id="dbb09-204">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="dbb09-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbb09-205">Response</span></span>
<span data-ttu-id="dbb09-206">В случае успешного выполнения этот метод возвращает код отклика и объект `201 Created` [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dbb09-206">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbb09-207">Пример</span><span class="sxs-lookup"><span data-stu-id="dbb09-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="dbb09-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="dbb09-208">Request</span></span>
<span data-ttu-id="dbb09-209">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dbb09-209">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 1533

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupCollectionDefinition",
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
  ],
  "maximumCount": 12,
  "minimumCount": 12
}
```

### <a name="response"></a><span data-ttu-id="dbb09-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="dbb09-210">Response</span></span>
<span data-ttu-id="dbb09-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dbb09-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1582

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupCollectionDefinition",
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
  "id": "739da194-a194-739d-94a1-9d7394a19d73",
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
  ],
  "maximumCount": 12,
  "minimumCount": 12
}
```




