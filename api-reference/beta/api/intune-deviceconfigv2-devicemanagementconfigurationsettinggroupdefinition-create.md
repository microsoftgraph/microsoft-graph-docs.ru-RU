---
title: Создание Девицеманажементконфигуратионсеттингграупдефинитион
description: Создание нового объекта Девицеманажементконфигуратионсеттингграупдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7c59ab6bd5a2aca7b4f6b11a2ad07ebe78ba766d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242505"
---
# <a name="create-devicemanagementconfigurationsettinggroupdefinition"></a><span data-ttu-id="fa3aa-103">Создание Девицеманажементконфигуратионсеттингграупдефинитион</span><span class="sxs-lookup"><span data-stu-id="fa3aa-103">Create deviceManagementConfigurationSettingGroupDefinition</span></span>

<span data-ttu-id="fa3aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa3aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa3aa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa3aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa3aa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa3aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa3aa-107">Создание нового объекта [девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="fa3aa-107">Create a new [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa3aa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fa3aa-108">Prerequisites</span></span>
<span data-ttu-id="fa3aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa3aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa3aa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa3aa-111">Permission type</span></span>|<span data-ttu-id="fa3aa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa3aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa3aa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa3aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fa3aa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa3aa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fa3aa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa3aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa3aa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa3aa-116">Not supported.</span></span>|
|<span data-ttu-id="fa3aa-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fa3aa-117">Application</span></span>|<span data-ttu-id="fa3aa-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa3aa-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa3aa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa3aa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="fa3aa-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fa3aa-120">Request headers</span></span>
|<span data-ttu-id="fa3aa-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa3aa-121">Header</span></span>|<span data-ttu-id="fa3aa-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fa3aa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa3aa-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa3aa-123">Authorization</span></span>|<span data-ttu-id="fa3aa-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa3aa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa3aa-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fa3aa-125">Accept</span></span>|<span data-ttu-id="fa3aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa3aa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa3aa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa3aa-127">Request body</span></span>
<span data-ttu-id="fa3aa-128">В тексте запроса добавьте представление объекта Девицеманажементконфигуратионсеттингграупдефинитион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa3aa-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingGroupDefinition object.</span></span>

<span data-ttu-id="fa3aa-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементконфигуратионсеттингграупдефинитион.</span><span class="sxs-lookup"><span data-stu-id="fa3aa-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingGroupDefinition.</span></span>

|<span data-ttu-id="fa3aa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa3aa-130">Property</span></span>|<span data-ttu-id="fa3aa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fa3aa-131">Type</span></span>|<span data-ttu-id="fa3aa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fa3aa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa3aa-133">применения</span><span class="sxs-lookup"><span data-stu-id="fa3aa-133">applicability</span></span>|[<span data-ttu-id="fa3aa-134">девицеманажементконфигуратионсеттингаппликабилити</span><span class="sxs-lookup"><span data-stu-id="fa3aa-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="fa3aa-135">Сведения о том, какие параметры устройства применяются в унаследованном от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fa3aa-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="fa3aa-136">акцесстипес</span><span class="sxs-lookup"><span data-stu-id="fa3aa-136">accessTypes</span></span>|[<span data-ttu-id="fa3aa-137">девицеманажементконфигуратионсеттингакцесстипес</span><span class="sxs-lookup"><span data-stu-id="fa3aa-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="fa3aa-138">Режим доступа для чтения и записи параметра, унаследованного от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="fa3aa-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="fa3aa-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="fa3aa-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="fa3aa-140">keywords</span><span class="sxs-lookup"><span data-stu-id="fa3aa-140">keywords</span></span>|<span data-ttu-id="fa3aa-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fa3aa-141">String collection</span></span>|<span data-ttu-id="fa3aa-142">Маркеры, для которых параметры поиска унаследованы от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fa3aa-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="fa3aa-143">инфаурлс</span><span class="sxs-lookup"><span data-stu-id="fa3aa-143">infoUrls</span></span>|<span data-ttu-id="fa3aa-144">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fa3aa-144">String collection</span></span>|<span data-ttu-id="fa3aa-145">Список ссылок дополнительные сведения для параметра можно найти в разделе унаследовано от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fa3aa-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="fa3aa-146">экземпляр</span><span class="sxs-lookup"><span data-stu-id="fa3aa-146">occurrence</span></span>|[<span data-ttu-id="fa3aa-147">девицеманажементконфигуратионсеттингоккурренце</span><span class="sxs-lookup"><span data-stu-id="fa3aa-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="fa3aa-148">Указывает, является ли параметр обязательным или не наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fa3aa-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="fa3aa-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="fa3aa-149">baseUri</span></span>|<span data-ttu-id="fa3aa-150">String</span><span class="sxs-lookup"><span data-stu-id="fa3aa-150">String</span></span>|<span data-ttu-id="fa3aa-151">Базовый путь поставщика CSP наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fa3aa-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="fa3aa-152">оффсетури</span><span class="sxs-lookup"><span data-stu-id="fa3aa-152">offsetUri</span></span>|<span data-ttu-id="fa3aa-153">String</span><span class="sxs-lookup"><span data-stu-id="fa3aa-153">String</span></span>|<span data-ttu-id="fa3aa-154">Путь к поставщику службы шифрования из базового наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fa3aa-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="fa3aa-155">рутдефинитионид</span><span class="sxs-lookup"><span data-stu-id="fa3aa-155">rootDefinitionId</span></span>|<span data-ttu-id="fa3aa-156">String</span><span class="sxs-lookup"><span data-stu-id="fa3aa-156">String</span></span>|<span data-ttu-id="fa3aa-157">Определение корневого параметра, если параметр является дочерним.</span><span class="sxs-lookup"><span data-stu-id="fa3aa-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="fa3aa-158">Наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fa3aa-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="fa3aa-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="fa3aa-159">categoryId</span></span>|<span data-ttu-id="fa3aa-160">String</span><span class="sxs-lookup"><span data-stu-id="fa3aa-160">String</span></span>|<span data-ttu-id="fa3aa-161">Указывает группу областей, в которой параметр настроен в указанном поставщике службы конфигурации (CSP), унаследованном от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fa3aa-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="fa3aa-162">сеттингусаже</span><span class="sxs-lookup"><span data-stu-id="fa3aa-162">settingUsage</span></span>|[<span data-ttu-id="fa3aa-163">девицеманажементконфигуратионсеттингусаже</span><span class="sxs-lookup"><span data-stu-id="fa3aa-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="fa3aa-164">Тип параметра, например конфигурация и соответствие, наследуемые от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="fa3aa-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="fa3aa-165">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="fa3aa-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="fa3aa-166">id</span><span class="sxs-lookup"><span data-stu-id="fa3aa-166">id</span></span>|<span data-ttu-id="fa3aa-167">String</span><span class="sxs-lookup"><span data-stu-id="fa3aa-167">String</span></span>|<span data-ttu-id="fa3aa-168">Идентификатор элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fa3aa-168">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="fa3aa-169">description</span><span class="sxs-lookup"><span data-stu-id="fa3aa-169">description</span></span>|<span data-ttu-id="fa3aa-170">String</span><span class="sxs-lookup"><span data-stu-id="fa3aa-170">String</span></span>|<span data-ttu-id="fa3aa-171">Описание элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fa3aa-171">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="fa3aa-172">helpText</span><span class="sxs-lookup"><span data-stu-id="fa3aa-172">helpText</span></span>|<span data-ttu-id="fa3aa-173">String</span><span class="sxs-lookup"><span data-stu-id="fa3aa-173">String</span></span>|<span data-ttu-id="fa3aa-174">Текст справки элемента, наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fa3aa-174">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="fa3aa-175">name</span><span class="sxs-lookup"><span data-stu-id="fa3aa-175">name</span></span>|<span data-ttu-id="fa3aa-176">String</span><span class="sxs-lookup"><span data-stu-id="fa3aa-176">String</span></span>|<span data-ttu-id="fa3aa-177">Имя элемента, наследуемого из [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fa3aa-177">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="fa3aa-178">displayName</span><span class="sxs-lookup"><span data-stu-id="fa3aa-178">displayName</span></span>|<span data-ttu-id="fa3aa-179">String</span><span class="sxs-lookup"><span data-stu-id="fa3aa-179">String</span></span>|<span data-ttu-id="fa3aa-180">Отображаемое имя элемента, наследуемого от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fa3aa-180">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="fa3aa-181">version</span><span class="sxs-lookup"><span data-stu-id="fa3aa-181">version</span></span>|<span data-ttu-id="fa3aa-182">String</span><span class="sxs-lookup"><span data-stu-id="fa3aa-182">String</span></span>|<span data-ttu-id="fa3aa-183">Версия элемента наследуется от [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fa3aa-183">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="fa3aa-184">чилдидс</span><span class="sxs-lookup"><span data-stu-id="fa3aa-184">childIds</span></span>|<span data-ttu-id="fa3aa-185">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fa3aa-185">String collection</span></span>|<span data-ttu-id="fa3aa-186">Зависимые параметры дочерних элементов для этой группы параметров</span><span class="sxs-lookup"><span data-stu-id="fa3aa-186">Dependent child settings to this group of settings</span></span>|
|<span data-ttu-id="fa3aa-187">депендентон</span><span class="sxs-lookup"><span data-stu-id="fa3aa-187">dependentOn</span></span>|<span data-ttu-id="fa3aa-188">Коллекция [девицеманажементконфигуратиондепендентон](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="fa3aa-188">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="fa3aa-189">Список зависимостей для группы параметров</span><span class="sxs-lookup"><span data-stu-id="fa3aa-189">List of Dependencies for the setting group</span></span>|
|<span data-ttu-id="fa3aa-190">депендедонби</span><span class="sxs-lookup"><span data-stu-id="fa3aa-190">dependedOnBy</span></span>|<span data-ttu-id="fa3aa-191">Коллекция [девицеманажементконфигуратионсеттингдепендедонби](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="fa3aa-191">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="fa3aa-192">Список дочерних параметров, зависящих от этого параметра</span><span class="sxs-lookup"><span data-stu-id="fa3aa-192">List of child settings that depend on this setting</span></span>|



## <a name="response"></a><span data-ttu-id="fa3aa-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa3aa-193">Response</span></span>
<span data-ttu-id="fa3aa-194">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa3aa-194">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa3aa-195">Пример</span><span class="sxs-lookup"><span data-stu-id="fa3aa-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa3aa-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa3aa-196">Request</span></span>
<span data-ttu-id="fa3aa-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa3aa-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
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

### <a name="response"></a><span data-ttu-id="fa3aa-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa3aa-198">Response</span></span>
<span data-ttu-id="fa3aa-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa3aa-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




