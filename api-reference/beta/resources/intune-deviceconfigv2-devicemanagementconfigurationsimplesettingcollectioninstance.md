---
title: Тип ресурса Девицеманажементконфигуратионсимплесеттингколлектионинстанце
description: Экземпляр коллекции "простой параметр"
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b0886b7665f1f3ce16780f2ecccc77635fd70cf3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242360"
---
# <a name="devicemanagementconfigurationsimplesettingcollectioninstance-resource-type"></a><span data-ttu-id="d8b8d-103">Тип ресурса Девицеманажементконфигуратионсимплесеттингколлектионинстанце</span><span class="sxs-lookup"><span data-stu-id="d8b8d-103">deviceManagementConfigurationSimpleSettingCollectionInstance resource type</span></span>

<span data-ttu-id="d8b8d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8b8d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8b8d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8b8d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8b8d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8b8d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8b8d-107">Экземпляр коллекции "простой параметр"</span><span class="sxs-lookup"><span data-stu-id="d8b8d-107">Simple setting collection instance</span></span>


<span data-ttu-id="d8b8d-108">Наследуется от [девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="d8b8d-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d8b8d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8b8d-109">Properties</span></span>
|<span data-ttu-id="d8b8d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8b8d-110">Property</span></span>|<span data-ttu-id="d8b8d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d8b8d-111">Type</span></span>|<span data-ttu-id="d8b8d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d8b8d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8b8d-113">сеттингдефинитионид</span><span class="sxs-lookup"><span data-stu-id="d8b8d-113">settingDefinitionId</span></span>|<span data-ttu-id="d8b8d-114">String</span><span class="sxs-lookup"><span data-stu-id="d8b8d-114">String</span></span>|<span data-ttu-id="d8b8d-115">Параметр ID определения, наследуемый от [девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="d8b8d-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="d8b8d-116">симплесеттингколлектионвалуе</span><span class="sxs-lookup"><span data-stu-id="d8b8d-116">simpleSettingCollectionValue</span></span>|<span data-ttu-id="d8b8d-117">Коллекция [девицеманажементконфигуратионсимплесеттингвалуе](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d8b8d-117">[deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md) collection</span></span>|<span data-ttu-id="d8b8d-118">Значение экземпляра коллекции "Простая настройка"</span><span class="sxs-lookup"><span data-stu-id="d8b8d-118">Simple setting collection instance value</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8b8d-119">Связи</span><span class="sxs-lookup"><span data-stu-id="d8b8d-119">Relationships</span></span>
<span data-ttu-id="d8b8d-120">Нет</span><span class="sxs-lookup"><span data-stu-id="d8b8d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8b8d-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8b8d-121">JSON Representation</span></span>
<span data-ttu-id="d8b8d-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8b8d-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstance",
  "settingDefinitionId": "String",
  "simpleSettingCollectionValue": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValue",
      "value": "String"
    }
  ]
}
```




