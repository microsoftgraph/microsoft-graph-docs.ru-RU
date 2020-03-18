---
title: Тип ресурса Девицеманажементсеттингаппконстраинт
description: Ограничение, включающее параметр, содержит только доступные типы приложений.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4b80fa581686692a47051405cc68f4d6d0694b95
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785381"
---
# <a name="devicemanagementsettingappconstraint-resource-type"></a><span data-ttu-id="e05c7-103">Тип ресурса Девицеманажементсеттингаппконстраинт</span><span class="sxs-lookup"><span data-stu-id="e05c7-103">deviceManagementSettingAppConstraint resource type</span></span>

> <span data-ttu-id="e05c7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e05c7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e05c7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e05c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e05c7-106">Ограничение, включающее параметр, содержит только доступные типы приложений.</span><span class="sxs-lookup"><span data-stu-id="e05c7-106">Constraint enforcing the setting contains only vaild app types.</span></span>


<span data-ttu-id="e05c7-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="e05c7-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e05c7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e05c7-108">Properties</span></span>
|<span data-ttu-id="e05c7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e05c7-109">Property</span></span>|<span data-ttu-id="e05c7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e05c7-110">Type</span></span>|<span data-ttu-id="e05c7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e05c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e05c7-112">суппортедтипес</span><span class="sxs-lookup"><span data-stu-id="e05c7-112">supportedTypes</span></span>|<span data-ttu-id="e05c7-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e05c7-113">String collection</span></span>|<span data-ttu-id="e05c7-114">Допустимые типы приложений, которые необходимо разрешить для этого параметра</span><span class="sxs-lookup"><span data-stu-id="e05c7-114">Acceptable app types to allow for this setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="e05c7-115">Связи</span><span class="sxs-lookup"><span data-stu-id="e05c7-115">Relationships</span></span>
<span data-ttu-id="e05c7-116">Нет</span><span class="sxs-lookup"><span data-stu-id="e05c7-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e05c7-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e05c7-117">JSON Representation</span></span>
<span data-ttu-id="e05c7-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e05c7-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingAppConstraint",
  "supportedTypes": [
    "String"
  ]
}
```



