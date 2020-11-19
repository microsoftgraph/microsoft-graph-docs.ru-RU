---
title: Обновление Девицеманажементконфигуратиончоицесеттингдефинитион
description: Обновление свойств объекта Девицеманажементконфигуратиончоицесеттингдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 69fac11d560de22f9537592edeed8bc63b01d44f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242319"
---
# <a name="update-devicemanagementconfigurationchoicesettingdefinition"></a><span data-ttu-id="b2f18-103">Обновление Девицеманажементконфигуратиончоицесеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="b2f18-103">Update deviceManagementConfigurationChoiceSettingDefinition</span></span>

<span data-ttu-id="b2f18-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2f18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2f18-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2f18-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2f18-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2f18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2f18-107">Обновление свойств объекта [девицеманажементконфигуратиончоицесеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="b2f18-107">Update the properties of a [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2f18-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b2f18-108">Prerequisites</span></span>
<span data-ttu-id="b2f18-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2f18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2f18-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2f18-111">Permission type</span></span>|<span data-ttu-id="b2f18-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2f18-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2f18-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2f18-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2f18-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2f18-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2f18-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2f18-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2f18-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2f18-116">Not supported.</span></span>|
|<span data-ttu-id="b2f18-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b2f18-117">Application</span></span>|<span data-ttu-id="b2f18-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2f18-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2f18-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2f18-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="b2f18-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b2f18-120">Request headers</span></span>
|<span data-ttu-id="b2f18-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2f18-121">Header</span></span>|<span data-ttu-id="b2f18-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b2f18-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2f18-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2f18-123">Authorization</span></span>|<span data-ttu-id="b2f18-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2f18-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2f18-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b2f18-125">Accept</span></span>|<span data-ttu-id="b2f18-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2f18-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2f18-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2f18-127">Request body</span></span>
<span data-ttu-id="b2f18-128">В тексте запроса добавьте представление объекта [девицеманажементконфигуратиончоицесеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2f18-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) object.</span></span>

<span data-ttu-id="b2f18-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементконфигуратиончоицесеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b2f18-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md).</span></span>

|<span data-ttu-id="b2f18-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2f18-130">Property</span></span>|<span data-ttu-id="b2f18-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b2f18-131">Type</span></span>|<span data-ttu-id="b2f18-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b2f18-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2f18-133">применения</span><span class="sxs-lookup"><span data-stu-id="b2f18-133">applicability</span></span>|[<span data-ttu-id="b2f18-134">девицеманажементконфигуратионсеттингаппликабилити</span><span class="sxs-lookup"><span data-stu-id="b2f18-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="b2f18-135">Сведения о том, какие параметры устройства применяются в унаследованном от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2f18-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b2f18-136">акцесстипес</span><span class="sxs-lookup"><span data-stu-id="b2f18-136">accessTypes</span></span>|[<span data-ttu-id="b2f18-137">девицеманажементконфигуратионсеттингакцесстипес</span><span class="sxs-lookup"><span data-stu-id="b2f18-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="b2f18-138">Режим доступа для чтения и записи параметра, унаследованного от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b2f18-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="b2f18-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="b2f18-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="b2f18-140">keywords</span><span class="sxs-lookup"><span data-stu-id="b2f18-140">keywords</span></span>|<span data-ttu-id="b2f18-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b2f18-141">String collection</span></span>|<span data-ttu-id="b2f18-142">Маркеры, для которых параметры поиска унаследованы от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2f18-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b2f18-143">инфаурлс</span><span class="sxs-lookup"><span data-stu-id="b2f18-143">infoUrls</span></span>|<span data-ttu-id="b2f18-144">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b2f18-144">String collection</span></span>|<span data-ttu-id="b2f18-145">Список ссылок дополнительные сведения для параметра можно найти в разделе унаследовано от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2f18-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b2f18-146">экземпляр</span><span class="sxs-lookup"><span data-stu-id="b2f18-146">occurrence</span></span>|[<span data-ttu-id="b2f18-147">девицеманажементконфигуратионсеттингоккурренце</span><span class="sxs-lookup"><span data-stu-id="b2f18-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="b2f18-148">Указывает, является ли параметр обязательным или не наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2f18-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b2f18-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="b2f18-149">baseUri</span></span>|<span data-ttu-id="b2f18-150">String</span><span class="sxs-lookup"><span data-stu-id="b2f18-150">String</span></span>|<span data-ttu-id="b2f18-151">Базовый путь поставщика CSP наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2f18-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b2f18-152">оффсетури</span><span class="sxs-lookup"><span data-stu-id="b2f18-152">offsetUri</span></span>|<span data-ttu-id="b2f18-153">String</span><span class="sxs-lookup"><span data-stu-id="b2f18-153">String</span></span>|<span data-ttu-id="b2f18-154">Путь к поставщику службы шифрования из базового наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2f18-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b2f18-155">рутдефинитионид</span><span class="sxs-lookup"><span data-stu-id="b2f18-155">rootDefinitionId</span></span>|<span data-ttu-id="b2f18-156">String</span><span class="sxs-lookup"><span data-stu-id="b2f18-156">String</span></span>|<span data-ttu-id="b2f18-157">Определение корневого параметра, если параметр является дочерним.</span><span class="sxs-lookup"><span data-stu-id="b2f18-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="b2f18-158">Наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2f18-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b2f18-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="b2f18-159">categoryId</span></span>|<span data-ttu-id="b2f18-160">String</span><span class="sxs-lookup"><span data-stu-id="b2f18-160">String</span></span>|<span data-ttu-id="b2f18-161">Указывает группу областей, в которой параметр настроен в указанном поставщике службы конфигурации (CSP), унаследованном от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2f18-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b2f18-162">сеттингусаже</span><span class="sxs-lookup"><span data-stu-id="b2f18-162">settingUsage</span></span>|[<span data-ttu-id="b2f18-163">девицеманажементконфигуратионсеттингусаже</span><span class="sxs-lookup"><span data-stu-id="b2f18-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="b2f18-164">Тип параметра, например конфигурация и соответствие, наследуемые от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b2f18-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="b2f18-165">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="b2f18-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="b2f18-166">id</span><span class="sxs-lookup"><span data-stu-id="b2f18-166">id</span></span>|<span data-ttu-id="b2f18-167">String</span><span class="sxs-lookup"><span data-stu-id="b2f18-167">String</span></span>|<span data-ttu-id="b2f18-168">Идентификатор элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2f18-168">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b2f18-169">description</span><span class="sxs-lookup"><span data-stu-id="b2f18-169">description</span></span>|<span data-ttu-id="b2f18-170">String</span><span class="sxs-lookup"><span data-stu-id="b2f18-170">String</span></span>|<span data-ttu-id="b2f18-171">Описание элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2f18-171">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b2f18-172">helpText</span><span class="sxs-lookup"><span data-stu-id="b2f18-172">helpText</span></span>|<span data-ttu-id="b2f18-173">String</span><span class="sxs-lookup"><span data-stu-id="b2f18-173">String</span></span>|<span data-ttu-id="b2f18-174">Текст справки элемента, наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2f18-174">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b2f18-175">name</span><span class="sxs-lookup"><span data-stu-id="b2f18-175">name</span></span>|<span data-ttu-id="b2f18-176">String</span><span class="sxs-lookup"><span data-stu-id="b2f18-176">String</span></span>|<span data-ttu-id="b2f18-177">Имя элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2f18-177">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b2f18-178">displayName</span><span class="sxs-lookup"><span data-stu-id="b2f18-178">displayName</span></span>|<span data-ttu-id="b2f18-179">String</span><span class="sxs-lookup"><span data-stu-id="b2f18-179">String</span></span>|<span data-ttu-id="b2f18-180">Отображаемое имя элемента, наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2f18-180">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b2f18-181">version</span><span class="sxs-lookup"><span data-stu-id="b2f18-181">version</span></span>|<span data-ttu-id="b2f18-182">String</span><span class="sxs-lookup"><span data-stu-id="b2f18-182">String</span></span>|<span data-ttu-id="b2f18-183">Версия элемента наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2f18-183">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="b2f18-184">options</span><span class="sxs-lookup"><span data-stu-id="b2f18-184">options</span></span>|<span data-ttu-id="b2f18-185">Коллекция [девицеманажементконфигуратионоптиондефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b2f18-185">[deviceManagementConfigurationOptionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinition.md) collection</span></span>|<span data-ttu-id="b2f18-186">Параметры для параметра, который можно выбрать</span><span class="sxs-lookup"><span data-stu-id="b2f18-186">Options for the setting that can be selected</span></span>|
|<span data-ttu-id="b2f18-187">дефаултоптионид</span><span class="sxs-lookup"><span data-stu-id="b2f18-187">defaultOptionId</span></span>|<span data-ttu-id="b2f18-188">String</span><span class="sxs-lookup"><span data-stu-id="b2f18-188">String</span></span>|<span data-ttu-id="b2f18-189">Вариант по умолчанию для параметра Choice</span><span class="sxs-lookup"><span data-stu-id="b2f18-189">Default option for choice setting</span></span>|



## <a name="response"></a><span data-ttu-id="b2f18-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2f18-190">Response</span></span>
<span data-ttu-id="b2f18-191">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементконфигуратиончоицесеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b2f18-191">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2f18-192">Пример</span><span class="sxs-lookup"><span data-stu-id="b2f18-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2f18-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2f18-193">Request</span></span>
<span data-ttu-id="b2f18-194">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2f18-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 9877

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

### <a name="response"></a><span data-ttu-id="b2f18-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2f18-195">Response</span></span>
<span data-ttu-id="b2f18-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b2f18-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9926

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




