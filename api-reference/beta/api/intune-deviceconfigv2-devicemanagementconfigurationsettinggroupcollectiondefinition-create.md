---
title: Создание Девицеманажементконфигуратионсеттингграупколлектиондефинитион
description: Создание нового объекта Девицеманажементконфигуратионсеттингграупколлектиондефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 863a4e9573cf83afb1f2b91334cc771c0036c383
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242542"
---
# <a name="create-devicemanagementconfigurationsettinggroupcollectiondefinition"></a><span data-ttu-id="8d425-103">Создание Девицеманажементконфигуратионсеттингграупколлектиондефинитион</span><span class="sxs-lookup"><span data-stu-id="8d425-103">Create deviceManagementConfigurationSettingGroupCollectionDefinition</span></span>

<span data-ttu-id="8d425-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d425-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d425-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d425-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d425-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d425-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d425-107">Создание нового объекта [девицеманажементконфигуратионсеттингграупколлектиондефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="8d425-107">Create a new [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d425-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8d425-108">Prerequisites</span></span>
<span data-ttu-id="8d425-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d425-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d425-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d425-111">Permission type</span></span>|<span data-ttu-id="8d425-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d425-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d425-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d425-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d425-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d425-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d425-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d425-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d425-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d425-116">Not supported.</span></span>|
|<span data-ttu-id="8d425-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8d425-117">Application</span></span>|<span data-ttu-id="8d425-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d425-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d425-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d425-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="8d425-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8d425-120">Request headers</span></span>
|<span data-ttu-id="8d425-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d425-121">Header</span></span>|<span data-ttu-id="8d425-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8d425-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d425-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d425-123">Authorization</span></span>|<span data-ttu-id="8d425-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d425-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d425-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8d425-125">Accept</span></span>|<span data-ttu-id="8d425-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d425-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d425-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d425-127">Request body</span></span>
<span data-ttu-id="8d425-128">В тексте запроса добавьте представление объекта Девицеманажементконфигуратионсеттингграупколлектиондефинитион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d425-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingGroupCollectionDefinition object.</span></span>

<span data-ttu-id="8d425-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементконфигуратионсеттингграупколлектиондефинитион.</span><span class="sxs-lookup"><span data-stu-id="8d425-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingGroupCollectionDefinition.</span></span>

|<span data-ttu-id="8d425-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d425-130">Property</span></span>|<span data-ttu-id="8d425-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8d425-131">Type</span></span>|<span data-ttu-id="8d425-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8d425-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d425-133">применения</span><span class="sxs-lookup"><span data-stu-id="8d425-133">applicability</span></span>|[<span data-ttu-id="8d425-134">девицеманажементконфигуратионсеттингаппликабилити</span><span class="sxs-lookup"><span data-stu-id="8d425-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="8d425-135">Сведения о том, какие параметры устройства применяются в унаследованном от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8d425-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8d425-136">акцесстипес</span><span class="sxs-lookup"><span data-stu-id="8d425-136">accessTypes</span></span>|[<span data-ttu-id="8d425-137">девицеманажементконфигуратионсеттингакцесстипес</span><span class="sxs-lookup"><span data-stu-id="8d425-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="8d425-138">Режим доступа для чтения и записи параметра, унаследованного от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="8d425-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="8d425-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="8d425-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="8d425-140">keywords</span><span class="sxs-lookup"><span data-stu-id="8d425-140">keywords</span></span>|<span data-ttu-id="8d425-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8d425-141">String collection</span></span>|<span data-ttu-id="8d425-142">Маркеры, для которых параметры поиска унаследованы от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8d425-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8d425-143">инфаурлс</span><span class="sxs-lookup"><span data-stu-id="8d425-143">infoUrls</span></span>|<span data-ttu-id="8d425-144">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8d425-144">String collection</span></span>|<span data-ttu-id="8d425-145">Список ссылок дополнительные сведения для параметра можно найти в разделе унаследовано от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8d425-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8d425-146">экземпляр</span><span class="sxs-lookup"><span data-stu-id="8d425-146">occurrence</span></span>|[<span data-ttu-id="8d425-147">девицеманажементконфигуратионсеттингоккурренце</span><span class="sxs-lookup"><span data-stu-id="8d425-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="8d425-148">Указывает, является ли параметр обязательным или не наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8d425-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8d425-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="8d425-149">baseUri</span></span>|<span data-ttu-id="8d425-150">String</span><span class="sxs-lookup"><span data-stu-id="8d425-150">String</span></span>|<span data-ttu-id="8d425-151">Базовый путь поставщика CSP наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8d425-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8d425-152">оффсетури</span><span class="sxs-lookup"><span data-stu-id="8d425-152">offsetUri</span></span>|<span data-ttu-id="8d425-153">String</span><span class="sxs-lookup"><span data-stu-id="8d425-153">String</span></span>|<span data-ttu-id="8d425-154">Путь к поставщику службы шифрования из базового наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8d425-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8d425-155">рутдефинитионид</span><span class="sxs-lookup"><span data-stu-id="8d425-155">rootDefinitionId</span></span>|<span data-ttu-id="8d425-156">String</span><span class="sxs-lookup"><span data-stu-id="8d425-156">String</span></span>|<span data-ttu-id="8d425-157">Определение корневого параметра, если параметр является дочерним.</span><span class="sxs-lookup"><span data-stu-id="8d425-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="8d425-158">Наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8d425-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8d425-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="8d425-159">categoryId</span></span>|<span data-ttu-id="8d425-160">String</span><span class="sxs-lookup"><span data-stu-id="8d425-160">String</span></span>|<span data-ttu-id="8d425-161">Указывает группу областей, в которой параметр настроен в указанном поставщике службы конфигурации (CSP), унаследованном от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8d425-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8d425-162">сеттингусаже</span><span class="sxs-lookup"><span data-stu-id="8d425-162">settingUsage</span></span>|[<span data-ttu-id="8d425-163">девицеманажементконфигуратионсеттингусаже</span><span class="sxs-lookup"><span data-stu-id="8d425-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="8d425-164">Тип параметра, например конфигурация и соответствие, наследуемые от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="8d425-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="8d425-165">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="8d425-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="8d425-166">id</span><span class="sxs-lookup"><span data-stu-id="8d425-166">id</span></span>|<span data-ttu-id="8d425-167">String</span><span class="sxs-lookup"><span data-stu-id="8d425-167">String</span></span>|<span data-ttu-id="8d425-168">Идентификатор элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8d425-168">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8d425-169">description</span><span class="sxs-lookup"><span data-stu-id="8d425-169">description</span></span>|<span data-ttu-id="8d425-170">String</span><span class="sxs-lookup"><span data-stu-id="8d425-170">String</span></span>|<span data-ttu-id="8d425-171">Описание элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8d425-171">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8d425-172">helpText</span><span class="sxs-lookup"><span data-stu-id="8d425-172">helpText</span></span>|<span data-ttu-id="8d425-173">String</span><span class="sxs-lookup"><span data-stu-id="8d425-173">String</span></span>|<span data-ttu-id="8d425-174">Текст справки элемента, наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8d425-174">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8d425-175">name</span><span class="sxs-lookup"><span data-stu-id="8d425-175">name</span></span>|<span data-ttu-id="8d425-176">String</span><span class="sxs-lookup"><span data-stu-id="8d425-176">String</span></span>|<span data-ttu-id="8d425-177">Имя элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8d425-177">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8d425-178">displayName</span><span class="sxs-lookup"><span data-stu-id="8d425-178">displayName</span></span>|<span data-ttu-id="8d425-179">String</span><span class="sxs-lookup"><span data-stu-id="8d425-179">String</span></span>|<span data-ttu-id="8d425-180">Отображаемое имя элемента, наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8d425-180">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8d425-181">version</span><span class="sxs-lookup"><span data-stu-id="8d425-181">version</span></span>|<span data-ttu-id="8d425-182">String</span><span class="sxs-lookup"><span data-stu-id="8d425-182">String</span></span>|<span data-ttu-id="8d425-183">Версия элемента наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8d425-183">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8d425-184">чилдидс</span><span class="sxs-lookup"><span data-stu-id="8d425-184">childIds</span></span>|<span data-ttu-id="8d425-185">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8d425-185">String collection</span></span>|<span data-ttu-id="8d425-186">Зависимые параметры дочерних элементов для этой группы параметров, унаследованных от [девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8d425-186">Dependent child settings to this group of settings Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="8d425-187">депендентон</span><span class="sxs-lookup"><span data-stu-id="8d425-187">dependentOn</span></span>|<span data-ttu-id="8d425-188">Коллекция [девицеманажементконфигуратиондепендентон](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="8d425-188">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="8d425-189">Список зависимостей для группы параметров, наследуемой от [девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8d425-189">List of Dependencies for the setting group Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="8d425-190">депендедонби</span><span class="sxs-lookup"><span data-stu-id="8d425-190">dependedOnBy</span></span>|<span data-ttu-id="8d425-191">Коллекция [девицеманажементконфигуратионсеттингдепендедонби](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="8d425-191">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="8d425-192">Список дочерних параметров, зависящих от этого параметра, наследуемого от [девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8d425-192">List of child settings that depend on this setting Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="8d425-193">максимумкаунт</span><span class="sxs-lookup"><span data-stu-id="8d425-193">maximumCount</span></span>|<span data-ttu-id="8d425-194">Int32</span><span class="sxs-lookup"><span data-stu-id="8d425-194">Int32</span></span>|<span data-ttu-id="8d425-195">Максимальное число параметров для параметра количество групп в коллекции.</span><span class="sxs-lookup"><span data-stu-id="8d425-195">Maximum number of setting group count in the collection.</span></span> <span data-ttu-id="8d425-196">Допустимые значения — от 1 до 100</span><span class="sxs-lookup"><span data-stu-id="8d425-196">Valid values 1 to 100</span></span>|
|<span data-ttu-id="8d425-197">минимумкаунт</span><span class="sxs-lookup"><span data-stu-id="8d425-197">minimumCount</span></span>|<span data-ttu-id="8d425-198">Int32</span><span class="sxs-lookup"><span data-stu-id="8d425-198">Int32</span></span>|<span data-ttu-id="8d425-199">Минимальное число параметров в коллекции.</span><span class="sxs-lookup"><span data-stu-id="8d425-199">Minimum number of setting group count in the collection.</span></span> <span data-ttu-id="8d425-200">Допустимые значения — от 1 до 100</span><span class="sxs-lookup"><span data-stu-id="8d425-200">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="8d425-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d425-201">Response</span></span>
<span data-ttu-id="8d425-202">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементконфигуратионсеттингграупколлектиондефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8d425-202">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d425-203">Пример</span><span class="sxs-lookup"><span data-stu-id="8d425-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d425-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d425-204">Request</span></span>
<span data-ttu-id="8d425-205">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d425-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
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

### <a name="response"></a><span data-ttu-id="8d425-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d425-206">Response</span></span>
<span data-ttu-id="8d425-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d425-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




