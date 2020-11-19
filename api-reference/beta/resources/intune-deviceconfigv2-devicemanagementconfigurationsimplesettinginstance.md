---
title: Тип ресурса Девицеманажементконфигуратионсимплесеттингинстанце
description: Экземпляр простого параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 52ee180adbdd19ac95aa70159f198797d75ec302
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242392"
---
# <a name="devicemanagementconfigurationsimplesettinginstance-resource-type"></a><span data-ttu-id="04251-103">Тип ресурса Девицеманажементконфигуратионсимплесеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="04251-103">deviceManagementConfigurationSimpleSettingInstance resource type</span></span>

<span data-ttu-id="04251-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04251-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04251-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04251-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04251-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04251-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04251-107">Экземпляр простого параметра</span><span class="sxs-lookup"><span data-stu-id="04251-107">Simple setting instance</span></span>


<span data-ttu-id="04251-108">Наследуется от [девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="04251-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="04251-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="04251-109">Properties</span></span>
|<span data-ttu-id="04251-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="04251-110">Property</span></span>|<span data-ttu-id="04251-111">Тип</span><span class="sxs-lookup"><span data-stu-id="04251-111">Type</span></span>|<span data-ttu-id="04251-112">Описание</span><span class="sxs-lookup"><span data-stu-id="04251-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04251-113">сеттингдефинитионид</span><span class="sxs-lookup"><span data-stu-id="04251-113">settingDefinitionId</span></span>|<span data-ttu-id="04251-114">String</span><span class="sxs-lookup"><span data-stu-id="04251-114">String</span></span>|<span data-ttu-id="04251-115">Параметр ID определения, наследуемый от [девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="04251-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="04251-116">симплесеттингвалуе</span><span class="sxs-lookup"><span data-stu-id="04251-116">simpleSettingValue</span></span>|[<span data-ttu-id="04251-117">девицеманажементконфигуратионсимплесеттингвалуе</span><span class="sxs-lookup"><span data-stu-id="04251-117">deviceManagementConfigurationSimpleSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)|<span data-ttu-id="04251-118">Значение экземпляра простого параметра</span><span class="sxs-lookup"><span data-stu-id="04251-118">Simple setting instance value</span></span>|

## <a name="relationships"></a><span data-ttu-id="04251-119">Связи</span><span class="sxs-lookup"><span data-stu-id="04251-119">Relationships</span></span>
<span data-ttu-id="04251-120">Нет</span><span class="sxs-lookup"><span data-stu-id="04251-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04251-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04251-121">JSON Representation</span></span>
<span data-ttu-id="04251-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04251-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingInstance",
  "settingDefinitionId": "String",
  "simpleSettingValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValue",
    "value": "String"
  }
}
```




