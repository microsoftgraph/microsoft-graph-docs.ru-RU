---
title: Создание Девицеманажементконфигуратиончоицесеттингколлектиондефинитион
description: Создание нового объекта Девицеманажементконфигуратиончоицесеттингколлектиондефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6dab7cfe23a5629f8fb7f18d4766e19cbeaa2dd6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242148"
---
# <a name="create-devicemanagementconfigurationchoicesettingcollectiondefinition"></a><span data-ttu-id="92ca2-103">Создание Девицеманажементконфигуратиончоицесеттингколлектиондефинитион</span><span class="sxs-lookup"><span data-stu-id="92ca2-103">Create deviceManagementConfigurationChoiceSettingCollectionDefinition</span></span>

<span data-ttu-id="92ca2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92ca2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92ca2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92ca2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92ca2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92ca2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92ca2-107">Создание нового объекта [девицеманажементконфигуратиончоицесеттингколлектиондефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="92ca2-107">Create a new [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92ca2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="92ca2-108">Prerequisites</span></span>
<span data-ttu-id="92ca2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92ca2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92ca2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92ca2-111">Permission type</span></span>|<span data-ttu-id="92ca2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="92ca2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92ca2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92ca2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92ca2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92ca2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="92ca2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92ca2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92ca2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92ca2-116">Not supported.</span></span>|
|<span data-ttu-id="92ca2-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="92ca2-117">Application</span></span>|<span data-ttu-id="92ca2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92ca2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92ca2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92ca2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="92ca2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="92ca2-120">Request headers</span></span>
|<span data-ttu-id="92ca2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92ca2-121">Header</span></span>|<span data-ttu-id="92ca2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="92ca2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92ca2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92ca2-123">Authorization</span></span>|<span data-ttu-id="92ca2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92ca2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92ca2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="92ca2-125">Accept</span></span>|<span data-ttu-id="92ca2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92ca2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92ca2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92ca2-127">Request body</span></span>
<span data-ttu-id="92ca2-128">В тексте запроса добавьте представление объекта Девицеманажементконфигуратиончоицесеттингколлектиондефинитион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92ca2-128">In the request body, supply a JSON representation for the deviceManagementConfigurationChoiceSettingCollectionDefinition object.</span></span>

<span data-ttu-id="92ca2-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементконфигуратиончоицесеттингколлектиондефинитион.</span><span class="sxs-lookup"><span data-stu-id="92ca2-129">The following table shows the properties that are required when you create the deviceManagementConfigurationChoiceSettingCollectionDefinition.</span></span>

|<span data-ttu-id="92ca2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="92ca2-130">Property</span></span>|<span data-ttu-id="92ca2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="92ca2-131">Type</span></span>|<span data-ttu-id="92ca2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="92ca2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92ca2-133">применения</span><span class="sxs-lookup"><span data-stu-id="92ca2-133">applicability</span></span>|[<span data-ttu-id="92ca2-134">девицеманажементконфигуратионсеттингаппликабилити</span><span class="sxs-lookup"><span data-stu-id="92ca2-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="92ca2-135">Сведения о том, какие параметры устройства применяются в унаследованном от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ca2-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ca2-136">акцесстипес</span><span class="sxs-lookup"><span data-stu-id="92ca2-136">accessTypes</span></span>|[<span data-ttu-id="92ca2-137">девицеманажементконфигуратионсеттингакцесстипес</span><span class="sxs-lookup"><span data-stu-id="92ca2-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="92ca2-138">Режим доступа для чтения и записи параметра, унаследованного от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="92ca2-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="92ca2-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="92ca2-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="92ca2-140">keywords</span><span class="sxs-lookup"><span data-stu-id="92ca2-140">keywords</span></span>|<span data-ttu-id="92ca2-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="92ca2-141">String collection</span></span>|<span data-ttu-id="92ca2-142">Маркеры, для которых параметры поиска унаследованы от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ca2-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ca2-143">инфаурлс</span><span class="sxs-lookup"><span data-stu-id="92ca2-143">infoUrls</span></span>|<span data-ttu-id="92ca2-144">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="92ca2-144">String collection</span></span>|<span data-ttu-id="92ca2-145">Список ссылок дополнительные сведения для параметра можно найти в разделе унаследовано от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ca2-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ca2-146">экземпляр</span><span class="sxs-lookup"><span data-stu-id="92ca2-146">occurrence</span></span>|[<span data-ttu-id="92ca2-147">девицеманажементконфигуратионсеттингоккурренце</span><span class="sxs-lookup"><span data-stu-id="92ca2-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="92ca2-148">Указывает, является ли параметр обязательным или не наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ca2-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ca2-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="92ca2-149">baseUri</span></span>|<span data-ttu-id="92ca2-150">String</span><span class="sxs-lookup"><span data-stu-id="92ca2-150">String</span></span>|<span data-ttu-id="92ca2-151">Базовый путь поставщика CSP наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ca2-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ca2-152">оффсетури</span><span class="sxs-lookup"><span data-stu-id="92ca2-152">offsetUri</span></span>|<span data-ttu-id="92ca2-153">String</span><span class="sxs-lookup"><span data-stu-id="92ca2-153">String</span></span>|<span data-ttu-id="92ca2-154">Путь к поставщику службы шифрования из базового наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ca2-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ca2-155">рутдефинитионид</span><span class="sxs-lookup"><span data-stu-id="92ca2-155">rootDefinitionId</span></span>|<span data-ttu-id="92ca2-156">String</span><span class="sxs-lookup"><span data-stu-id="92ca2-156">String</span></span>|<span data-ttu-id="92ca2-157">Определение корневого параметра, если параметр является дочерним.</span><span class="sxs-lookup"><span data-stu-id="92ca2-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="92ca2-158">Наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ca2-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ca2-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="92ca2-159">categoryId</span></span>|<span data-ttu-id="92ca2-160">String</span><span class="sxs-lookup"><span data-stu-id="92ca2-160">String</span></span>|<span data-ttu-id="92ca2-161">Указывает группу областей, в которой параметр настроен в указанном поставщике службы конфигурации (CSP), унаследованном от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ca2-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ca2-162">сеттингусаже</span><span class="sxs-lookup"><span data-stu-id="92ca2-162">settingUsage</span></span>|[<span data-ttu-id="92ca2-163">девицеманажементконфигуратионсеттингусаже</span><span class="sxs-lookup"><span data-stu-id="92ca2-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="92ca2-164">Тип параметра, например конфигурация и соответствие, наследуемые от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="92ca2-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="92ca2-165">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="92ca2-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="92ca2-166">id</span><span class="sxs-lookup"><span data-stu-id="92ca2-166">id</span></span>|<span data-ttu-id="92ca2-167">String</span><span class="sxs-lookup"><span data-stu-id="92ca2-167">String</span></span>|<span data-ttu-id="92ca2-168">Идентификатор элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ca2-168">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ca2-169">description</span><span class="sxs-lookup"><span data-stu-id="92ca2-169">description</span></span>|<span data-ttu-id="92ca2-170">String</span><span class="sxs-lookup"><span data-stu-id="92ca2-170">String</span></span>|<span data-ttu-id="92ca2-171">Описание элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ca2-171">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ca2-172">helpText</span><span class="sxs-lookup"><span data-stu-id="92ca2-172">helpText</span></span>|<span data-ttu-id="92ca2-173">String</span><span class="sxs-lookup"><span data-stu-id="92ca2-173">String</span></span>|<span data-ttu-id="92ca2-174">Текст справки элемента, наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ca2-174">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ca2-175">name</span><span class="sxs-lookup"><span data-stu-id="92ca2-175">name</span></span>|<span data-ttu-id="92ca2-176">String</span><span class="sxs-lookup"><span data-stu-id="92ca2-176">String</span></span>|<span data-ttu-id="92ca2-177">Имя элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ca2-177">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ca2-178">displayName</span><span class="sxs-lookup"><span data-stu-id="92ca2-178">displayName</span></span>|<span data-ttu-id="92ca2-179">String</span><span class="sxs-lookup"><span data-stu-id="92ca2-179">String</span></span>|<span data-ttu-id="92ca2-180">Отображаемое имя элемента, наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ca2-180">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ca2-181">version</span><span class="sxs-lookup"><span data-stu-id="92ca2-181">version</span></span>|<span data-ttu-id="92ca2-182">String</span><span class="sxs-lookup"><span data-stu-id="92ca2-182">String</span></span>|<span data-ttu-id="92ca2-183">Версия элемента наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ca2-183">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="92ca2-184">options</span><span class="sxs-lookup"><span data-stu-id="92ca2-184">options</span></span>|<span data-ttu-id="92ca2-185">Коллекция [девицеманажементконфигуратионоптиондефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ca2-185">[deviceManagementConfigurationOptionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinition.md) collection</span></span>|<span data-ttu-id="92ca2-186">Параметры, которые могут быть выбраны в качестве наследуемых от [девицеманажементконфигуратиончоицесеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ca2-186">Options for the setting that can be selected Inherited from [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span></span>|
|<span data-ttu-id="92ca2-187">дефаултоптионид</span><span class="sxs-lookup"><span data-stu-id="92ca2-187">defaultOptionId</span></span>|<span data-ttu-id="92ca2-188">String</span><span class="sxs-lookup"><span data-stu-id="92ca2-188">String</span></span>|<span data-ttu-id="92ca2-189">Параметр по умолчанию для параметра Choice, наследуемого из [девицеманажементконфигуратиончоицесеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="92ca2-189">Default option for choice setting Inherited from [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md)</span></span>|
|<span data-ttu-id="92ca2-190">максимумкаунт</span><span class="sxs-lookup"><span data-stu-id="92ca2-190">maximumCount</span></span>|<span data-ttu-id="92ca2-191">Int32</span><span class="sxs-lookup"><span data-stu-id="92ca2-191">Int32</span></span>|<span data-ttu-id="92ca2-192">Максимальное число вариантов выбора в коллекции.</span><span class="sxs-lookup"><span data-stu-id="92ca2-192">Maximum number of choices in the collection.</span></span> <span data-ttu-id="92ca2-193">Допустимые значения — от 1 до 100</span><span class="sxs-lookup"><span data-stu-id="92ca2-193">Valid values 1 to 100</span></span>|
|<span data-ttu-id="92ca2-194">минимумкаунт</span><span class="sxs-lookup"><span data-stu-id="92ca2-194">minimumCount</span></span>|<span data-ttu-id="92ca2-195">Int32</span><span class="sxs-lookup"><span data-stu-id="92ca2-195">Int32</span></span>|<span data-ttu-id="92ca2-196">Минимальное число вариантов в коллекции.</span><span class="sxs-lookup"><span data-stu-id="92ca2-196">Minimum number of choices in the collection.</span></span> <span data-ttu-id="92ca2-197">Допустимые значения — от 1 до 100</span><span class="sxs-lookup"><span data-stu-id="92ca2-197">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="92ca2-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="92ca2-198">Response</span></span>
<span data-ttu-id="92ca2-199">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементконфигуратиончоицесеттингколлектиондефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="92ca2-199">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationChoiceSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92ca2-200">Пример</span><span class="sxs-lookup"><span data-stu-id="92ca2-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="92ca2-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="92ca2-201">Request</span></span>
<span data-ttu-id="92ca2-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92ca2-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 9933

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingCollectionDefinition",
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
  "defaultOptionId": "Default Option Id value",
  "maximumCount": 12,
  "minimumCount": 12
}
```

### <a name="response"></a><span data-ttu-id="92ca2-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="92ca2-203">Response</span></span>
<span data-ttu-id="92ca2-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92ca2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 9982

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingCollectionDefinition",
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
  "id": "eb03fdca-fdca-eb03-cafd-03ebcafd03eb",
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
  "defaultOptionId": "Default Option Id value",
  "maximumCount": 12,
  "minimumCount": 12
}
```




