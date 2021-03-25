---
title: Обновление deviceManagementConfigurationSettingGroupCollectionDefinition
description: Обновление свойств объекта deviceManagementConfigurationSettingGroupCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 74df3f91a0190429fdc618bf33793536c62dab0a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150845"
---
# <a name="update-devicemanagementconfigurationsettinggroupcollectiondefinition"></a><span data-ttu-id="8225c-103">Обновление deviceManagementConfigurationSettingGroupCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="8225c-103">Update deviceManagementConfigurationSettingGroupCollectionDefinition</span></span>

<span data-ttu-id="8225c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8225c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8225c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8225c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8225c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8225c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8225c-107">Обновление свойств объекта [deviceManagementConfigurationSettingGroupCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-107">Update the properties of a [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8225c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8225c-108">Prerequisites</span></span>
<span data-ttu-id="8225c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8225c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8225c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8225c-111">Permission type</span></span>|<span data-ttu-id="8225c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8225c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8225c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8225c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8225c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8225c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8225c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8225c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8225c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8225c-116">Not supported.</span></span>|
|<span data-ttu-id="8225c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8225c-117">Application</span></span>|<span data-ttu-id="8225c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8225c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8225c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8225c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="8225c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8225c-120">Request headers</span></span>
|<span data-ttu-id="8225c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8225c-121">Header</span></span>|<span data-ttu-id="8225c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8225c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8225c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8225c-123">Authorization</span></span>|<span data-ttu-id="8225c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8225c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8225c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8225c-125">Accept</span></span>|<span data-ttu-id="8225c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8225c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8225c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8225c-127">Request body</span></span>
<span data-ttu-id="8225c-128">В теле запроса поставляем представление JSON для [объекта deviceManagementConfigurationSettingGroupCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object.</span></span>

<span data-ttu-id="8225c-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementConfigurationSettingGroupCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md).</span></span>

|<span data-ttu-id="8225c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8225c-130">Property</span></span>|<span data-ttu-id="8225c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8225c-131">Type</span></span>|<span data-ttu-id="8225c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8225c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8225c-133">применимость</span><span class="sxs-lookup"><span data-stu-id="8225c-133">applicability</span></span>|[<span data-ttu-id="8225c-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="8225c-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="8225c-135">Сведения о том, какие параметры устройства применимы к унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8225c-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="8225c-136">accessTypes</span></span>|[<span data-ttu-id="8225c-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="8225c-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="8225c-138">Режим доступа к режиму чтения и записи параметров, унаследованных от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="8225c-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="8225c-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="8225c-140">keywords</span><span class="sxs-lookup"><span data-stu-id="8225c-140">keywords</span></span>|<span data-ttu-id="8225c-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8225c-141">String collection</span></span>|<span data-ttu-id="8225c-142">Маркеры для поиска параметров на унаследованных от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8225c-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="8225c-143">infoUrls</span></span>|<span data-ttu-id="8225c-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8225c-144">String collection</span></span>|<span data-ttu-id="8225c-145">Список ссылок, дополнительные сведения о параметре можно найти на сайте Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8225c-146">возникновение</span><span class="sxs-lookup"><span data-stu-id="8225c-146">occurrence</span></span>|[<span data-ttu-id="8225c-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="8225c-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="8225c-148">Указывает, требуется ли параметр или не наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8225c-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="8225c-149">baseUri</span></span>|<span data-ttu-id="8225c-150">Строка</span><span class="sxs-lookup"><span data-stu-id="8225c-150">String</span></span>|<span data-ttu-id="8225c-151">Базовый путь CSP, унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8225c-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="8225c-152">offsetUri</span></span>|<span data-ttu-id="8225c-153">Строка</span><span class="sxs-lookup"><span data-stu-id="8225c-153">String</span></span>|<span data-ttu-id="8225c-154">Смещение пути CSP из базы, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8225c-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8225c-155">rootDefinitionId</span></span>|<span data-ttu-id="8225c-156">Строка</span><span class="sxs-lookup"><span data-stu-id="8225c-156">String</span></span>|<span data-ttu-id="8225c-157">Определение корневого параметра, если это параметр ребенка.</span><span class="sxs-lookup"><span data-stu-id="8225c-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="8225c-158">Унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8225c-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="8225c-159">categoryId</span></span>|<span data-ttu-id="8225c-160">Строка</span><span class="sxs-lookup"><span data-stu-id="8225c-160">String</span></span>|<span data-ttu-id="8225c-161">Указывает группу области, в которой параметр настроен в указанном поставщике служб конфигурации (CSP), унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8225c-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="8225c-162">settingUsage</span></span>|[<span data-ttu-id="8225c-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="8225c-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="8225c-164">Тип настройки, например конфигурация и соответствие требованиям, унаследованные от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="8225c-165">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="8225c-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="8225c-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="8225c-166">uxBehavior</span></span>|[<span data-ttu-id="8225c-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="8225c-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="8225c-168">Настройка представления типа управления в UX, унаследованной от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="8225c-169">Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="8225c-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="8225c-170">visibility</span><span class="sxs-lookup"><span data-stu-id="8225c-170">visibility</span></span>|[<span data-ttu-id="8225c-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="8225c-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="8225c-172">Настройка области видимости для UX, унаследованной от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="8225c-173">Возможные значения: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="8225c-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="8225c-174">id</span><span class="sxs-lookup"><span data-stu-id="8225c-174">id</span></span>|<span data-ttu-id="8225c-175">Строка</span><span class="sxs-lookup"><span data-stu-id="8225c-175">String</span></span>|<span data-ttu-id="8225c-176">Идентификатор элемента, унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-176">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8225c-177">description</span><span class="sxs-lookup"><span data-stu-id="8225c-177">description</span></span>|<span data-ttu-id="8225c-178">Строка</span><span class="sxs-lookup"><span data-stu-id="8225c-178">String</span></span>|<span data-ttu-id="8225c-179">Описание элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-179">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8225c-180">helpText</span><span class="sxs-lookup"><span data-stu-id="8225c-180">helpText</span></span>|<span data-ttu-id="8225c-181">Строка</span><span class="sxs-lookup"><span data-stu-id="8225c-181">String</span></span>|<span data-ttu-id="8225c-182">Справка текста элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-182">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8225c-183">name</span><span class="sxs-lookup"><span data-stu-id="8225c-183">name</span></span>|<span data-ttu-id="8225c-184">String</span><span class="sxs-lookup"><span data-stu-id="8225c-184">String</span></span>|<span data-ttu-id="8225c-185">Имя элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-185">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8225c-186">displayName</span><span class="sxs-lookup"><span data-stu-id="8225c-186">displayName</span></span>|<span data-ttu-id="8225c-187">Строка</span><span class="sxs-lookup"><span data-stu-id="8225c-187">String</span></span>|<span data-ttu-id="8225c-188">Отображение имени элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-188">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8225c-189">version</span><span class="sxs-lookup"><span data-stu-id="8225c-189">version</span></span>|<span data-ttu-id="8225c-190">String</span><span class="sxs-lookup"><span data-stu-id="8225c-190">String</span></span>|<span data-ttu-id="8225c-191">Версия элемента, унаследована от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-191">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="8225c-192">childIds</span><span class="sxs-lookup"><span data-stu-id="8225c-192">childIds</span></span>|<span data-ttu-id="8225c-193">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8225c-193">String collection</span></span>|<span data-ttu-id="8225c-194">Зависимые параметры ребенка для этой группы параметров, унаследованных от [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-194">Dependent child settings to this group of settings Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="8225c-195">dependentOn</span><span class="sxs-lookup"><span data-stu-id="8225c-195">dependentOn</span></span>|<span data-ttu-id="8225c-196">[коллекция deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-196">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="8225c-197">Список зависимостей для группы параметров, унаследованных от [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-197">List of Dependencies for the setting group Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="8225c-198">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="8225c-198">dependedOnBy</span></span>|<span data-ttu-id="8225c-199">[коллекция deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-199">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="8225c-200">Список параметров ребенка, которые зависят от этого параметра, унаследованных от [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8225c-200">List of child settings that depend on this setting Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="8225c-201">maximumCount</span><span class="sxs-lookup"><span data-stu-id="8225c-201">maximumCount</span></span>|<span data-ttu-id="8225c-202">Int32</span><span class="sxs-lookup"><span data-stu-id="8225c-202">Int32</span></span>|<span data-ttu-id="8225c-203">Максимальное количество параметров количества групп в коллекции.</span><span class="sxs-lookup"><span data-stu-id="8225c-203">Maximum number of setting group count in the collection.</span></span> <span data-ttu-id="8225c-204">Допустимые значения от 1 до 100</span><span class="sxs-lookup"><span data-stu-id="8225c-204">Valid values 1 to 100</span></span>|
|<span data-ttu-id="8225c-205">minimumCount</span><span class="sxs-lookup"><span data-stu-id="8225c-205">minimumCount</span></span>|<span data-ttu-id="8225c-206">Int32</span><span class="sxs-lookup"><span data-stu-id="8225c-206">Int32</span></span>|<span data-ttu-id="8225c-207">Минимальное количество параметров группы в коллекции.</span><span class="sxs-lookup"><span data-stu-id="8225c-207">Minimum number of setting group count in the collection.</span></span> <span data-ttu-id="8225c-208">Допустимые значения от 1 до 100</span><span class="sxs-lookup"><span data-stu-id="8225c-208">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="8225c-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="8225c-209">Response</span></span>
<span data-ttu-id="8225c-210">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8225c-210">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8225c-211">Пример</span><span class="sxs-lookup"><span data-stu-id="8225c-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="8225c-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="8225c-212">Request</span></span>
<span data-ttu-id="8225c-213">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8225c-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 1569

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
  "visibility": "settingsCatalog",
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

### <a name="response"></a><span data-ttu-id="8225c-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="8225c-214">Response</span></span>
<span data-ttu-id="8225c-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8225c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1618

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
  "visibility": "settingsCatalog",
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




