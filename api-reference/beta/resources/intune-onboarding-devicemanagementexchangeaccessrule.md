---
title: Тип ресурса Девицеманажементексчанжеакцессруле
description: Правила доступа к устройству в Exchange.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a6d32744d2fd3cb48f52c85b314e72d50983dffc
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42779193"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="84c12-103">Тип ресурса Девицеманажементексчанжеакцессруле</span><span class="sxs-lookup"><span data-stu-id="84c12-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="84c12-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84c12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84c12-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84c12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84c12-106">Правила доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="84c12-106">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="84c12-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="84c12-107">Properties</span></span>
|<span data-ttu-id="84c12-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="84c12-108">Property</span></span>|<span data-ttu-id="84c12-109">Тип</span><span class="sxs-lookup"><span data-stu-id="84c12-109">Type</span></span>|<span data-ttu-id="84c12-110">Описание</span><span class="sxs-lookup"><span data-stu-id="84c12-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84c12-111">девицекласс</span><span class="sxs-lookup"><span data-stu-id="84c12-111">deviceClass</span></span>|[<span data-ttu-id="84c12-112">девицеманажементексчанжедевицекласс</span><span class="sxs-lookup"><span data-stu-id="84c12-112">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="84c12-113">Класс устройства, на который влияет это правило.</span><span class="sxs-lookup"><span data-stu-id="84c12-113">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="84c12-114">accessLevel</span><span class="sxs-lookup"><span data-stu-id="84c12-114">accessLevel</span></span>|[<span data-ttu-id="84c12-115">девицеманажементексчанжеакцесслевел</span><span class="sxs-lookup"><span data-stu-id="84c12-115">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="84c12-116">Уровень доступа для Exchange, предоставляемый этим правилом.</span><span class="sxs-lookup"><span data-stu-id="84c12-116">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="84c12-117">Возможные значения: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="84c12-117">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84c12-118">Связи</span><span class="sxs-lookup"><span data-stu-id="84c12-118">Relationships</span></span>
<span data-ttu-id="84c12-119">Нет</span><span class="sxs-lookup"><span data-stu-id="84c12-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84c12-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84c12-120">JSON Representation</span></span>
<span data-ttu-id="84c12-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84c12-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeAccessRule",
  "deviceClass": {
    "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
    "name": "String",
    "type": "String"
  },
  "accessLevel": "String"
}
```



