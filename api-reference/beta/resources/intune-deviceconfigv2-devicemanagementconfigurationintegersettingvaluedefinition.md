---
title: Тип ресурса Девицеманажементконфигуратионинтежерсеттингвалуедефинитион
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d4c2fdb6b26b67b6c61dcbba295933d0c3797500
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242228"
---
# <a name="devicemanagementconfigurationintegersettingvaluedefinition-resource-type"></a><span data-ttu-id="b952f-103">Тип ресурса Девицеманажементконфигуратионинтежерсеттингвалуедефинитион</span><span class="sxs-lookup"><span data-stu-id="b952f-103">deviceManagementConfigurationIntegerSettingValueDefinition resource type</span></span>

<span data-ttu-id="b952f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b952f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b952f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b952f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b952f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b952f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b952f-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="b952f-107">Not yet documented</span></span>


<span data-ttu-id="b952f-108">Наследуется от [девицеманажементконфигуратионсеттингвалуедефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)</span><span class="sxs-lookup"><span data-stu-id="b952f-108">Inherits from [deviceManagementConfigurationSettingValueDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluedefinition.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b952f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b952f-109">Properties</span></span>
|<span data-ttu-id="b952f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b952f-110">Property</span></span>|<span data-ttu-id="b952f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b952f-111">Type</span></span>|<span data-ttu-id="b952f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b952f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b952f-113">максимумвалуе</span><span class="sxs-lookup"><span data-stu-id="b952f-113">maximumValue</span></span>|<span data-ttu-id="b952f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="b952f-114">Int64</span></span>|<span data-ttu-id="b952f-115">Максимально допустимое значение целого числа</span><span class="sxs-lookup"><span data-stu-id="b952f-115">Maximum allowed value of the integer</span></span>|
|<span data-ttu-id="b952f-116">минимумвалуе</span><span class="sxs-lookup"><span data-stu-id="b952f-116">minimumValue</span></span>|<span data-ttu-id="b952f-117">Int64</span><span class="sxs-lookup"><span data-stu-id="b952f-117">Int64</span></span>|<span data-ttu-id="b952f-118">Минимальное допустимое значение целого числа</span><span class="sxs-lookup"><span data-stu-id="b952f-118">Minimum allowed value of the integer</span></span>|

## <a name="relationships"></a><span data-ttu-id="b952f-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b952f-119">Relationships</span></span>
<span data-ttu-id="b952f-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b952f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b952f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b952f-121">JSON Representation</span></span>
<span data-ttu-id="b952f-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b952f-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinition",
  "maximumValue": 1024,
  "minimumValue": 1024
}
```




