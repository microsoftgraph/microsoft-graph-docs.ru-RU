---
title: Создание Девицеманажементконфигуратионсеттингдефинитион
description: Создание нового объекта Девицеманажементконфигуратионсеттингдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f16ae5a778df7d0398a137f86cda6dfcb3dbdb6d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242565"
---
# <a name="create-devicemanagementconfigurationsettingdefinition"></a><span data-ttu-id="8f25d-103">Создание Девицеманажементконфигуратионсеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="8f25d-103">Create deviceManagementConfigurationSettingDefinition</span></span>

<span data-ttu-id="8f25d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f25d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f25d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f25d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f25d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f25d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f25d-107">Создание нового объекта [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="8f25d-107">Create a new [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f25d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8f25d-108">Prerequisites</span></span>
<span data-ttu-id="8f25d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f25d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f25d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f25d-111">Permission type</span></span>|<span data-ttu-id="8f25d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f25d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f25d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f25d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8f25d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f25d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8f25d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f25d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f25d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f25d-116">Not supported.</span></span>|
|<span data-ttu-id="8f25d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8f25d-117">Application</span></span>|<span data-ttu-id="8f25d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f25d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f25d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f25d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="8f25d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8f25d-120">Request headers</span></span>
|<span data-ttu-id="8f25d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f25d-121">Header</span></span>|<span data-ttu-id="8f25d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8f25d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f25d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f25d-123">Authorization</span></span>|<span data-ttu-id="8f25d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f25d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f25d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8f25d-125">Accept</span></span>|<span data-ttu-id="8f25d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8f25d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f25d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f25d-127">Request body</span></span>
<span data-ttu-id="8f25d-128">В тексте запроса добавьте представление объекта Девицеманажементконфигуратионсеттингдефинитион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f25d-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingDefinition object.</span></span>

<span data-ttu-id="8f25d-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементконфигуратионсеттингдефинитион.</span><span class="sxs-lookup"><span data-stu-id="8f25d-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingDefinition.</span></span>

|<span data-ttu-id="8f25d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f25d-130">Property</span></span>|<span data-ttu-id="8f25d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8f25d-131">Type</span></span>|<span data-ttu-id="8f25d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8f25d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f25d-133">применения</span><span class="sxs-lookup"><span data-stu-id="8f25d-133">applicability</span></span>|[<span data-ttu-id="8f25d-134">девицеманажементконфигуратионсеттингаппликабилити</span><span class="sxs-lookup"><span data-stu-id="8f25d-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="8f25d-135">Сведения о том, какие параметры устройства применяются для</span><span class="sxs-lookup"><span data-stu-id="8f25d-135">Details which device setting is applicable on</span></span>|
|<span data-ttu-id="8f25d-136">акцесстипес</span><span class="sxs-lookup"><span data-stu-id="8f25d-136">accessTypes</span></span>|[<span data-ttu-id="8f25d-137">девицеманажементконфигуратионсеттингакцесстипес</span><span class="sxs-lookup"><span data-stu-id="8f25d-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="8f25d-138">Режим доступа для чтения и записи параметра.</span><span class="sxs-lookup"><span data-stu-id="8f25d-138">Read/write access mode of the setting.</span></span> <span data-ttu-id="8f25d-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="8f25d-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="8f25d-140">keywords</span><span class="sxs-lookup"><span data-stu-id="8f25d-140">keywords</span></span>|<span data-ttu-id="8f25d-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8f25d-141">String collection</span></span>|<span data-ttu-id="8f25d-142">Маркеры, для которых необходимо выполнить поиск параметров</span><span class="sxs-lookup"><span data-stu-id="8f25d-142">Tokens which to search settings on</span></span>|
|<span data-ttu-id="8f25d-143">инфаурлс</span><span class="sxs-lookup"><span data-stu-id="8f25d-143">infoUrls</span></span>|<span data-ttu-id="8f25d-144">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8f25d-144">String collection</span></span>|<span data-ttu-id="8f25d-145">Список ссылок дополнительные сведения для параметра можно найти по адресу</span><span class="sxs-lookup"><span data-stu-id="8f25d-145">List of links more info for the setting can be found at</span></span>|
|<span data-ttu-id="8f25d-146">экземпляр</span><span class="sxs-lookup"><span data-stu-id="8f25d-146">occurrence</span></span>|[<span data-ttu-id="8f25d-147">девицеманажементконфигуратионсеттингоккурренце</span><span class="sxs-lookup"><span data-stu-id="8f25d-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="8f25d-148">Указывает, является ли параметр обязательным или нет</span><span class="sxs-lookup"><span data-stu-id="8f25d-148">Indicates whether the setting is required or not</span></span>|
|<span data-ttu-id="8f25d-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="8f25d-149">baseUri</span></span>|<span data-ttu-id="8f25d-150">String</span><span class="sxs-lookup"><span data-stu-id="8f25d-150">String</span></span>|<span data-ttu-id="8f25d-151">Путь к основному поставщику служб шифрования</span><span class="sxs-lookup"><span data-stu-id="8f25d-151">Base CSP Path</span></span>|
|<span data-ttu-id="8f25d-152">оффсетури</span><span class="sxs-lookup"><span data-stu-id="8f25d-152">offsetUri</span></span>|<span data-ttu-id="8f25d-153">String</span><span class="sxs-lookup"><span data-stu-id="8f25d-153">String</span></span>|<span data-ttu-id="8f25d-154">Путь от базового поставщика CSP</span><span class="sxs-lookup"><span data-stu-id="8f25d-154">Offset CSP Path from Base</span></span>|
|<span data-ttu-id="8f25d-155">рутдефинитионид</span><span class="sxs-lookup"><span data-stu-id="8f25d-155">rootDefinitionId</span></span>|<span data-ttu-id="8f25d-156">String</span><span class="sxs-lookup"><span data-stu-id="8f25d-156">String</span></span>|<span data-ttu-id="8f25d-157">Определение корневого параметра, если параметр является дочерним.</span><span class="sxs-lookup"><span data-stu-id="8f25d-157">Root setting definition if the setting is a child setting.</span></span>|
|<span data-ttu-id="8f25d-158">categoryId</span><span class="sxs-lookup"><span data-stu-id="8f25d-158">categoryId</span></span>|<span data-ttu-id="8f25d-159">String</span><span class="sxs-lookup"><span data-stu-id="8f25d-159">String</span></span>|<span data-ttu-id="8f25d-160">Указывает группу областей, в которой параметр настроен в указанном поставщике службы конфигурации (CSP).</span><span class="sxs-lookup"><span data-stu-id="8f25d-160">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP)</span></span>|
|<span data-ttu-id="8f25d-161">сеттингусаже</span><span class="sxs-lookup"><span data-stu-id="8f25d-161">settingUsage</span></span>|[<span data-ttu-id="8f25d-162">девицеманажементконфигуратионсеттингусаже</span><span class="sxs-lookup"><span data-stu-id="8f25d-162">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="8f25d-163">Тип параметра, например, "Конфигурация" и "соответствие".</span><span class="sxs-lookup"><span data-stu-id="8f25d-163">Setting type, for example, configuration and compliance.</span></span> <span data-ttu-id="8f25d-164">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="8f25d-164">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="8f25d-165">id</span><span class="sxs-lookup"><span data-stu-id="8f25d-165">id</span></span>|<span data-ttu-id="8f25d-166">String</span><span class="sxs-lookup"><span data-stu-id="8f25d-166">String</span></span>|<span data-ttu-id="8f25d-167">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="8f25d-167">Identifier for item</span></span>|
|<span data-ttu-id="8f25d-168">description</span><span class="sxs-lookup"><span data-stu-id="8f25d-168">description</span></span>|<span data-ttu-id="8f25d-169">String</span><span class="sxs-lookup"><span data-stu-id="8f25d-169">String</span></span>|<span data-ttu-id="8f25d-170">Описание элемента</span><span class="sxs-lookup"><span data-stu-id="8f25d-170">Description of the item</span></span>|
|<span data-ttu-id="8f25d-171">helpText</span><span class="sxs-lookup"><span data-stu-id="8f25d-171">helpText</span></span>|<span data-ttu-id="8f25d-172">String</span><span class="sxs-lookup"><span data-stu-id="8f25d-172">String</span></span>|<span data-ttu-id="8f25d-173">Текст справки элемента</span><span class="sxs-lookup"><span data-stu-id="8f25d-173">Help text of the item</span></span>|
|<span data-ttu-id="8f25d-174">name</span><span class="sxs-lookup"><span data-stu-id="8f25d-174">name</span></span>|<span data-ttu-id="8f25d-175">String</span><span class="sxs-lookup"><span data-stu-id="8f25d-175">String</span></span>|<span data-ttu-id="8f25d-176">Имя элемента</span><span class="sxs-lookup"><span data-stu-id="8f25d-176">Name of the item</span></span>|
|<span data-ttu-id="8f25d-177">displayName</span><span class="sxs-lookup"><span data-stu-id="8f25d-177">displayName</span></span>|<span data-ttu-id="8f25d-178">String</span><span class="sxs-lookup"><span data-stu-id="8f25d-178">String</span></span>|<span data-ttu-id="8f25d-179">Отображаемое имя элемента</span><span class="sxs-lookup"><span data-stu-id="8f25d-179">Display name of the item</span></span>|
|<span data-ttu-id="8f25d-180">version</span><span class="sxs-lookup"><span data-stu-id="8f25d-180">version</span></span>|<span data-ttu-id="8f25d-181">String</span><span class="sxs-lookup"><span data-stu-id="8f25d-181">String</span></span>|<span data-ttu-id="8f25d-182">Версия элемента</span><span class="sxs-lookup"><span data-stu-id="8f25d-182">Item Version</span></span>|



## <a name="response"></a><span data-ttu-id="8f25d-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f25d-183">Response</span></span>
<span data-ttu-id="8f25d-184">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f25d-184">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f25d-185">Пример</span><span class="sxs-lookup"><span data-stu-id="8f25d-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f25d-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f25d-186">Request</span></span>
<span data-ttu-id="8f25d-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f25d-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
Content-type: application/json
Content-length: 977

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingDefinition",
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
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="8f25d-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f25d-188">Response</span></span>
<span data-ttu-id="8f25d-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f25d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1026

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingDefinition",
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
  "id": "7af649e5-49e5-7af6-e549-f67ae549f67a",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```




