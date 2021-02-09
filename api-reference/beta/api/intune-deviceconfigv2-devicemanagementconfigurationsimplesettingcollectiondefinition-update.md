---
title: Обновление deviceManagementConfigurationSimpleSettingCollectionDefinition
description: Обновление свойств объекта deviceManagementConfigurationSimpleSettingCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 75004523f63ec1754acb2c72c056c265125fba5c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156527"
---
# <a name="update-devicemanagementconfigurationsimplesettingcollectiondefinition"></a><span data-ttu-id="1fd92-103">Обновление deviceManagementConfigurationSimpleSettingCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="1fd92-103">Update deviceManagementConfigurationSimpleSettingCollectionDefinition</span></span>

<span data-ttu-id="1fd92-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fd92-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1fd92-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fd92-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fd92-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1fd92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fd92-107">Обновление свойств объекта [deviceManagementConfigurationSimpleSettingCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-107">Update the properties of a [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fd92-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1fd92-108">Prerequisites</span></span>
<span data-ttu-id="1fd92-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fd92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fd92-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fd92-111">Permission type</span></span>|<span data-ttu-id="1fd92-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fd92-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fd92-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fd92-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1fd92-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fd92-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1fd92-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fd92-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fd92-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fd92-116">Not supported.</span></span>|
|<span data-ttu-id="1fd92-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1fd92-117">Application</span></span>|<span data-ttu-id="1fd92-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fd92-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fd92-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fd92-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="1fd92-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1fd92-120">Request headers</span></span>
|<span data-ttu-id="1fd92-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1fd92-121">Header</span></span>|<span data-ttu-id="1fd92-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1fd92-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fd92-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1fd92-123">Authorization</span></span>|<span data-ttu-id="1fd92-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fd92-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fd92-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1fd92-125">Accept</span></span>|<span data-ttu-id="1fd92-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1fd92-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fd92-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1fd92-127">Request body</span></span>
<span data-ttu-id="1fd92-128">В теле запроса предопределение представления объекта [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="1fd92-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object.</span></span>

<span data-ttu-id="1fd92-129">В следующей таблице показаны свойства, необходимые при создании [объекта deviceManagementConfigurationSimpleSettingCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md).</span></span>

|<span data-ttu-id="1fd92-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1fd92-130">Property</span></span>|<span data-ttu-id="1fd92-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1fd92-131">Type</span></span>|<span data-ttu-id="1fd92-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1fd92-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fd92-133">применимость</span><span class="sxs-lookup"><span data-stu-id="1fd92-133">applicability</span></span>|[<span data-ttu-id="1fd92-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="1fd92-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="1fd92-135">Сведения о том, какой параметр устройства применим к inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1fd92-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="1fd92-136">accessTypes</span></span>|[<span data-ttu-id="1fd92-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="1fd92-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="1fd92-138">Режим доступа для чтения и записи параметра. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="1fd92-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="1fd92-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="1fd92-140">keywords</span><span class="sxs-lookup"><span data-stu-id="1fd92-140">keywords</span></span>|<span data-ttu-id="1fd92-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1fd92-141">String collection</span></span>|<span data-ttu-id="1fd92-142">Маркеры для поиска параметров на унаследованных от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1fd92-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="1fd92-143">infoUrls</span></span>|<span data-ttu-id="1fd92-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1fd92-144">String collection</span></span>|<span data-ttu-id="1fd92-145">Список ссылок, дополнительные сведения о параметре можно найти по адресу Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1fd92-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="1fd92-146">occurrence</span></span>|[<span data-ttu-id="1fd92-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="1fd92-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="1fd92-148">Указывает, требуется ли параметр или не наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1fd92-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="1fd92-149">baseUri</span></span>|<span data-ttu-id="1fd92-150">String</span><span class="sxs-lookup"><span data-stu-id="1fd92-150">String</span></span>|<span data-ttu-id="1fd92-151">Базовый путь CSP Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1fd92-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="1fd92-152">offsetUri</span></span>|<span data-ttu-id="1fd92-153">String</span><span class="sxs-lookup"><span data-stu-id="1fd92-153">String</span></span>|<span data-ttu-id="1fd92-154">Смещение пути CSP от Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1fd92-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="1fd92-155">rootDefinitionId</span></span>|<span data-ttu-id="1fd92-156">String</span><span class="sxs-lookup"><span data-stu-id="1fd92-156">String</span></span>|<span data-ttu-id="1fd92-157">Определение корневого параметра, если этот параметр является параметром-child.</span><span class="sxs-lookup"><span data-stu-id="1fd92-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="1fd92-158">Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1fd92-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="1fd92-159">categoryId</span></span>|<span data-ttu-id="1fd92-160">String</span><span class="sxs-lookup"><span data-stu-id="1fd92-160">String</span></span>|<span data-ttu-id="1fd92-161">Указывает группу области, в которой настроен параметр в указанном поставщике служб конфигурации (CSP), наследуемом от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1fd92-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="1fd92-162">settingUsage</span></span>|[<span data-ttu-id="1fd92-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="1fd92-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="1fd92-164">Тип параметра, например конфигурация и соответствие. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="1fd92-165">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="1fd92-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="1fd92-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="1fd92-166">uxBehavior</span></span>|[<span data-ttu-id="1fd92-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="1fd92-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="1fd92-168">Представление типа параметра в UX. Наследуется от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="1fd92-169">Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="1fd92-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="1fd92-170">id</span><span class="sxs-lookup"><span data-stu-id="1fd92-170">id</span></span>|<span data-ttu-id="1fd92-171">String</span><span class="sxs-lookup"><span data-stu-id="1fd92-171">String</span></span>|<span data-ttu-id="1fd92-172">Идентификатор элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-172">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1fd92-173">description</span><span class="sxs-lookup"><span data-stu-id="1fd92-173">description</span></span>|<span data-ttu-id="1fd92-174">String</span><span class="sxs-lookup"><span data-stu-id="1fd92-174">String</span></span>|<span data-ttu-id="1fd92-175">Описание элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-175">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1fd92-176">helpText</span><span class="sxs-lookup"><span data-stu-id="1fd92-176">helpText</span></span>|<span data-ttu-id="1fd92-177">String</span><span class="sxs-lookup"><span data-stu-id="1fd92-177">String</span></span>|<span data-ttu-id="1fd92-178">Текст справки для элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-178">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1fd92-179">name</span><span class="sxs-lookup"><span data-stu-id="1fd92-179">name</span></span>|<span data-ttu-id="1fd92-180">String</span><span class="sxs-lookup"><span data-stu-id="1fd92-180">String</span></span>|<span data-ttu-id="1fd92-181">Имя элемента. Наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-181">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1fd92-182">displayName</span><span class="sxs-lookup"><span data-stu-id="1fd92-182">displayName</span></span>|<span data-ttu-id="1fd92-183">String</span><span class="sxs-lookup"><span data-stu-id="1fd92-183">String</span></span>|<span data-ttu-id="1fd92-184">Отображающее имя элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-184">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1fd92-185">version</span><span class="sxs-lookup"><span data-stu-id="1fd92-185">version</span></span>|<span data-ttu-id="1fd92-186">String</span><span class="sxs-lookup"><span data-stu-id="1fd92-186">String</span></span>|<span data-ttu-id="1fd92-187">Версия элемента. Наследуется [от deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-187">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1fd92-188">valueDefinition</span><span class="sxs-lookup"><span data-stu-id="1fd92-188">valueDefinition</span></span>|[<span data-ttu-id="1fd92-189">deviceManagementConfigurationSettingValueDefinition</span><span class="sxs-lookup"><span data-stu-id="1fd92-189">deviceManagementConfigurationSettingValueDefinition</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)|<span data-ttu-id="1fd92-190">Определение значения для этого параметра Наследуется от [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-190">Definition of the value for this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="1fd92-191">defaultValue</span><span class="sxs-lookup"><span data-stu-id="1fd92-191">defaultValue</span></span>|[<span data-ttu-id="1fd92-192">deviceManagementConfigurationSettingValue</span><span class="sxs-lookup"><span data-stu-id="1fd92-192">deviceManagementConfigurationSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|<span data-ttu-id="1fd92-193">Значение по умолчанию для этого параметра. Наследуется от [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-193">Default setting value for this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="1fd92-194">dependentOn</span><span class="sxs-lookup"><span data-stu-id="1fd92-194">dependentOn</span></span>|<span data-ttu-id="1fd92-195">[Коллекция deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-195">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="1fd92-196">список родительских параметров, которые этот параметр зависит от унаследованных от [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-196">list of parent settings this setting is dependent on Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="1fd92-197">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="1fd92-197">dependedOnBy</span></span>|<span data-ttu-id="1fd92-198">[Коллекция deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-198">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="1fd92-199">список параметров, которые зависят от этого параметра. Наследуется от [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1fd92-199">list of child settings that depend on this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="1fd92-200">maximumCount</span><span class="sxs-lookup"><span data-stu-id="1fd92-200">maximumCount</span></span>|<span data-ttu-id="1fd92-201">Int32</span><span class="sxs-lookup"><span data-stu-id="1fd92-201">Int32</span></span>|<span data-ttu-id="1fd92-202">Максимальное количество простых параметров в коллекции.</span><span class="sxs-lookup"><span data-stu-id="1fd92-202">Maximum number of simple settings in the collection.</span></span> <span data-ttu-id="1fd92-203">Допустимые значения: от 1 до 100</span><span class="sxs-lookup"><span data-stu-id="1fd92-203">Valid values 1 to 100</span></span>|
|<span data-ttu-id="1fd92-204">minimumCount</span><span class="sxs-lookup"><span data-stu-id="1fd92-204">minimumCount</span></span>|<span data-ttu-id="1fd92-205">Int32</span><span class="sxs-lookup"><span data-stu-id="1fd92-205">Int32</span></span>|<span data-ttu-id="1fd92-206">Минимальное количество простых параметров в коллекции.</span><span class="sxs-lookup"><span data-stu-id="1fd92-206">Minimum number of simple settings in the collection.</span></span> <span data-ttu-id="1fd92-207">Допустимые значения: от 1 до 100</span><span class="sxs-lookup"><span data-stu-id="1fd92-207">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="1fd92-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fd92-208">Response</span></span>
<span data-ttu-id="1fd92-209">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1fd92-209">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fd92-210">Пример</span><span class="sxs-lookup"><span data-stu-id="1fd92-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fd92-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fd92-211">Request</span></span>
<span data-ttu-id="1fd92-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1fd92-212">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 9212

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionDefinition",
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
  "valueDefinition": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueDefinition"
  },
  "defaultValue": {
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
  "maximumCount": 12,
  "minimumCount": 12
}
```

### <a name="response"></a><span data-ttu-id="1fd92-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fd92-213">Response</span></span>
<span data-ttu-id="1fd92-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1fd92-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9261

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionDefinition",
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
  "id": "cb4abda1-bda1-cb4a-a1bd-4acba1bd4acb",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value",
  "valueDefinition": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueDefinition"
  },
  "defaultValue": {
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
  "maximumCount": 12,
  "minimumCount": 12
}
```




