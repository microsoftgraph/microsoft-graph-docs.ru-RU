---
title: Создание deviceManagementConfigurationSimpleSettingCollectionDefinition
description: Создание нового объекта deviceManagementConfigurationSimpleSettingCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bfecd68d43105cf4e2a4d1a12ae8ca6d385e133e
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867940"
---
# <a name="create-devicemanagementconfigurationsimplesettingcollectiondefinition"></a><span data-ttu-id="28672-103">Создание deviceManagementConfigurationSimpleSettingCollectionDefinition</span><span class="sxs-lookup"><span data-stu-id="28672-103">Create deviceManagementConfigurationSimpleSettingCollectionDefinition</span></span>

<span data-ttu-id="28672-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28672-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28672-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28672-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28672-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28672-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28672-107">Создание нового [объекта deviceManagementConfigurationSimpleSettingCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-107">Create a new [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28672-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="28672-108">Prerequisites</span></span>
<span data-ttu-id="28672-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28672-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28672-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28672-111">Permission type</span></span>|<span data-ttu-id="28672-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28672-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28672-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28672-113">Delegated (work or school account)</span></span>|<span data-ttu-id="28672-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28672-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="28672-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28672-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28672-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28672-116">Not supported.</span></span>|
|<span data-ttu-id="28672-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="28672-117">Application</span></span>|<span data-ttu-id="28672-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28672-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28672-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28672-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reusableSettings
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="28672-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="28672-120">Request headers</span></span>
|<span data-ttu-id="28672-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28672-121">Header</span></span>|<span data-ttu-id="28672-122">Значение</span><span class="sxs-lookup"><span data-stu-id="28672-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28672-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28672-123">Authorization</span></span>|<span data-ttu-id="28672-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28672-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28672-125">Accept</span><span class="sxs-lookup"><span data-stu-id="28672-125">Accept</span></span>|<span data-ttu-id="28672-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28672-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28672-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28672-127">Request body</span></span>
<span data-ttu-id="28672-128">В теле запроса поставляем представление JSON для объекта deviceManagementConfigurationSimpleSettingCollectionDefinition.</span><span class="sxs-lookup"><span data-stu-id="28672-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSimpleSettingCollectionDefinition object.</span></span>

<span data-ttu-id="28672-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementConfigurationSimpleSettingCollectionDefinition.</span><span class="sxs-lookup"><span data-stu-id="28672-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSimpleSettingCollectionDefinition.</span></span>

|<span data-ttu-id="28672-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="28672-130">Property</span></span>|<span data-ttu-id="28672-131">Тип</span><span class="sxs-lookup"><span data-stu-id="28672-131">Type</span></span>|<span data-ttu-id="28672-132">Описание</span><span class="sxs-lookup"><span data-stu-id="28672-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28672-133">применимость</span><span class="sxs-lookup"><span data-stu-id="28672-133">applicability</span></span>|[<span data-ttu-id="28672-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="28672-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="28672-135">Сведения о том, какие параметры устройства применимы к унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-135">Details which device setting is applicable on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="28672-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="28672-136">accessTypes</span></span>|[<span data-ttu-id="28672-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="28672-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="28672-138">Режим доступа к режиму чтения и записи параметров, унаследованных от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-138">Read/write access mode of the setting Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="28672-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="28672-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="28672-140">keywords</span><span class="sxs-lookup"><span data-stu-id="28672-140">keywords</span></span>|<span data-ttu-id="28672-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="28672-141">String collection</span></span>|<span data-ttu-id="28672-142">Маркеры для поиска параметров на унаследованных от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-142">Tokens which to search settings on Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="28672-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="28672-143">infoUrls</span></span>|<span data-ttu-id="28672-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="28672-144">String collection</span></span>|<span data-ttu-id="28672-145">Список ссылок, дополнительные сведения о параметре можно найти на сайте Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-145">List of links more info for the setting can be found at Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="28672-146">возникновение</span><span class="sxs-lookup"><span data-stu-id="28672-146">occurrence</span></span>|[<span data-ttu-id="28672-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="28672-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="28672-148">Указывает, требуется ли параметр или не наследуется от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-148">Indicates whether the setting is required or not Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="28672-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="28672-149">baseUri</span></span>|<span data-ttu-id="28672-150">String</span><span class="sxs-lookup"><span data-stu-id="28672-150">String</span></span>|<span data-ttu-id="28672-151">Базовый путь CSP, унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-151">Base CSP Path Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="28672-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="28672-152">offsetUri</span></span>|<span data-ttu-id="28672-153">String</span><span class="sxs-lookup"><span data-stu-id="28672-153">String</span></span>|<span data-ttu-id="28672-154">Смещение пути CSP из базы, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-154">Offset CSP Path from Base Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="28672-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="28672-155">rootDefinitionId</span></span>|<span data-ttu-id="28672-156">String</span><span class="sxs-lookup"><span data-stu-id="28672-156">String</span></span>|<span data-ttu-id="28672-157">Определение корневого параметра, если это параметр ребенка.</span><span class="sxs-lookup"><span data-stu-id="28672-157">Root setting definition if the setting is a child setting.</span></span> <span data-ttu-id="28672-158">Унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-158">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="28672-159">categoryId</span><span class="sxs-lookup"><span data-stu-id="28672-159">categoryId</span></span>|<span data-ttu-id="28672-160">String</span><span class="sxs-lookup"><span data-stu-id="28672-160">String</span></span>|<span data-ttu-id="28672-161">Указывает группу области, в которой параметр настроен в указанном поставщике служб конфигурации (CSP), унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-161">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP) Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="28672-162">settingUsage</span><span class="sxs-lookup"><span data-stu-id="28672-162">settingUsage</span></span>|[<span data-ttu-id="28672-163">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="28672-163">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="28672-164">Тип настройки, например конфигурация и соответствие требованиям, унаследованные от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-164">Setting type, for example, configuration and compliance Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="28672-165">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="28672-165">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="28672-166">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="28672-166">uxBehavior</span></span>|[<span data-ttu-id="28672-167">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="28672-167">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="28672-168">Настройка представления типа управления в UX, унаследованной от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-168">Setting control type representation in the UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="28672-169">Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="28672-169">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="28672-170">visibility</span><span class="sxs-lookup"><span data-stu-id="28672-170">visibility</span></span>|[<span data-ttu-id="28672-171">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="28672-171">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="28672-172">Настройка области видимости для UX, унаследованной от [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-172">Setting visibility scope to UX Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span> <span data-ttu-id="28672-173">Возможные значения: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="28672-173">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="28672-174">referredSettingInformationList</span><span class="sxs-lookup"><span data-stu-id="28672-174">referredSettingInformationList</span></span>|<span data-ttu-id="28672-175">[коллекция deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md)</span><span class="sxs-lookup"><span data-stu-id="28672-175">[deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md) collection</span></span>|<span data-ttu-id="28672-176">Список переданных сведений о параметрах.</span><span class="sxs-lookup"><span data-stu-id="28672-176">List of referred setting information.</span></span> <span data-ttu-id="28672-177">Унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-177">Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="28672-178">id</span><span class="sxs-lookup"><span data-stu-id="28672-178">id</span></span>|<span data-ttu-id="28672-179">String</span><span class="sxs-lookup"><span data-stu-id="28672-179">String</span></span>|<span data-ttu-id="28672-180">Идентификатор элемента, унаследованный от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-180">Identifier for item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="28672-181">description</span><span class="sxs-lookup"><span data-stu-id="28672-181">description</span></span>|<span data-ttu-id="28672-182">String</span><span class="sxs-lookup"><span data-stu-id="28672-182">String</span></span>|<span data-ttu-id="28672-183">Описание элемента Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-183">Description of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="28672-184">helpText</span><span class="sxs-lookup"><span data-stu-id="28672-184">helpText</span></span>|<span data-ttu-id="28672-185">String</span><span class="sxs-lookup"><span data-stu-id="28672-185">String</span></span>|<span data-ttu-id="28672-186">Справка текста элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-186">Help text of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="28672-187">name</span><span class="sxs-lookup"><span data-stu-id="28672-187">name</span></span>|<span data-ttu-id="28672-188">String</span><span class="sxs-lookup"><span data-stu-id="28672-188">String</span></span>|<span data-ttu-id="28672-189">Имя элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-189">Name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="28672-190">displayName</span><span class="sxs-lookup"><span data-stu-id="28672-190">displayName</span></span>|<span data-ttu-id="28672-191">String</span><span class="sxs-lookup"><span data-stu-id="28672-191">String</span></span>|<span data-ttu-id="28672-192">Отображение имени элемента, унаследованной от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-192">Display name of the item Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="28672-193">version</span><span class="sxs-lookup"><span data-stu-id="28672-193">version</span></span>|<span data-ttu-id="28672-194">String</span><span class="sxs-lookup"><span data-stu-id="28672-194">String</span></span>|<span data-ttu-id="28672-195">Версия элемента, унаследована от [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-195">Item Version Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span></span>|
|<span data-ttu-id="28672-196">valueDefinition</span><span class="sxs-lookup"><span data-stu-id="28672-196">valueDefinition</span></span>|[<span data-ttu-id="28672-197">deviceManagementConfigurationSettingValueDefinition</span><span class="sxs-lookup"><span data-stu-id="28672-197">deviceManagementConfigurationSettingValueDefinition</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)|<span data-ttu-id="28672-198">Определение значения для этого параметра, унаследованной от [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-198">Definition of the value for this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="28672-199">defaultValue</span><span class="sxs-lookup"><span data-stu-id="28672-199">defaultValue</span></span>|[<span data-ttu-id="28672-200">deviceManagementConfigurationSettingValue</span><span class="sxs-lookup"><span data-stu-id="28672-200">deviceManagementConfigurationSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)|<span data-ttu-id="28672-201">Значение параметра по умолчанию для этого параметра, унаследованной от [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-201">Default setting value for this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="28672-202">dependentOn</span><span class="sxs-lookup"><span data-stu-id="28672-202">dependentOn</span></span>|<span data-ttu-id="28672-203">[коллекция deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md)</span><span class="sxs-lookup"><span data-stu-id="28672-203">[deviceManagementConfigurationDependentOn](../resources/intune-deviceconfigv2-devicemanagementconfigurationdependenton.md) collection</span></span>|<span data-ttu-id="28672-204">список родительских параметров, которые этот параметр зависит от унаследованных от [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-204">list of parent settings this setting is dependent on Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="28672-205">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="28672-205">dependedOnBy</span></span>|<span data-ttu-id="28672-206">[коллекция deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md)</span><span class="sxs-lookup"><span data-stu-id="28672-206">[deviceManagementConfigurationSettingDependedOnBy](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdependedonby.md) collection</span></span>|<span data-ttu-id="28672-207">список параметров ребенка, которые зависят от этого параметра, унаследованных от [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="28672-207">list of child settings that depend on this setting Inherited from [deviceManagementConfigurationSimpleSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingdefinition.md)</span></span>|
|<span data-ttu-id="28672-208">maximumCount</span><span class="sxs-lookup"><span data-stu-id="28672-208">maximumCount</span></span>|<span data-ttu-id="28672-209">Int32</span><span class="sxs-lookup"><span data-stu-id="28672-209">Int32</span></span>|<span data-ttu-id="28672-210">Максимальное количество простых параметров в коллекции.</span><span class="sxs-lookup"><span data-stu-id="28672-210">Maximum number of simple settings in the collection.</span></span> <span data-ttu-id="28672-211">Допустимые значения от 1 до 100</span><span class="sxs-lookup"><span data-stu-id="28672-211">Valid values 1 to 100</span></span>|
|<span data-ttu-id="28672-212">minimumCount</span><span class="sxs-lookup"><span data-stu-id="28672-212">minimumCount</span></span>|<span data-ttu-id="28672-213">Int32</span><span class="sxs-lookup"><span data-stu-id="28672-213">Int32</span></span>|<span data-ttu-id="28672-214">Минимальное количество простых параметров в коллекции.</span><span class="sxs-lookup"><span data-stu-id="28672-214">Minimum number of simple settings in the collection.</span></span> <span data-ttu-id="28672-215">Допустимые значения от 1 до 100</span><span class="sxs-lookup"><span data-stu-id="28672-215">Valid values 1 to 100</span></span>|



## <a name="response"></a><span data-ttu-id="28672-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="28672-216">Response</span></span>
<span data-ttu-id="28672-217">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="28672-217">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSimpleSettingCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingcollectiondefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28672-218">Пример</span><span class="sxs-lookup"><span data-stu-id="28672-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="28672-219">Запрос</span><span class="sxs-lookup"><span data-stu-id="28672-219">Request</span></span>
<span data-ttu-id="28672-220">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28672-220">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reusableSettings
Content-type: application/json
Content-length: 9464

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

### <a name="response"></a><span data-ttu-id="28672-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="28672-221">Response</span></span>
<span data-ttu-id="28672-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28672-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 9513

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
  "visibility": "settingsCatalog",
  "referredSettingInformationList": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
      "settingDefinitionId": "Setting Definition Id value"
    }
  ],
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




