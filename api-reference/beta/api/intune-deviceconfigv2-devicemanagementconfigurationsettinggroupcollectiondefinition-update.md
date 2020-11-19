---
title: Обновление Девицеманажементконфигуратионсеттингграупколлектиондефинитион
description: Обновление свойств объекта Девицеманажементконфигуратионсеттингграупколлектиондефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5df45ef61eeee8e547c75491e21593e639fc3662
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242530"
---
# <a name="update-devicemanagementconfigurationsettinggroupcollectiondefinition"></a><span data-ttu-id="96dd0-103">Обновление Девицеманажементконфигуратионсеттингграупколлектиондефинитион</span><span class="sxs-lookup"><span data-stu-id="96dd0-103">Update deviceManagementConfigurationSettingGroupCollectionDefinition</span></span>

<span data-ttu-id="96dd0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96dd0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96dd0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96dd0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96dd0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="96dd0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96dd0-107">Обновление свойств объекта [девицеманажементконфигуратионсеттингграупколлектиондефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="96dd0-107">Update the properties of a [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96dd0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="96dd0-108">Prerequisites</span></span>
<span data-ttu-id="96dd0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96dd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96dd0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96dd0-111">Permission type</span></span>|<span data-ttu-id="96dd0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="96dd0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96dd0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96dd0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96dd0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96dd0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="96dd0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96dd0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96dd0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96dd0-116">Not supported.</span></span>|
|<span data-ttu-id="96dd0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="96dd0-117">Application</span></span>|<span data-ttu-id="96dd0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96dd0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96dd0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96dd0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="96dd0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="96dd0-120">Request headers</span></span>
|<span data-ttu-id="96dd0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="96dd0-121">Header</span></span>|<span data-ttu-id="96dd0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="96dd0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96dd0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96dd0-123">Authorization</span></span>|<span data-ttu-id="96dd0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96dd0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96dd0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="96dd0-125">Accept</span></span>|<span data-ttu-id="96dd0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96dd0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96dd0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96dd0-127">Request body</span></span>
<span data-ttu-id="96dd0-128">В тексте запроса добавьте представление объекта [девицеманажементконфигуратионсеттингграупколлектиондефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96dd0-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object.</span></span>

<span data-ttu-id="96dd0-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементконфигуратионсеттингграупколлектиондефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md).</span><span class="sxs-lookup"><span data-stu-id="96dd0-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md).</span></span>

