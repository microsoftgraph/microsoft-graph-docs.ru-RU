---
title: Тип ресурса Девицеманажементсеттингрежексконстраинт
description: Ограничение, в соответствии с которым параметр соответствует заданному шаблону регулярного выражения
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 23b2397911afb877f513019e289800823f57a3c9
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34984480"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a><span data-ttu-id="5675a-103">Тип ресурса Девицеманажементсеттингрежексконстраинт</span><span class="sxs-lookup"><span data-stu-id="5675a-103">deviceManagementSettingRegexConstraint resource type</span></span>

> <span data-ttu-id="5675a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5675a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5675a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5675a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5675a-106">Ограничение, в соответствии с которым параметр соответствует заданному шаблону регулярного выражения</span><span class="sxs-lookup"><span data-stu-id="5675a-106">Constraint enforcing the setting matches against a given RegEx pattern</span></span>


<span data-ttu-id="5675a-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="5675a-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5675a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5675a-108">Properties</span></span>
|<span data-ttu-id="5675a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5675a-109">Property</span></span>|<span data-ttu-id="5675a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5675a-110">Type</span></span>|<span data-ttu-id="5675a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5675a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5675a-112">выражений</span><span class="sxs-lookup"><span data-stu-id="5675a-112">regex</span></span>|<span data-ttu-id="5675a-113">String</span><span class="sxs-lookup"><span data-stu-id="5675a-113">String</span></span>|<span data-ttu-id="5675a-114">Шаблон регулярного выражения, с которым выполняется сравнение</span><span class="sxs-lookup"><span data-stu-id="5675a-114">The RegEx pattern to match against</span></span>|

## <a name="relationships"></a><span data-ttu-id="5675a-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="5675a-115">Relationships</span></span>
<span data-ttu-id="5675a-116">Нет</span><span class="sxs-lookup"><span data-stu-id="5675a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5675a-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5675a-117">JSON Representation</span></span>
<span data-ttu-id="5675a-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5675a-118">Here is a JSON representation of the resource.</span></span>
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





