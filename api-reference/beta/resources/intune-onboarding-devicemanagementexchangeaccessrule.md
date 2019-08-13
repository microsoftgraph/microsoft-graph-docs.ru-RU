---
title: Тип ресурса Девицеманажементексчанжеакцессруле
description: Правила доступа к устройству в Exchange.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9577ba5acf826598b0cefa6cf884bcc25dc50107
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374206"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="1056e-103">Тип ресурса Девицеманажементексчанжеакцессруле</span><span class="sxs-lookup"><span data-stu-id="1056e-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="1056e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1056e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1056e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1056e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1056e-106">Правила доступа к устройству в Exchange.</span><span class="sxs-lookup"><span data-stu-id="1056e-106">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="1056e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1056e-107">Properties</span></span>
|<span data-ttu-id="1056e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1056e-108">Property</span></span>|<span data-ttu-id="1056e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1056e-109">Type</span></span>|<span data-ttu-id="1056e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1056e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1056e-111">девицекласс</span><span class="sxs-lookup"><span data-stu-id="1056e-111">deviceClass</span></span>|[<span data-ttu-id="1056e-112">девицеманажементексчанжедевицекласс</span><span class="sxs-lookup"><span data-stu-id="1056e-112">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="1056e-113">Класс устройства, на который влияет это правило.</span><span class="sxs-lookup"><span data-stu-id="1056e-113">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="1056e-114">accessLevel</span><span class="sxs-lookup"><span data-stu-id="1056e-114">accessLevel</span></span>|[<span data-ttu-id="1056e-115">девицеманажементексчанжеакцесслевел</span><span class="sxs-lookup"><span data-stu-id="1056e-115">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="1056e-116">Уровень доступа для Exchange, предоставляемый этим правилом.</span><span class="sxs-lookup"><span data-stu-id="1056e-116">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="1056e-117">Возможные значения: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="1056e-117">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1056e-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="1056e-118">Relationships</span></span>
<span data-ttu-id="1056e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="1056e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1056e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1056e-120">JSON Representation</span></span>
<span data-ttu-id="1056e-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1056e-121">Here is a JSON representation of the resource.</span></span>
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



