---
title: Обновление Девицеманажементконфигуратионсеттингдефинитион
description: Обновление свойств объекта Девицеманажементконфигуратионсеттингдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cb49bbd90b7c952deba932e0bbd1946f7bfc6ede
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242547"
---
# <a name="update-devicemanagementconfigurationsettingdefinition"></a><span data-ttu-id="4d5bc-103">Обновление Девицеманажементконфигуратионсеттингдефинитион</span><span class="sxs-lookup"><span data-stu-id="4d5bc-103">Update deviceManagementConfigurationSettingDefinition</span></span>

<span data-ttu-id="4d5bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d5bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d5bc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d5bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d5bc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d5bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d5bc-107">Обновление свойств объекта [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="4d5bc-107">Update the properties of a [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d5bc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4d5bc-108">Prerequisites</span></span>
<span data-ttu-id="4d5bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d5bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d5bc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4d5bc-111">Permission type</span></span>|<span data-ttu-id="4d5bc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4d5bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d5bc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4d5bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4d5bc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d5bc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4d5bc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4d5bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d5bc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d5bc-116">Not supported.</span></span>|
|<span data-ttu-id="4d5bc-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4d5bc-117">Application</span></span>|<span data-ttu-id="4d5bc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d5bc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d5bc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4d5bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="4d5bc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4d5bc-120">Request headers</span></span>
|<span data-ttu-id="4d5bc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4d5bc-121">Header</span></span>|<span data-ttu-id="4d5bc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4d5bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d5bc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4d5bc-123">Authorization</span></span>|<span data-ttu-id="4d5bc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4d5bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d5bc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4d5bc-125">Accept</span></span>|<span data-ttu-id="4d5bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d5bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d5bc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4d5bc-127">Request body</span></span>
<span data-ttu-id="4d5bc-128">В тексте запроса добавьте представление объекта [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d5bc-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

<span data-ttu-id="4d5bc-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4d5bc-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span>

|<span data-ttu-id="4d5bc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d5bc-130">Property</span></span>|<span data-ttu-id="4d5bc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4d5bc-131">Type</span></span>|<span data-ttu-id="4d5bc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4d5bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d5bc-133">применения</span><span class="sxs-lookup"><span data-stu-id="4d5bc-133">applicability</span></span>|[<span data-ttu-id="4d5bc-134">девицеманажементконфигуратионсеттингаппликабилити</span><span class="sxs-lookup"><span data-stu-id="4d5bc-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="4d5bc-135">Сведения о том, какие параметры устройства применяются для</span><span class="sxs-lookup"><span data-stu-id="4d5bc-135">Details which device setting is applicable on</span></span>|
|<span data-ttu-id="4d5bc-136">акцесстипес</span><span class="sxs-lookup"><span data-stu-id="4d5bc-136">accessTypes</span></span>|[<span data-ttu-id="4d5bc-137">девицеманажементконфигуратионсеттингакцесстипес</span><span class="sxs-lookup"><span data-stu-id="4d5bc-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="4d5bc-138">Режим доступа для чтения и записи параметра.</span><span class="sxs-lookup"><span data-stu-id="4d5bc-138">Read/write access mode of the setting.</span></span> <span data-ttu-id="4d5bc-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="4d5bc-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="4d5bc-140">keywords</span><span class="sxs-lookup"><span data-stu-id="4d5bc-140">keywords</span></span>|<span data-ttu-id="4d5bc-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4d5bc-141">String collection</span></span>|<span data-ttu-id="4d5bc-142">Маркеры, для которых необходимо выполнить поиск параметров</span><span class="sxs-lookup"><span data-stu-id="4d5bc-142">Tokens which to search settings on</span></span>|
|<span data-ttu-id="4d5bc-143">инфаурлс</span><span class="sxs-lookup"><span data-stu-id="4d5bc-143">infoUrls</span></span>|<span data-ttu-id="4d5bc-144">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4d5bc-144">String collection</span></span>|<span data-ttu-id="4d5bc-145">Список ссылок дополнительные сведения для параметра можно найти по адресу</span><span class="sxs-lookup"><span data-stu-id="4d5bc-145">List of links more info for the setting can be found at</span></span>|
|<span data-ttu-id="4d5bc-146">экземпляр</span><span class="sxs-lookup"><span data-stu-id="4d5bc-146">occurrence</span></span>|[<span data-ttu-id="4d5bc-147">девицеманажементконфигуратионсеттингоккурренце</span><span class="sxs-lookup"><span data-stu-id="4d5bc-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="4d5bc-148">Указывает, является ли параметр обязательным или нет</span><span class="sxs-lookup"><span data-stu-id="4d5bc-148">Indicates whether the setting is required or not</span></span>|
|<span data-ttu-id="4d5bc-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="4d5bc-149">baseUri</span></span>|<span data-ttu-id="4d5bc-150">String</span><span class="sxs-lookup"><span data-stu-id="4d5bc-150">String</span></span>|<span data-ttu-id="4d5bc-151">Путь к основному поставщику служб шифрования</span><span class="sxs-lookup"><span data-stu-id="4d5bc-151">Base CSP Path</span></span>|
|<span data-ttu-id="4d5bc-152">оффсетури</span><span class="sxs-lookup"><span data-stu-id="4d5bc-152">offsetUri</span></span>|<span data-ttu-id="4d5bc-153">String</span><span class="sxs-lookup"><span data-stu-id="4d5bc-153">String</span></span>|<span data-ttu-id="4d5bc-154">Путь от базового поставщика CSP</span><span class="sxs-lookup"><span data-stu-id="4d5bc-154">Offset CSP Path from Base</span></span>|
|<span data-ttu-id="4d5bc-155">рутдефинитионид</span><span class="sxs-lookup"><span data-stu-id="4d5bc-155">rootDefinitionId</span></span>|<span data-ttu-id="4d5bc-156">String</span><span class="sxs-lookup"><span data-stu-id="4d5bc-156">String</span></span>|<span data-ttu-id="4d5bc-157">Определение корневого параметра, если параметр является дочерним.</span><span class="sxs-lookup"><span data-stu-id="4d5bc-157">Root setting definition if the setting is a child setting.</span></span>|
|<span data-ttu-id="4d5bc-158">categoryId</span><span class="sxs-lookup"><span data-stu-id="4d5bc-158">categoryId</span></span>|<span data-ttu-id="4d5bc-159">String</span><span class="sxs-lookup"><span data-stu-id="4d5bc-159">String</span></span>|<span data-ttu-id="4d5bc-160">Указывает группу областей, в которой параметр настроен в указанном поставщике службы конфигурации (CSP).</span><span class="sxs-lookup"><span data-stu-id="4d5bc-160">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP)</span></span>|
|<span data-ttu-id="4d5bc-161">сеттингусаже</span><span class="sxs-lookup"><span data-stu-id="4d5bc-161">settingUsage</span></span>|[<span data-ttu-id="4d5bc-162">девицеманажементконфигуратионсеттингусаже</span><span class="sxs-lookup"><span data-stu-id="4d5bc-162">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="4d5bc-163">Тип параметра, например, "Конфигурация" и "соответствие".</span><span class="sxs-lookup"><span data-stu-id="4d5bc-163">Setting type, for example, configuration and compliance.</span></span> <span data-ttu-id="4d5bc-164">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="4d5bc-164">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="4d5bc-165">id</span><span class="sxs-lookup"><span data-stu-id="4d5bc-165">id</span></span>|<span data-ttu-id="4d5bc-166">String</span><span class="sxs-lookup"><span data-stu-id="4d5bc-166">String</span></span>|<span data-ttu-id="4d5bc-167">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="4d5bc-167">Identifier for item</span></span>|
|<span data-ttu-id="4d5bc-168">description</span><span class="sxs-lookup"><span data-stu-id="4d5bc-168">description</span></span>|<span data-ttu-id="4d5bc-169">String</span><span class="sxs-lookup"><span data-stu-id="4d5bc-169">String</span></span>|<span data-ttu-id="4d5bc-170">Описание элемента</span><span class="sxs-lookup"><span data-stu-id="4d5bc-170">Description of the item</span></span>|
|<span data-ttu-id="4d5bc-171">helpText</span><span class="sxs-lookup"><span data-stu-id="4d5bc-171">helpText</span></span>|<span data-ttu-id="4d5bc-172">String</span><span class="sxs-lookup"><span data-stu-id="4d5bc-172">String</span></span>|<span data-ttu-id="4d5bc-173">Текст справки элемента</span><span class="sxs-lookup"><span data-stu-id="4d5bc-173">Help text of the item</span></span>|
|<span data-ttu-id="4d5bc-174">name</span><span class="sxs-lookup"><span data-stu-id="4d5bc-174">name</span></span>|<span data-ttu-id="4d5bc-175">String</span><span class="sxs-lookup"><span data-stu-id="4d5bc-175">String</span></span>|<span data-ttu-id="4d5bc-176">Имя элемента</span><span class="sxs-lookup"><span data-stu-id="4d5bc-176">Name of the item</span></span>|
|<span data-ttu-id="4d5bc-177">displayName</span><span class="sxs-lookup"><span data-stu-id="4d5bc-177">displayName</span></span>|<span data-ttu-id="4d5bc-178">String</span><span class="sxs-lookup"><span data-stu-id="4d5bc-178">String</span></span>|<span data-ttu-id="4d5bc-179">Отображаемое имя элемента</span><span class="sxs-lookup"><span data-stu-id="4d5bc-179">Display name of the item</span></span>|
|<span data-ttu-id="4d5bc-180">version</span><span class="sxs-lookup"><span data-stu-id="4d5bc-180">version</span></span>|<span data-ttu-id="4d5bc-181">String</span><span class="sxs-lookup"><span data-stu-id="4d5bc-181">String</span></span>|<span data-ttu-id="4d5bc-182">Версия элемента</span><span class="sxs-lookup"><span data-stu-id="4d5bc-182">Item Version</span></span>|



## <a name="response"></a><span data-ttu-id="4d5bc-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d5bc-183">Response</span></span>
<span data-ttu-id="4d5bc-184">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементконфигуратионсеттингдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4d5bc-184">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d5bc-185">Пример</span><span class="sxs-lookup"><span data-stu-id="4d5bc-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d5bc-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="4d5bc-186">Request</span></span>
<span data-ttu-id="4d5bc-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4d5bc-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
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

### <a name="response"></a><span data-ttu-id="4d5bc-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="4d5bc-188">Response</span></span>
<span data-ttu-id="4d5bc-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4d5bc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




