---
title: Тип ресурса Девицеманажементконфигуратионстрингсеттингвалуедефинитион
description: Ограничения строк
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 03a96252cffabddd2acb613ff365fd16951fd55c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242384"
---
# <a name="devicemanagementconfigurationstringsettingvaluedefinition-resource-type"></a><span data-ttu-id="7cf34-103">Тип ресурса Девицеманажементконфигуратионстрингсеттингвалуедефинитион</span><span class="sxs-lookup"><span data-stu-id="7cf34-103">deviceManagementConfigurationStringSettingValueDefinition resource type</span></span>

<span data-ttu-id="7cf34-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cf34-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7cf34-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cf34-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7cf34-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7cf34-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cf34-107">Ограничения строк</span><span class="sxs-lookup"><span data-stu-id="7cf34-107">String constraints</span></span>


<span data-ttu-id="7cf34-108">Наследуется от [девицеманажементконфигуратионсеттингвалуедефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7cf34-108">Inherits from [deviceManagementConfigurationSettingValueDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7cf34-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7cf34-109">Properties</span></span>
|<span data-ttu-id="7cf34-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7cf34-110">Property</span></span>|<span data-ttu-id="7cf34-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7cf34-111">Type</span></span>|<span data-ttu-id="7cf34-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7cf34-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cf34-113">format</span><span class="sxs-lookup"><span data-stu-id="7cf34-113">format</span></span>|[<span data-ttu-id="7cf34-114">девицеманажементконфигуратионстрингформат</span><span class="sxs-lookup"><span data-stu-id="7cf34-114">deviceManagementConfigurationStringFormat</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringformat.md)|<span data-ttu-id="7cf34-115">Предварительно определенный формат строки.</span><span class="sxs-lookup"><span data-stu-id="7cf34-115">Pre-defined format of the string.</span></span> <span data-ttu-id="7cf34-116">Возможные значения: `none` , `email` ,,,,, `guid` `ip` `base64` `url` `version` ,,, `xml` `date` `time` , `binary` , `regEx` , `json` , `dateTime` , `surfaceHub` .</span><span class="sxs-lookup"><span data-stu-id="7cf34-116">Possible values are: `none`, `email`, `guid`, `ip`, `base64`, `url`, `version`, `xml`, `date`, `time`, `binary`, `regEx`, `json`, `dateTime`, `surfaceHub`.</span></span>|
|<span data-ttu-id="7cf34-117">инпутвалидатионсчема</span><span class="sxs-lookup"><span data-stu-id="7cf34-117">inputValidationSchema</span></span>|<span data-ttu-id="7cf34-118">String</span><span class="sxs-lookup"><span data-stu-id="7cf34-118">String</span></span>|<span data-ttu-id="7cf34-119">Регулярное выражение или любая схема XML или JSON, которой должна быть соотнесена входная строка</span><span class="sxs-lookup"><span data-stu-id="7cf34-119">Regular expression or any xml or json schema that the input string should match</span></span>|
|<span data-ttu-id="7cf34-120">максимумленгс</span><span class="sxs-lookup"><span data-stu-id="7cf34-120">maximumLength</span></span>|<span data-ttu-id="7cf34-121">Int64</span><span class="sxs-lookup"><span data-stu-id="7cf34-121">Int64</span></span>|<span data-ttu-id="7cf34-122">Максимальная длина строки.</span><span class="sxs-lookup"><span data-stu-id="7cf34-122">Maximum length of string.</span></span> <span data-ttu-id="7cf34-123">Допустимые значения — от 0 до 87516</span><span class="sxs-lookup"><span data-stu-id="7cf34-123">Valid values 0 to 87516</span></span>|
|<span data-ttu-id="7cf34-124">минимумленгс</span><span class="sxs-lookup"><span data-stu-id="7cf34-124">minimumLength</span></span>|<span data-ttu-id="7cf34-125">Int64</span><span class="sxs-lookup"><span data-stu-id="7cf34-125">Int64</span></span>|<span data-ttu-id="7cf34-126">Минимальная длина строки.</span><span class="sxs-lookup"><span data-stu-id="7cf34-126">Minimum length of string.</span></span> <span data-ttu-id="7cf34-127">Допустимые значения — от 0 до 87516</span><span class="sxs-lookup"><span data-stu-id="7cf34-127">Valid values 0 to 87516</span></span>|
|<span data-ttu-id="7cf34-128">Secret</span><span class="sxs-lookup"><span data-stu-id="7cf34-128">isSecret</span></span>|<span data-ttu-id="7cf34-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="7cf34-129">Boolean</span></span>|<span data-ttu-id="7cf34-130">Указывает, нужно ли считать параметр секретом.</span><span class="sxs-lookup"><span data-stu-id="7cf34-130">Specifies whether the setting needs to be treated as a secret.</span></span> <span data-ttu-id="7cf34-131">Параметры, помеченные как "Да", будут зашифрованы на транспорте и будут отображаться в виде звездочек, когда они представлены в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="7cf34-131">Settings marked as yes will be encrypted in transit and at rest and will be displayed as asterisks when represented in the UX.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7cf34-132">Связи</span><span class="sxs-lookup"><span data-stu-id="7cf34-132">Relationships</span></span>
<span data-ttu-id="7cf34-133">Нет</span><span class="sxs-lookup"><span data-stu-id="7cf34-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7cf34-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7cf34-134">JSON Representation</span></span>
<span data-ttu-id="7cf34-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7cf34-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationStringSettingValueDefinition",
  "format": "String",
  "inputValidationSchema": "String",
  "maximumLength": 1024,
  "minimumLength": 1024,
  "isSecret": true
}
```




