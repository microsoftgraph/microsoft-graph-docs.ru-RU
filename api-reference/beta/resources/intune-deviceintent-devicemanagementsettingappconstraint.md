---
title: Тип ресурса Девицеманажементсеттингаппконстраинт
description: Ограничение, включающее параметр, содержит только доступные типы приложений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 891b07ff24bb43696ba45de418194295446a98f3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49275596"
---
# <a name="devicemanagementsettingappconstraint-resource-type"></a><span data-ttu-id="42d2e-103">Тип ресурса Девицеманажементсеттингаппконстраинт</span><span class="sxs-lookup"><span data-stu-id="42d2e-103">deviceManagementSettingAppConstraint resource type</span></span>

<span data-ttu-id="42d2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42d2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42d2e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42d2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42d2e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42d2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42d2e-107">Ограничение, включающее параметр, содержит только доступные типы приложений.</span><span class="sxs-lookup"><span data-stu-id="42d2e-107">Constraint enforcing the setting contains only vaild app types.</span></span>


<span data-ttu-id="42d2e-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="42d2e-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="42d2e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="42d2e-109">Properties</span></span>
|<span data-ttu-id="42d2e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="42d2e-110">Property</span></span>|<span data-ttu-id="42d2e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="42d2e-111">Type</span></span>|<span data-ttu-id="42d2e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="42d2e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42d2e-113">суппортедтипес</span><span class="sxs-lookup"><span data-stu-id="42d2e-113">supportedTypes</span></span>|<span data-ttu-id="42d2e-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="42d2e-114">String collection</span></span>|<span data-ttu-id="42d2e-115">Допустимые типы приложений, которые необходимо разрешить для этого параметра</span><span class="sxs-lookup"><span data-stu-id="42d2e-115">Acceptable app types to allow for this setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="42d2e-116">Связи</span><span class="sxs-lookup"><span data-stu-id="42d2e-116">Relationships</span></span>
<span data-ttu-id="42d2e-117">Нет</span><span class="sxs-lookup"><span data-stu-id="42d2e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42d2e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42d2e-118">JSON Representation</span></span>
<span data-ttu-id="42d2e-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42d2e-119">Here is a JSON representation of the resource.</span></span>
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




