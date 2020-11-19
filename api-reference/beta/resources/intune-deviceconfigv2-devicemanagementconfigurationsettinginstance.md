---
title: Тип ресурса Девицеманажементконфигуратионсеттингинстанце
description: Установка экземпляра в политике
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 757b60c1e290612bbf51ac66ec42d3f27ac57cca
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302210"
---
# <a name="devicemanagementconfigurationsettinginstance-resource-type"></a><span data-ttu-id="e3538-103">Тип ресурса Девицеманажементконфигуратионсеттингинстанце</span><span class="sxs-lookup"><span data-stu-id="e3538-103">deviceManagementConfigurationSettingInstance resource type</span></span>

<span data-ttu-id="e3538-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3538-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3538-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3538-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3538-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e3538-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3538-107">Установка экземпляра в политике</span><span class="sxs-lookup"><span data-stu-id="e3538-107">Setting instance within policy</span></span>

## <a name="properties"></a><span data-ttu-id="e3538-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3538-108">Properties</span></span>
|<span data-ttu-id="e3538-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3538-109">Property</span></span>|<span data-ttu-id="e3538-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e3538-110">Type</span></span>|<span data-ttu-id="e3538-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e3538-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3538-112">сеттингдефинитионид</span><span class="sxs-lookup"><span data-stu-id="e3538-112">settingDefinitionId</span></span>|<span data-ttu-id="e3538-113">String</span><span class="sxs-lookup"><span data-stu-id="e3538-113">String</span></span>|<span data-ttu-id="e3538-114">Идентификатор определения параметра</span><span class="sxs-lookup"><span data-stu-id="e3538-114">Setting Definition Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3538-115">Связи</span><span class="sxs-lookup"><span data-stu-id="e3538-115">Relationships</span></span>
<span data-ttu-id="e3538-116">Нет</span><span class="sxs-lookup"><span data-stu-id="e3538-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3538-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e3538-117">JSON Representation</span></span>
<span data-ttu-id="e3538-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3538-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingInstance",
  "settingDefinitionId": "String"
}
```




