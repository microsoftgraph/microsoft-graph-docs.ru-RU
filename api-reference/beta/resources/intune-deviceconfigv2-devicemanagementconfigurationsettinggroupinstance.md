---
title: Тип ресурса Девицеманажементконфигуратионсеттингграупинстанце
description: Установка экземпляра в политике
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1ab5093675e8d1bc9b0796a5a937b9bed894ca24
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242176"
---
# <a name="devicemanagementconfigurationsettinggroupinstance-resource-type"></a><span data-ttu-id="4416a-103">Тип ресурса Девицеманажементконфигуратионсеттингграупинстанце</span><span class="sxs-lookup"><span data-stu-id="4416a-103">deviceManagementConfigurationSettingGroupInstance resource type</span></span>

<span data-ttu-id="4416a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4416a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4416a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4416a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4416a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4416a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4416a-107">Установка экземпляра в политике</span><span class="sxs-lookup"><span data-stu-id="4416a-107">Setting instance within policy</span></span>


<span data-ttu-id="4416a-108">Наследуется от [девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="4416a-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4416a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4416a-109">Properties</span></span>
|<span data-ttu-id="4416a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4416a-110">Property</span></span>|<span data-ttu-id="4416a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4416a-111">Type</span></span>|<span data-ttu-id="4416a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4416a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4416a-113">сеттингдефинитионид</span><span class="sxs-lookup"><span data-stu-id="4416a-113">settingDefinitionId</span></span>|<span data-ttu-id="4416a-114">String</span><span class="sxs-lookup"><span data-stu-id="4416a-114">String</span></span>|<span data-ttu-id="4416a-115">Параметр ID определения, наследуемый от [девицеманажементконфигуратионсеттингинстанце](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="4416a-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="4416a-116">Связи</span><span class="sxs-lookup"><span data-stu-id="4416a-116">Relationships</span></span>
<span data-ttu-id="4416a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="4416a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4416a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4416a-118">JSON Representation</span></span>
<span data-ttu-id="4416a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4416a-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingGroupInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupInstance",
  "settingDefinitionId": "String"
}
```




