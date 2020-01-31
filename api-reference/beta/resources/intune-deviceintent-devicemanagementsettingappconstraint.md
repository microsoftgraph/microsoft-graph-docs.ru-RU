---
title: Тип ресурса Девицеманажементсеттингаппконстраинт
description: Ограничение, включающее параметр, содержит только доступные типы приложений.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 218e4ca91d69c1d68b19e12ed659a3cd87884b5b
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636793"
---
# <a name="devicemanagementsettingappconstraint-resource-type"></a><span data-ttu-id="84af6-103">Тип ресурса Девицеманажементсеттингаппконстраинт</span><span class="sxs-lookup"><span data-stu-id="84af6-103">deviceManagementSettingAppConstraint resource type</span></span>

> <span data-ttu-id="84af6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84af6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84af6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84af6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84af6-106">Ограничение, включающее параметр, содержит только доступные типы приложений.</span><span class="sxs-lookup"><span data-stu-id="84af6-106">Constraint enforcing the setting contains only vaild app types.</span></span>


<span data-ttu-id="84af6-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="84af6-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="84af6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="84af6-108">Properties</span></span>
|<span data-ttu-id="84af6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="84af6-109">Property</span></span>|<span data-ttu-id="84af6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="84af6-110">Type</span></span>|<span data-ttu-id="84af6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="84af6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84af6-112">суппортедтипес</span><span class="sxs-lookup"><span data-stu-id="84af6-112">supportedTypes</span></span>|<span data-ttu-id="84af6-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="84af6-113">String collection</span></span>|<span data-ttu-id="84af6-114">Допустимые типы приложений, которые необходимо разрешить для этого параметра</span><span class="sxs-lookup"><span data-stu-id="84af6-114">Acceptable app types to allow for this setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="84af6-115">Связи</span><span class="sxs-lookup"><span data-stu-id="84af6-115">Relationships</span></span>
<span data-ttu-id="84af6-116">Нет</span><span class="sxs-lookup"><span data-stu-id="84af6-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84af6-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84af6-117">JSON Representation</span></span>
<span data-ttu-id="84af6-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84af6-118">Here is a JSON representation of the resource.</span></span>
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



