---
title: Обновление deviceManagementConfigurationChoiceSettingDefinition
description: Обновление свойств объекта deviceManagementConfigurationChoiceSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8f348ccf7da8bcf2447993f048cbf7f37287dcd7
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156555"
---
# <a name="update-devicemanagementconfigurationchoicesettingdefinition"></a><span data-ttu-id="d5b5f-103">Обновление deviceManagementConfigurationChoiceSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="d5b5f-103">Update deviceManagementConfigurationChoiceSettingDefinition</span></span>

<span data-ttu-id="d5b5f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5b5f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5b5f-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5b5f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5b5f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5b5f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5b5f-107">Обновление свойств объекта [deviceManagementConfigurationChoiceSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-107">Update the properties of a [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5b5f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d5b5f-108">Prerequisites</span></span>
<span data-ttu-id="d5b5f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5b5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5b5f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5b5f-111">Permission type</span></span>|<span data-ttu-id="d5b5f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5b5f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5b5f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5b5f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d5b5f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5b5f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5b5f-116">Not supported.</span></span>|
|<span data-ttu-id="d5b5f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5b5f-117">Application</span></span>|<span data-ttu-id="d5b5f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5b5f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5b5f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5b5f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="d5b5f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d5b5f-120">Request headers</span></span>
|<span data-ttu-id="d5b5f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5b5f-121">Header</span></span>|<span data-ttu-id="d5b5f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d5b5f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5b5f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5b5f-123">Authorization</span></span>|<span data-ttu-id="d5b5f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5b5f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5b5f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d5b5f-125">Accept</span></span>|<span data-ttu-id="d5b5f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5b5f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5b5f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d5b5f-127">Request body</span></span>
<span data-ttu-id="d5b5f-128">В теле запроса предопределение представления объекта [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="d5b5f-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) object.</span></span>

<span data-ttu-id="d5b5f-129">В следующей таблице показаны свойства, необходимые при создании [объекта deviceManagementConfigurationChoiceSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md).</span></span>

|<span data-ttu-id="d5b5f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5b5f-130">Property</span></span>|<span data-ttu-id="d5b5f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d5b5f-131">Type</span></span>|<span data-ttu-id="d5b5f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d5b5f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5b5f-133">применимость</span><span class="sxs-lookup"><span data-stu-id="d5b5f-133">applicability</span></span>|[<span data-ttu-id="d5b5f-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="d5b5f-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="d5b5f-135">Сведения о том, какой параметр устройства применим к inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="d5b5f-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="d5b5f-136">accessTypes</span></span>|[<span data-ttu-id="d5b5f-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="d5b5f-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="d5b5f-138">Режим доступа для чтения и записи параметра. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="d5b5f-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="d5b5f-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="d5b5f-140">keywords</span><span class="sxs-lookup"><span data-stu-id="d5b5f-140">keywords</span></span>|<span data-ttu-id="d5b5f-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d5b5f-141">String collection</span></span>|<span data-ttu-id="d5b5f-142">Маркеры для поиска параметров на унаследованных от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="d5b5f-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="d5b5f-143">infoUrls</span></span>|<span data-ttu-id="d5b5f-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d5b5f-144">String collection</span></span>|<span data-ttu-id="d5b5f-145">Список ссылок, дополнительные сведения о параметре можно найти по адресу Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="d5b5f-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="d5b5f-146">occurrence</span></span>|[<span data-ttu-id="d5b5f-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="d5b5f-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="d5b5f-148">Указывает, требуется ли параметр или не наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="d5b5f-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="d5b5f-149">baseUri</span></span>|<span data-ttu-id="d5b5f-150">String</span><span class="sxs-lookup"><span data-stu-id="d5b5f-150">String</span></span>|<span data-ttu-id="d5b5f-151">Базовый путь CSP Наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="d5b5f-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="d5b5f-152">offsetUri</span></span>|<span data-ttu-id="d5b5f-153">String</span><span class="sxs-lookup"><span data-stu-id="d5b5f-153">String</span></span>|<span data-ttu-id="d5b5f-154">Смещение пути CSP от Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="d5b5f-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="d5b5f-155">rootDefinitionId</span></span>|<span data-ttu-id="d5b5f-156">String</span><span class="sxs-lookup"><span data-stu-id="d5b5f-156">String</span></span>|<span data-ttu-id="d5b5f-157">Определение корневого параметра, если этот параметр является параметром-child.</span><span class="sxs-lookup"><span data-stu-id="d5b5f-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="d5b5f-158">Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="d5b5f-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="d5b5f-159">categoryId</span></span>|<span data-ttu-id="d5b5f-160">String</span><span class="sxs-lookup"><span data-stu-id="d5b5f-160">String</span></span>|<span data-ttu-id="d5b5f-161">Указывает группу области, в которой настроен параметр в указанном поставщике служб конфигурации (CSP), наследуемом от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="d5b5f-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="d5b5f-162">settingUsage</span></span>|[<span data-ttu-id="d5b5f-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="d5b5f-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="d5b5f-164">Тип параметра, например конфигурация и соответствие. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="d5b5f-165">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="d5b5f-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="d5b5f-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="d5b5f-166">uxBehavior</span></span>|[<span data-ttu-id="d5b5f-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="d5b5f-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="d5b5f-168">Представление типа параметра в UX. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="d5b5f-169">Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="d5b5f-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="d5b5f-170">id</span><span class="sxs-lookup"><span data-stu-id="d5b5f-170">id</span></span>|<span data-ttu-id="d5b5f-171">String</span><span class="sxs-lookup"><span data-stu-id="d5b5f-171">String</span></span>|<span data-ttu-id="d5b5f-172">Идентификатор элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-172">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="d5b5f-173">description</span><span class="sxs-lookup"><span data-stu-id="d5b5f-173">description</span></span>|<span data-ttu-id="d5b5f-174">String</span><span class="sxs-lookup"><span data-stu-id="d5b5f-174">String</span></span>|<span data-ttu-id="d5b5f-175">Описание элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-175">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="d5b5f-176">helpText</span><span class="sxs-lookup"><span data-stu-id="d5b5f-176">helpText</span></span>|<span data-ttu-id="d5b5f-177">String</span><span class="sxs-lookup"><span data-stu-id="d5b5f-177">String</span></span>|<span data-ttu-id="d5b5f-178">Текст справки для элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-178">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="d5b5f-179">name</span><span class="sxs-lookup"><span data-stu-id="d5b5f-179">name</span></span>|<span data-ttu-id="d5b5f-180">String</span><span class="sxs-lookup"><span data-stu-id="d5b5f-180">String</span></span>|<span data-ttu-id="d5b5f-181">Имя элемента. Наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-181">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="d5b5f-182">displayName</span><span class="sxs-lookup"><span data-stu-id="d5b5f-182">displayName</span></span>|<span data-ttu-id="d5b5f-183">String</span><span class="sxs-lookup"><span data-stu-id="d5b5f-183">String</span></span>|<span data-ttu-id="d5b5f-184">Отображающее имя элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-184">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="d5b5f-185">version</span><span class="sxs-lookup"><span data-stu-id="d5b5f-185">version</span></span>|<span data-ttu-id="d5b5f-186">String</span><span class="sxs-lookup"><span data-stu-id="d5b5f-186">String</span></span>|<span data-ttu-id="d5b5f-187">Версия элемента. Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-187">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="d5b5f-188">options</span><span class="sxs-lookup"><span data-stu-id="d5b5f-188">options</span></span>|<span data-ttu-id="d5b5f-189">[Коллекция deviceManagementConfigurationOptionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d5b5f-189">[deviceManagementConfigurationOptionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinition.md) collection</span></span>|<span data-ttu-id="d5b5f-190">Параметры параметра, который можно выбрать</span><span class="sxs-lookup"><span data-stu-id="d5b5f-190">Options for the setting that can be selected</span></span>|
|<span data-ttu-id="d5b5f-191">defaultOptionId</span><span class="sxs-lookup"><span data-stu-id="d5b5f-191">defaultOptionId</span></span>|<span data-ttu-id="d5b5f-192">String</span><span class="sxs-lookup"><span data-stu-id="d5b5f-192">String</span></span>|<span data-ttu-id="d5b5f-193">Параметр выбора по умолчанию</span><span class="sxs-lookup"><span data-stu-id="d5b5f-193">Default option for choice setting</span></span>|



## <a name="response"></a><span data-ttu-id="d5b5f-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5b5f-194">Response</span></span>
<span data-ttu-id="d5b5f-195">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d5b5f-195">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5b5f-196">Пример</span><span class="sxs-lookup"><span data-stu-id="d5b5f-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5b5f-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5b5f-197">Request</span></span>
<span data-ttu-id="d5b5f-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5b5f-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 9906

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingDefinition",
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
  "defaultOptionId": "Default Option Id value"
}
```

### <a name="response"></a><span data-ttu-id="d5b5f-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5b5f-199">Response</span></span>
<span data-ttu-id="d5b5f-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5b5f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9955

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingDefinition",
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
  "id": "30b2258a-258a-30b2-8a25-b2308a25b230",
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
  "defaultOptionId": "Default Option Id value"
}
```




