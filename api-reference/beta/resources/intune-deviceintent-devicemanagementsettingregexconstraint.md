---
title: Тип ресурса Девицеманажементсеттингрежексконстраинт
description: Ограничение, в соответствии с которым параметр соответствует заданному шаблону регулярного выражения
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9e4eca30a72ebeeaf3c1410fd458821519ea11c9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785297"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a><span data-ttu-id="38c32-103">Тип ресурса Девицеманажементсеттингрежексконстраинт</span><span class="sxs-lookup"><span data-stu-id="38c32-103">deviceManagementSettingRegexConstraint resource type</span></span>

> <span data-ttu-id="38c32-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38c32-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38c32-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38c32-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38c32-106">Ограничение, в соответствии с которым параметр соответствует заданному шаблону регулярного выражения</span><span class="sxs-lookup"><span data-stu-id="38c32-106">Constraint enforcing the setting matches against a given RegEx pattern</span></span>


<span data-ttu-id="38c32-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="38c32-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="38c32-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="38c32-108">Properties</span></span>
|<span data-ttu-id="38c32-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="38c32-109">Property</span></span>|<span data-ttu-id="38c32-110">Тип</span><span class="sxs-lookup"><span data-stu-id="38c32-110">Type</span></span>|<span data-ttu-id="38c32-111">Описание</span><span class="sxs-lookup"><span data-stu-id="38c32-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38c32-112">выражений</span><span class="sxs-lookup"><span data-stu-id="38c32-112">regex</span></span>|<span data-ttu-id="38c32-113">String</span><span class="sxs-lookup"><span data-stu-id="38c32-113">String</span></span>|<span data-ttu-id="38c32-114">Шаблон регулярного выражения, с которым выполняется сравнение</span><span class="sxs-lookup"><span data-stu-id="38c32-114">The RegEx pattern to match against</span></span>|

## <a name="relationships"></a><span data-ttu-id="38c32-115">Связи</span><span class="sxs-lookup"><span data-stu-id="38c32-115">Relationships</span></span>
<span data-ttu-id="38c32-116">Нет</span><span class="sxs-lookup"><span data-stu-id="38c32-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38c32-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38c32-117">JSON Representation</span></span>
<span data-ttu-id="38c32-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38c32-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingRegexConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingRegexConstraint",
  "regex": "String"
}
```



