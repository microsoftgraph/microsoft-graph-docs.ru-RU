---
title: Обновление deviceManagementConfigurationSettingGroupDefinition
description: Обновление свойств объекта deviceManagementConfigurationSettingGroupDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0533dc0db73b49545d3d63eaf5cb413a74c6e3d5
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866638"
---
# <a name="update-devicemanagementconfigurationsettinggroupdefinition"></a><span data-ttu-id="1f43d-103">Обновление deviceManagementConfigurationSettingGroupDefinition</span><span class="sxs-lookup"><span data-stu-id="1f43d-103">Update deviceManagementConfigurationSettingGroupDefinition</span></span>

<span data-ttu-id="1f43d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f43d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f43d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f43d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f43d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f43d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f43d-107">Обновление свойств объекта [deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-107">Update the properties of a [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f43d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1f43d-108">Prerequisites</span></span>
<span data-ttu-id="1f43d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f43d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f43d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f43d-111">Permission type</span></span>|<span data-ttu-id="1f43d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f43d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f43d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f43d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f43d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f43d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1f43d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f43d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f43d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f43d-116">Not supported.</span></span>|
|<span data-ttu-id="1f43d-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="1f43d-117">Application</span></span>|<span data-ttu-id="1f43d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f43d-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f43d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f43d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reusableSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="1f43d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1f43d-120">Request headers</span></span>
|<span data-ttu-id="1f43d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f43d-121">Header</span></span>|<span data-ttu-id="1f43d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1f43d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f43d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f43d-123">Authorization</span></span>|<span data-ttu-id="1f43d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f43d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f43d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1f43d-125">Accept</span></span>|<span data-ttu-id="1f43d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1f43d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f43d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f43d-127">Request body</span></span>
<span data-ttu-id="1f43d-128">В теле запроса поставляем представление JSON для [объекта deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

<span data-ttu-id="1f43d-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md).</span></span>

|<span data-ttu-id="1f43d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f43d-130">Property</span></span>|<span data-ttu-id="1f43d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1f43d-131">Type</span></span>|<span data-ttu-id="1f43d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1f43d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f43d-133">применимость</span><span class="sxs-lookup"><span data-stu-id="1f43d-133">applicability</span></span>|[<span data-ttu-id="1f43d-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="1f43d-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="1f43d-135">Сведения о том, какие параметры устройства применимы к унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1f43d-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="1f43d-136">accessTypes</span></span>|[<span data-ttu-id="1f43d-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="1f43d-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="1f43d-138">Режим доступа к режиму чтения и записи параметров, унаследованных от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="1f43d-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="1f43d-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="1f43d-140">keywords</span><span class="sxs-lookup"><span data-stu-id="1f43d-140">keywords</span></span>|<span data-ttu-id="1f43d-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1f43d-141">String collection</span></span>|<span data-ttu-id="1f43d-142">Маркеры для поиска параметров на унаследованных от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1f43d-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="1f43d-143">infoUrls</span></span>|<span data-ttu-id="1f43d-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1f43d-144">String collection</span></span>|<span data-ttu-id="1f43d-145">Список ссылок, дополнительные сведения о параметре можно найти на сайте Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1f43d-146">возникновение</span><span class="sxs-lookup"><span data-stu-id="1f43d-146">occurrence</span></span>|[<span data-ttu-id="1f43d-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="1f43d-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="1f43d-148">Указывает, требуется ли параметр или не наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1f43d-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="1f43d-149">baseUri</span></span>|<span data-ttu-id="1f43d-150">String</span><span class="sxs-lookup"><span data-stu-id="1f43d-150">String</span></span>|<span data-ttu-id="1f43d-151">Базовый путь CSP, унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1f43d-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="1f43d-152">offsetUri</span></span>|<span data-ttu-id="1f43d-153">String</span><span class="sxs-lookup"><span data-stu-id="1f43d-153">String</span></span>|<span data-ttu-id="1f43d-154">Смещение пути CSP из базы, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1f43d-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="1f43d-155">rootDefinitionId</span></span>|<span data-ttu-id="1f43d-156">String</span><span class="sxs-lookup"><span data-stu-id="1f43d-156">String</span></span>|<span data-ttu-id="1f43d-157">Определение корневого параметра, если это параметр ребенка.</span><span class="sxs-lookup"><span data-stu-id="1f43d-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="1f43d-158">Унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1f43d-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="1f43d-159">categoryId</span></span>|<span data-ttu-id="1f43d-160">String</span><span class="sxs-lookup"><span data-stu-id="1f43d-160">String</span></span>|<span data-ttu-id="1f43d-161">Указывает группу области, в которой параметр настроен в указанном поставщике служб конфигурации (CSP), унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1f43d-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="1f43d-162">settingUsage</span></span>|[<span data-ttu-id="1f43d-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="1f43d-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="1f43d-164">Тип настройки, например конфигурация и соответствие требованиям, унаследованные от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="1f43d-165">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="1f43d-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="1f43d-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="1f43d-166">uxBehavior</span></span>|[<span data-ttu-id="1f43d-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="1f43d-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="1f43d-168">Настройка представления типа управления в UX, унаследованной от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="1f43d-169">Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="1f43d-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="1f43d-170">visibility</span><span class="sxs-lookup"><span data-stu-id="1f43d-170">visibility</span></span>|[<span data-ttu-id="1f43d-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="1f43d-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="1f43d-172">Настройка области видимости для UX, унаследованной от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="1f43d-173">Возможные значения: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="1f43d-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="1f43d-174">referredSettingInformationList</span><span class="sxs-lookup"><span data-stu-id="1f43d-174">referredSettingInformationList</span></span>|<span data-ttu-id="1f43d-175">[коллекция deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-175">[deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md) collection</span></span>|<span data-ttu-id="1f43d-176">Список переданных сведений о параметрах.</span><span class="sxs-lookup"><span data-stu-id="1f43d-176">List of referred setting information.</span></span> <span data-ttu-id="1f43d-177">Унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-177">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1f43d-178">id</span><span class="sxs-lookup"><span data-stu-id="1f43d-178">id</span></span>|<span data-ttu-id="1f43d-179">String</span><span class="sxs-lookup"><span data-stu-id="1f43d-179">String</span></span>|<span data-ttu-id="1f43d-180">Идентификатор элемента, унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-180">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1f43d-181">description</span><span class="sxs-lookup"><span data-stu-id="1f43d-181">description</span></span>|<span data-ttu-id="1f43d-182">String</span><span class="sxs-lookup"><span data-stu-id="1f43d-182">String</span></span>|<span data-ttu-id="1f43d-183">Описание элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-183">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1f43d-184">helpText</span><span class="sxs-lookup"><span data-stu-id="1f43d-184">helpText</span></span>|<span data-ttu-id="1f43d-185">String</span><span class="sxs-lookup"><span data-stu-id="1f43d-185">String</span></span>|<span data-ttu-id="1f43d-186">Справка текста элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-186">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1f43d-187">name</span><span class="sxs-lookup"><span data-stu-id="1f43d-187">name</span></span>|<span data-ttu-id="1f43d-188">String</span><span class="sxs-lookup"><span data-stu-id="1f43d-188">String</span></span>|<span data-ttu-id="1f43d-189">Имя элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-189">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1f43d-190">displayName</span><span class="sxs-lookup"><span data-stu-id="1f43d-190">displayName</span></span>|<span data-ttu-id="1f43d-191">String</span><span class="sxs-lookup"><span data-stu-id="1f43d-191">String</span></span>|<span data-ttu-id="1f43d-192">Отображение имени элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-192">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1f43d-193">version</span><span class="sxs-lookup"><span data-stu-id="1f43d-193">version</span></span>|<span data-ttu-id="1f43d-194">String</span><span class="sxs-lookup"><span data-stu-id="1f43d-194">String</span></span>|<span data-ttu-id="1f43d-195">Версия элемента, унаследована от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-195">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="1f43d-196">childIds</span><span class="sxs-lookup"><span data-stu-id="1f43d-196">childIds</span></span>|<span data-ttu-id="1f43d-197">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1f43d-197">String collection</span></span>|<span data-ttu-id="1f43d-198">Зависимые параметры ребенка для этой группы параметров</span><span class="sxs-lookup"><span data-stu-id="1f43d-198">Dependent child settings to this group of settings</span></span>|
|<span data-ttu-id="1f43d-199">dependentOn</span><span class="sxs-lookup"><span data-stu-id="1f43d-199">dependentOn</span></span>|<span data-ttu-id="1f43d-200">[коллекция deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-200">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="1f43d-201">Список зависимостей для группы параметров</span><span class="sxs-lookup"><span data-stu-id="1f43d-201">List of Dependencies for the setting group</span></span>|
|<span data-ttu-id="1f43d-202">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="1f43d-202">dependedOnBy</span></span>|<span data-ttu-id="1f43d-203">[коллекция deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="1f43d-203">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="1f43d-204">Список параметров ребенка, которые зависят от этого параметра</span><span class="sxs-lookup"><span data-stu-id="1f43d-204">List of child settings that depend on this setting</span></span>|



## <a name="response"></a><span data-ttu-id="1f43d-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f43d-205">Response</span></span>
<span data-ttu-id="1f43d-206">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1f43d-206">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f43d-207">Пример</span><span class="sxs-lookup"><span data-stu-id="1f43d-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f43d-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f43d-208">Request</span></span>
<span data-ttu-id="1f43d-209">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f43d-209">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1f43d-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f43d-210">Response</span></span>
<span data-ttu-id="1f43d-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f43d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