|<span data-ttu-id="96dd0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="96dd0-130">Property</span></span>|<span data-ttu-id="96dd0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="96dd0-131">Type</span></span>|<span data-ttu-id="96dd0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="96dd0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96dd0-133">применения</span><span class="sxs-lookup"><span data-stu-id="96dd0-133">applicability</span></span>|[<span data-ttu-id="96dd0-134">девицеманажементконфигуратионсеттингаппликабилити</span><span class="sxs-lookup"><span data-stu-id="96dd0-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="96dd0-135">Сведения о том, какие параметры устройства применяются в унаследованном от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="96dd0-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="96dd0-136">акцесстипес</span><span class="sxs-lookup"><span data-stu-id="96dd0-136">accessTypes</span></span>|[<span data-ttu-id="96dd0-137">девицеманажементконфигуратионсеттингакцесстипес</span><span class="sxs-lookup"><span data-stu-id="96dd0-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="96dd0-138">Режим доступа для чтения и записи параметра, унаследованного от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="96dd0-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="96dd0-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="96dd0-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="96dd0-140">keywords</span><span class="sxs-lookup"><span data-stu-id="96dd0-140">keywords</span></span>|<span data-ttu-id="96dd0-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="96dd0-141">String collection</span></span>|<span data-ttu-id="96dd0-142">Маркеры, для которых параметры поиска унаследованы от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="96dd0-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="96dd0-143">инфаурлс</span><span class="sxs-lookup"><span data-stu-id="96dd0-143">infoUrls</span></span>|<span data-ttu-id="96dd0-144">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="96dd0-144">String collection</span></span>|<span data-ttu-id="96dd0-145">Список ссылок дополнительные сведения для параметра можно найти в разделе унаследовано от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="96dd0-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="96dd0-146">экземпляр</span><span class="sxs-lookup"><span data-stu-id="96dd0-146">occurrence</span></span>|[<span data-ttu-id="96dd0-147">девицеманажементконфигуратионсеттингоккурренце</span><span class="sxs-lookup"><span data-stu-id="96dd0-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="96dd0-148">Указывает, является ли параметр обязательным или не наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="96dd0-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="96dd0-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="96dd0-149">baseUri</span></span>|<span data-ttu-id="96dd0-150">String</span><span class="sxs-lookup"><span data-stu-id="96dd0-150">String</span></span>|<span data-ttu-id="96dd0-151">Базовый путь поставщика CSP наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="96dd0-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="96dd0-152">оффсетури</span><span class="sxs-lookup"><span data-stu-id="96dd0-152">offsetUri</span></span>|<span data-ttu-id="96dd0-153">String</span><span class="sxs-lookup"><span data-stu-id="96dd0-153">String</span></span>|<span data-ttu-id="96dd0-154">Путь к поставщику службы шифрования из базового наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="96dd0-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="96dd0-155">рутдефинитионид</span><span class="sxs-lookup"><span data-stu-id="96dd0-155">rootDefinitionId</span></span>|<span data-ttu-id="96dd0-156">String</span><span class="sxs-lookup"><span data-stu-id="96dd0-156">String</span></span>|<span data-ttu-id="96dd0-157">Определение корневого параметра, если параметр является дочерним.</span><span class="sxs-lookup"><span data-stu-id="96dd0-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="96dd0-158">Наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="96dd0-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="96dd0-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="96dd0-159">categoryId</span></span>|<span data-ttu-id="96dd0-160">String</span><span class="sxs-lookup"><span data-stu-id="96dd0-160">String</span></span>|<span data-ttu-id="96dd0-161">Указывает группу областей, в которой параметр настроен в указанном поставщике службы конфигурации (CSP), унаследованном от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="96dd0-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="96dd0-162">сеттингусаже</span><span class="sxs-lookup"><span data-stu-id="96dd0-162">settingUsage</span></span>|[<span data-ttu-id="96dd0-163">девицеманажементконфигуратионсеттингусаже</span><span class="sxs-lookup"><span data-stu-id="96dd0-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="96dd0-164">Тип параметра, например конфигурация и соответствие, наследуемые от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="96dd0-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="96dd0-165">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="96dd0-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="96dd0-166">id</span><span class="sxs-lookup"><span data-stu-id="96dd0-166">id</span></span>|<span data-ttu-id="96dd0-167">String</span><span class="sxs-lookup"><span data-stu-id="96dd0-167">String</span></span>|<span data-ttu-id="96dd0-168">Идентификатор элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="96dd0-168">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="96dd0-169">description</span><span class="sxs-lookup"><span data-stu-id="96dd0-169">description</span></span>|<span data-ttu-id="96dd0-170">String</span><span class="sxs-lookup"><span data-stu-id="96dd0-170">String</span></span>|<span data-ttu-id="96dd0-171">Описание элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="96dd0-171">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="96dd0-172">helpText</span><span class="sxs-lookup"><span data-stu-id="96dd0-172">helpText</span></span>|<span data-ttu-id="96dd0-173">String</span><span class="sxs-lookup"><span data-stu-id="96dd0-173">String</span></span>|<span data-ttu-id="96dd0-174">Текст справки элемента, наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="96dd0-174">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="96dd0-175">name</span><span class="sxs-lookup"><span data-stu-id="96dd0-175">name</span></span>|<span data-ttu-id="96dd0-176">String</span><span class="sxs-lookup"><span data-stu-id="96dd0-176">String</span></span>|<span data-ttu-id="96dd0-177">Имя элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="96dd0-177">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="96dd0-178">displayName</span><span class="sxs-lookup"><span data-stu-id="96dd0-178">displayName</span></span>|<span data-ttu-id="96dd0-179">String</span><span class="sxs-lookup"><span data-stu-id="96dd0-179">String</span></span>|<span data-ttu-id="96dd0-180">Отображаемое имя элемента, наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="96dd0-180">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="96dd0-181">version</span><span class="sxs-lookup"><span data-stu-id="96dd0-181">version</span></span>|<span data-ttu-id="96dd0-182">String</span><span class="sxs-lookup"><span data-stu-id="96dd0-182">String</span></span>|<span data-ttu-id="96dd0-183">Версия элемента наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="96dd0-183">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="96dd0-184">чилдидс</span><span class="sxs-lookup"><span data-stu-id="96dd0-184">childIds</span></span>|<span data-ttu-id="96dd0-185">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="96dd0-185">String collection</span></span>|<span data-ttu-id="96dd0-186">Зависимые параметры дочерних элементов для этой группы параметров, унаследованных от [девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="96dd0-186">Dependent child settings to this group of settings Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="96dd0-187">депендентон</span><span class="sxs-lookup"><span data-stu-id="96dd0-187">dependentOn</span></span>|<span data-ttu-id="96dd0-188">Коллекция [девицеманажементконфигуратиондепендентон](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="96dd0-188">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="96dd0-189">Список зависимостей для группы параметров, наследуемой от [девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="96dd0-189">List of Dependencies for the setting group Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="96dd0-190">депендедонби</span><span class="sxs-lookup"><span data-stu-id="96dd0-190">dependedOnBy</span></span>|<span data-ttu-id="96dd0-191">Коллекция [девицеманажементконфигуратионсеттингдепендедонби](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="96dd0-191">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="96dd0-192">Список дочерних параметров, зависящих от этого параметра, наследуемого от [девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="96dd0-192">List of child settings that depend on this setting Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="96dd0-193">максимумкаунт</span><span class="sxs-lookup"><span data-stu-id="96dd0-193">maximumCount</span></span>|<span data-ttu-id="96dd0-194">Int32</span><span class="sxs-lookup"><span data-stu-id="96dd0-194">Int32</span></span>|<span data-ttu-id="96dd0-195">Максимальное число параметров для параметра количество групп в коллекции.</span><span class="sxs-lookup"><span data-stu-id="96dd0-195">Maximum number of setting group count in the collection.</span></span> <span data-ttu-id="96dd0-196">Допустимые значения — от 1 до 100</span><span class="sxs-lookup"><span data-stu-id="96dd0-196">Valid values 1 to 100</span></span>|
|<span data-ttu-id="96dd0-197">минимумкаунт</span><span class="sxs-lookup"><span data-stu-id="96dd0-197">minimumCount</span></span>|<span data-ttu-id="96dd0-198">Int32</span><span class="sxs-lookup"><span data-stu-id="96dd0-198">Int32</span></span>|<span data-ttu-id="96dd0-199">Минимальное число параметров в коллекции.</span><span class="sxs-lookup"><span data-stu-id="96dd0-199">Minimum number of setting group count in the collection.</span></span> <span data-ttu-id="96dd0-200">Допустимые значения — от 1 до 100</span><span class="sxs-lookup"><span data-stu-id="96dd0-200">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="96dd0-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="96dd0-201">Response</span></span>
<span data-ttu-id="96dd0-202">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементконфигуратионсеттингграупколлектиондефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="96dd0-202">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96dd0-203">Пример</span><span class="sxs-lookup"><span data-stu-id="96dd0-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="96dd0-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="96dd0-204">Request</span></span>
<span data-ttu-id="96dd0-205">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96dd0-205">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 1504

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

### <a name="response"></a><span data-ttu-id="96dd0-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="96dd0-206">Response</span></span>
<span data-ttu-id="96dd0-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="96dd0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1553

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




