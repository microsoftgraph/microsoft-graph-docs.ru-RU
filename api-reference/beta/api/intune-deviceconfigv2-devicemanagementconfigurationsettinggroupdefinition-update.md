---
title: Обновление Девицеманажементконфигуратионсеттингграупдефинитион
description: Обновление свойств объекта Девицеманажементконфигуратионсеттингграупдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3dc8951432f981c6f37183c0c780cf0982b79d33
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242487"
---
# <a name="update-devicemanagementconfigurationsettinggroupdefinition"></a><span data-ttu-id="5472a-103">Обновление Девицеманажементконфигуратионсеттингграупдефинитион</span><span class="sxs-lookup"><span data-stu-id="5472a-103">Update deviceManagementConfigurationSettingGroupDefinition</span></span>

<span data-ttu-id="5472a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5472a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5472a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5472a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5472a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5472a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5472a-107">Обновление свойств объекта [девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="5472a-107">Update the properties of a [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5472a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5472a-108">Prerequisites</span></span>
<span data-ttu-id="5472a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5472a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5472a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5472a-111">Permission type</span></span>|<span data-ttu-id="5472a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5472a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5472a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5472a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5472a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5472a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5472a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5472a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5472a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5472a-116">Not supported.</span></span>|
|<span data-ttu-id="5472a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5472a-117">Application</span></span>|<span data-ttu-id="5472a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5472a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5472a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5472a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="5472a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5472a-120">Request headers</span></span>
|<span data-ttu-id="5472a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5472a-121">Header</span></span>|<span data-ttu-id="5472a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5472a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5472a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5472a-123">Authorization</span></span>|<span data-ttu-id="5472a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5472a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5472a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5472a-125">Accept</span></span>|<span data-ttu-id="5472a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5472a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5472a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5472a-127">Request body</span></span>
<span data-ttu-id="5472a-128">В тексте запроса добавьте представление объекта [девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5472a-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

<span data-ttu-id="5472a-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5472a-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md).</span></span>

|<span data-ttu-id="5472a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5472a-130">Property</span></span>|<span data-ttu-id="5472a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5472a-131">Type</span></span>|<span data-ttu-id="5472a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5472a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5472a-133">применения</span><span class="sxs-lookup"><span data-stu-id="5472a-133">applicability</span></span>|[<span data-ttu-id="5472a-134">девицеманажементконфигуратионсеттингаппликабилити</span><span class="sxs-lookup"><span data-stu-id="5472a-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="5472a-135">Сведения о том, какие параметры устройства применяются в унаследованном от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5472a-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5472a-136">акцесстипес</span><span class="sxs-lookup"><span data-stu-id="5472a-136">accessTypes</span></span>|[<span data-ttu-id="5472a-137">девицеманажементконфигуратионсеттингакцесстипес</span><span class="sxs-lookup"><span data-stu-id="5472a-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="5472a-138">Режим доступа для чтения и записи параметра, унаследованного от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5472a-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="5472a-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="5472a-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="5472a-140">keywords</span><span class="sxs-lookup"><span data-stu-id="5472a-140">keywords</span></span>|<span data-ttu-id="5472a-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5472a-141">String collection</span></span>|<span data-ttu-id="5472a-142">Маркеры, для которых параметры поиска унаследованы от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5472a-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5472a-143">инфаурлс</span><span class="sxs-lookup"><span data-stu-id="5472a-143">infoUrls</span></span>|<span data-ttu-id="5472a-144">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5472a-144">String collection</span></span>|<span data-ttu-id="5472a-145">Список ссылок дополнительные сведения для параметра можно найти в разделе унаследовано от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5472a-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5472a-146">экземпляр</span><span class="sxs-lookup"><span data-stu-id="5472a-146">occurrence</span></span>|[<span data-ttu-id="5472a-147">девицеманажементконфигуратионсеттингоккурренце</span><span class="sxs-lookup"><span data-stu-id="5472a-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="5472a-148">Указывает, является ли параметр обязательным или не наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5472a-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5472a-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="5472a-149">baseUri</span></span>|<span data-ttu-id="5472a-150">String</span><span class="sxs-lookup"><span data-stu-id="5472a-150">String</span></span>|<span data-ttu-id="5472a-151">Базовый путь поставщика CSP наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5472a-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5472a-152">оффсетури</span><span class="sxs-lookup"><span data-stu-id="5472a-152">offsetUri</span></span>|<span data-ttu-id="5472a-153">String</span><span class="sxs-lookup"><span data-stu-id="5472a-153">String</span></span>|<span data-ttu-id="5472a-154">Путь к поставщику службы шифрования из базового наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5472a-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5472a-155">рутдефинитионид</span><span class="sxs-lookup"><span data-stu-id="5472a-155">rootDefinitionId</span></span>|<span data-ttu-id="5472a-156">String</span><span class="sxs-lookup"><span data-stu-id="5472a-156">String</span></span>|<span data-ttu-id="5472a-157">Определение корневого параметра, если параметр является дочерним.</span><span class="sxs-lookup"><span data-stu-id="5472a-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="5472a-158">Наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5472a-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5472a-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="5472a-159">categoryId</span></span>|<span data-ttu-id="5472a-160">String</span><span class="sxs-lookup"><span data-stu-id="5472a-160">String</span></span>|<span data-ttu-id="5472a-161">Указывает группу областей, в которой параметр настроен в указанном поставщике службы конфигурации (CSP), унаследованном от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5472a-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5472a-162">сеттингусаже</span><span class="sxs-lookup"><span data-stu-id="5472a-162">settingUsage</span></span>|[<span data-ttu-id="5472a-163">девицеманажементконфигуратионсеттингусаже</span><span class="sxs-lookup"><span data-stu-id="5472a-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="5472a-164">Тип параметра, например конфигурация и соответствие, наследуемые от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5472a-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="5472a-165">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="5472a-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="5472a-166">id</span><span class="sxs-lookup"><span data-stu-id="5472a-166">id</span></span>|<span data-ttu-id="5472a-167">String</span><span class="sxs-lookup"><span data-stu-id="5472a-167">String</span></span>|<span data-ttu-id="5472a-168">Идентификатор элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5472a-168">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5472a-169">description</span><span class="sxs-lookup"><span data-stu-id="5472a-169">description</span></span>|<span data-ttu-id="5472a-170">String</span><span class="sxs-lookup"><span data-stu-id="5472a-170">String</span></span>|<span data-ttu-id="5472a-171">Описание элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5472a-171">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5472a-172">helpText</span><span class="sxs-lookup"><span data-stu-id="5472a-172">helpText</span></span>|<span data-ttu-id="5472a-173">String</span><span class="sxs-lookup"><span data-stu-id="5472a-173">String</span></span>|<span data-ttu-id="5472a-174">Текст справки элемента, наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5472a-174">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5472a-175">name</span><span class="sxs-lookup"><span data-stu-id="5472a-175">name</span></span>|<span data-ttu-id="5472a-176">String</span><span class="sxs-lookup"><span data-stu-id="5472a-176">String</span></span>|<span data-ttu-id="5472a-177">Имя элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5472a-177">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5472a-178">displayName</span><span class="sxs-lookup"><span data-stu-id="5472a-178">displayName</span></span>|<span data-ttu-id="5472a-179">String</span><span class="sxs-lookup"><span data-stu-id="5472a-179">String</span></span>|<span data-ttu-id="5472a-180">Отображаемое имя элемента, наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5472a-180">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5472a-181">version</span><span class="sxs-lookup"><span data-stu-id="5472a-181">version</span></span>|<span data-ttu-id="5472a-182">String</span><span class="sxs-lookup"><span data-stu-id="5472a-182">String</span></span>|<span data-ttu-id="5472a-183">Версия элемента наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5472a-183">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="5472a-184">чилдидс</span><span class="sxs-lookup"><span data-stu-id="5472a-184">childIds</span></span>|<span data-ttu-id="5472a-185">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5472a-185">String collection</span></span>|<span data-ttu-id="5472a-186">Зависимые параметры дочерних элементов для этой группы параметров</span><span class="sxs-lookup"><span data-stu-id="5472a-186">Dependent child settings to this group of settings</span></span>|
|<span data-ttu-id="5472a-187">депендентон</span><span class="sxs-lookup"><span data-stu-id="5472a-187">dependentOn</span></span>|<span data-ttu-id="5472a-188">Коллекция [девицеманажементконфигуратиондепендентон](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="5472a-188">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="5472a-189">Список зависимостей для группы параметров</span><span class="sxs-lookup"><span data-stu-id="5472a-189">List of Dependencies for the setting group</span></span>|
|<span data-ttu-id="5472a-190">депендедонби</span><span class="sxs-lookup"><span data-stu-id="5472a-190">dependedOnBy</span></span>|<span data-ttu-id="5472a-191">Коллекция [девицеманажементконфигуратионсеттингдепендедонби](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="5472a-191">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="5472a-192">Список дочерних параметров, зависящих от этого параметра</span><span class="sxs-lookup"><span data-stu-id="5472a-192">List of child settings that depend on this setting</span></span>|



## <a name="response"></a><span data-ttu-id="5472a-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="5472a-193">Response</span></span>
<span data-ttu-id="5472a-194">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5472a-194">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5472a-195">Пример</span><span class="sxs-lookup"><span data-stu-id="5472a-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="5472a-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="5472a-196">Request</span></span>
<span data-ttu-id="5472a-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5472a-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 1448

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

### <a name="response"></a><span data-ttu-id="5472a-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="5472a-198">Response</span></span>
<span data-ttu-id="5472a-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5472a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1497

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




