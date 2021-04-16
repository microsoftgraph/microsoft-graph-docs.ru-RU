---
title: Создание deviceManagementConfigurationSettingGroupCollectionDefinition
description: Создание нового объекта deviceManagementConfigurationSettingGroupCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 666954c9428429cba8ffe4963ec53a8d8cfcbaeb
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864419"
---
# <a name="create-devicemanagementconfigurationsettinggroupcollectiondefinition"></a><span data-ttu-id="50525-103">Создание deviceManagementConfigurationSettingGroupCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="50525-103">Create deviceManagementConfigurationSettingGroupCollectionDefinition</span></span>

<span data-ttu-id="50525-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50525-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50525-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50525-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50525-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50525-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50525-107">Создание нового [объекта deviceManagementConfigurationSettingGroupCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-107">Create a new [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50525-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="50525-108">Prerequisites</span></span>
<span data-ttu-id="50525-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50525-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50525-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50525-111">Permission type</span></span>|<span data-ttu-id="50525-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50525-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50525-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50525-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50525-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50525-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50525-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50525-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50525-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50525-116">Not supported.</span></span>|
|<span data-ttu-id="50525-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="50525-117">Application</span></span>|<span data-ttu-id="50525-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50525-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50525-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50525-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reusableSettings
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="50525-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="50525-120">Request headers</span></span>
|<span data-ttu-id="50525-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50525-121">Header</span></span>|<span data-ttu-id="50525-122">Значение</span><span class="sxs-lookup"><span data-stu-id="50525-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50525-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50525-123">Authorization</span></span>|<span data-ttu-id="50525-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50525-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50525-125">Accept</span><span class="sxs-lookup"><span data-stu-id="50525-125">Accept</span></span>|<span data-ttu-id="50525-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50525-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50525-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50525-127">Request body</span></span>
<span data-ttu-id="50525-128">В теле запроса поставляем представление JSON для объекта deviceManagementConfigurationSettingGroupCollectionDefinition.</span><span class="sxs-lookup"><span data-stu-id="50525-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingGroupCollectionDefinition object.</span></span>

<span data-ttu-id="50525-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementConfigurationSettingGroupCollectionDefinition.</span><span class="sxs-lookup"><span data-stu-id="50525-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingGroupCollectionDefinition.</span></span>

|<span data-ttu-id="50525-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="50525-130">Property</span></span>|<span data-ttu-id="50525-131">Тип</span><span class="sxs-lookup"><span data-stu-id="50525-131">Type</span></span>|<span data-ttu-id="50525-132">Описание</span><span class="sxs-lookup"><span data-stu-id="50525-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50525-133">применимость</span><span class="sxs-lookup"><span data-stu-id="50525-133">applicability</span></span>|[<span data-ttu-id="50525-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="50525-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="50525-135">Сведения о том, какие параметры устройства применимы к унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="50525-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="50525-136">accessTypes</span></span>|[<span data-ttu-id="50525-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="50525-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="50525-138">Режим доступа к режиму чтения и записи параметров, унаследованных от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="50525-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="50525-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="50525-140">keywords</span><span class="sxs-lookup"><span data-stu-id="50525-140">keywords</span></span>|<span data-ttu-id="50525-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="50525-141">String collection</span></span>|<span data-ttu-id="50525-142">Маркеры для поиска параметров на унаследованных от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="50525-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="50525-143">infoUrls</span></span>|<span data-ttu-id="50525-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="50525-144">String collection</span></span>|<span data-ttu-id="50525-145">Список ссылок, дополнительные сведения о параметре можно найти на сайте Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="50525-146">возникновение</span><span class="sxs-lookup"><span data-stu-id="50525-146">occurrence</span></span>|[<span data-ttu-id="50525-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="50525-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="50525-148">Указывает, требуется ли параметр или не наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="50525-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="50525-149">baseUri</span></span>|<span data-ttu-id="50525-150">String</span><span class="sxs-lookup"><span data-stu-id="50525-150">String</span></span>|<span data-ttu-id="50525-151">Базовый путь CSP, унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="50525-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="50525-152">offsetUri</span></span>|<span data-ttu-id="50525-153">String</span><span class="sxs-lookup"><span data-stu-id="50525-153">String</span></span>|<span data-ttu-id="50525-154">Смещение пути CSP из базы, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="50525-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="50525-155">rootDefinitionId</span></span>|<span data-ttu-id="50525-156">String</span><span class="sxs-lookup"><span data-stu-id="50525-156">String</span></span>|<span data-ttu-id="50525-157">Определение корневого параметра, если это параметр ребенка.</span><span class="sxs-lookup"><span data-stu-id="50525-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="50525-158">Унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="50525-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="50525-159">categoryId</span></span>|<span data-ttu-id="50525-160">String</span><span class="sxs-lookup"><span data-stu-id="50525-160">String</span></span>|<span data-ttu-id="50525-161">Указывает группу области, в которой параметр настроен в указанном поставщике служб конфигурации (CSP), унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="50525-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="50525-162">settingUsage</span></span>|[<span data-ttu-id="50525-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="50525-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="50525-164">Тип настройки, например конфигурация и соответствие требованиям, унаследованные от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="50525-165">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="50525-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="50525-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="50525-166">uxBehavior</span></span>|[<span data-ttu-id="50525-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="50525-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="50525-168">Настройка представления типа управления в UX, унаследованной от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="50525-169">Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="50525-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="50525-170">visibility</span><span class="sxs-lookup"><span data-stu-id="50525-170">visibility</span></span>|[<span data-ttu-id="50525-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="50525-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="50525-172">Настройка области видимости для UX, унаследованной от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="50525-173">Возможные значения: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="50525-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="50525-174">referredSettingInformationList</span><span class="sxs-lookup"><span data-stu-id="50525-174">referredSettingInformationList</span></span>|<span data-ttu-id="50525-175">[коллекция deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md)</span><span class="sxs-lookup"><span data-stu-id="50525-175">[deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md) collection</span></span>|<span data-ttu-id="50525-176">Список переданных сведений о параметрах.</span><span class="sxs-lookup"><span data-stu-id="50525-176">List of referred setting information.</span></span> <span data-ttu-id="50525-177">Унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-177">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="50525-178">id</span><span class="sxs-lookup"><span data-stu-id="50525-178">id</span></span>|<span data-ttu-id="50525-179">String</span><span class="sxs-lookup"><span data-stu-id="50525-179">String</span></span>|<span data-ttu-id="50525-180">Идентификатор элемента, унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-180">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="50525-181">description</span><span class="sxs-lookup"><span data-stu-id="50525-181">description</span></span>|<span data-ttu-id="50525-182">String</span><span class="sxs-lookup"><span data-stu-id="50525-182">String</span></span>|<span data-ttu-id="50525-183">Описание элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-183">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="50525-184">helpText</span><span class="sxs-lookup"><span data-stu-id="50525-184">helpText</span></span>|<span data-ttu-id="50525-185">String</span><span class="sxs-lookup"><span data-stu-id="50525-185">String</span></span>|<span data-ttu-id="50525-186">Справка текста элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-186">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="50525-187">name</span><span class="sxs-lookup"><span data-stu-id="50525-187">name</span></span>|<span data-ttu-id="50525-188">String</span><span class="sxs-lookup"><span data-stu-id="50525-188">String</span></span>|<span data-ttu-id="50525-189">Имя элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-189">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="50525-190">displayName</span><span class="sxs-lookup"><span data-stu-id="50525-190">displayName</span></span>|<span data-ttu-id="50525-191">String</span><span class="sxs-lookup"><span data-stu-id="50525-191">String</span></span>|<span data-ttu-id="50525-192">Отображение имени элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-192">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="50525-193">version</span><span class="sxs-lookup"><span data-stu-id="50525-193">version</span></span>|<span data-ttu-id="50525-194">String</span><span class="sxs-lookup"><span data-stu-id="50525-194">String</span></span>|<span data-ttu-id="50525-195">Версия элемента, унаследована от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-195">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="50525-196">childIds</span><span class="sxs-lookup"><span data-stu-id="50525-196">childIds</span></span>|<span data-ttu-id="50525-197">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="50525-197">String collection</span></span>|<span data-ttu-id="50525-198">Зависимые параметры ребенка для этой группы параметров, унаследованных от [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-198">Dependent child settings to this group of settings Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="50525-199">dependentOn</span><span class="sxs-lookup"><span data-stu-id="50525-199">dependentOn</span></span>|<span data-ttu-id="50525-200">[коллекция deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="50525-200">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="50525-201">Список зависимостей для группы параметров, унаследованных от [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-201">List of Dependencies for the setting group Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="50525-202">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="50525-202">dependedOnBy</span></span>|<span data-ttu-id="50525-203">[коллекция deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="50525-203">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="50525-204">Список параметров ребенка, которые зависят от этого параметра, унаследованных от [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50525-204">List of child settings that depend on this setting Inherited from [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span></span>|
|<span data-ttu-id="50525-205">maximumCount</span><span class="sxs-lookup"><span data-stu-id="50525-205">maximumCount</span></span>|<span data-ttu-id="50525-206">Int32</span><span class="sxs-lookup"><span data-stu-id="50525-206">Int32</span></span>|<span data-ttu-id="50525-207">Максимальное количество параметров количества групп в коллекции.</span><span class="sxs-lookup"><span data-stu-id="50525-207">Maximum number of setting group count in the collection.</span></span> <span data-ttu-id="50525-208">Допустимые значения от 1 до 100</span><span class="sxs-lookup"><span data-stu-id="50525-208">Valid values 1 to 100</span></span>|
|<span data-ttu-id="50525-209">minimumCount</span><span class="sxs-lookup"><span data-stu-id="50525-209">minimumCount</span></span>|<span data-ttu-id="50525-210">Int32</span><span class="sxs-lookup"><span data-stu-id="50525-210">Int32</span></span>|<span data-ttu-id="50525-211">Минимальное количество параметров группы в коллекции.</span><span class="sxs-lookup"><span data-stu-id="50525-211">Minimum number of setting group count in the collection.</span></span> <span data-ttu-id="50525-212">Допустимые значения от 1 до 100</span><span class="sxs-lookup"><span data-stu-id="50525-212">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="50525-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="50525-213">Response</span></span>
<span data-ttu-id="50525-214">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="50525-214">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50525-215">Пример</span><span class="sxs-lookup"><span data-stu-id="50525-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="50525-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="50525-216">Request</span></span>
<span data-ttu-id="50525-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50525-217">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reusableSettings
Content-type: application/json
Content-length: 1785

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
  ],
  "maximumCount": 12,
  "minimumCount": 12
}
```

### <a name="response"></a><span data-ttu-id="50525-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="50525-218">Response</span></span>
<span data-ttu-id="50525-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50525-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1834

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
  "referredSettingInformationList": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
      "settingDefinitionId": "Setting Definition Id value"
    }
  ],
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




