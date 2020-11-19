---
title: Тип ресурса Девицеманажементсеттингрежексконстраинт
description: Ограничение, в соответствии с которым параметр соответствует заданному шаблону регулярного выражения
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 11d06b2af4273166b3d6cf93a36a76fecc7ec548
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267931"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a><span data-ttu-id="33e71-103">Тип ресурса Девицеманажементсеттингрежексконстраинт</span><span class="sxs-lookup"><span data-stu-id="33e71-103">deviceManagementSettingRegexConstraint resource type</span></span>

<span data-ttu-id="33e71-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33e71-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33e71-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33e71-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33e71-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33e71-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33e71-107">Ограничение, в соответствии с которым параметр соответствует заданному шаблону регулярного выражения</span><span class="sxs-lookup"><span data-stu-id="33e71-107">Constraint enforcing the setting matches against a given RegEx pattern</span></span>


<span data-ttu-id="33e71-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="33e71-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="33e71-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="33e71-109">Properties</span></span>
|<span data-ttu-id="33e71-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="33e71-110">Property</span></span>|<span data-ttu-id="33e71-111">Тип</span><span class="sxs-lookup"><span data-stu-id="33e71-111">Type</span></span>|<span data-ttu-id="33e71-112">Описание</span><span class="sxs-lookup"><span data-stu-id="33e71-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33e71-113">выражений</span><span class="sxs-lookup"><span data-stu-id="33e71-113">regex</span></span>|<span data-ttu-id="33e71-114">String</span><span class="sxs-lookup"><span data-stu-id="33e71-114">String</span></span>|<span data-ttu-id="33e71-115">Шаблон регулярного выражения, с которым выполняется сравнение</span><span class="sxs-lookup"><span data-stu-id="33e71-115">The RegEx pattern to match against</span></span>|

## <a name="relationships"></a><span data-ttu-id="33e71-116">Связи</span><span class="sxs-lookup"><span data-stu-id="33e71-116">Relationships</span></span>
<span data-ttu-id="33e71-117">Нет</span><span class="sxs-lookup"><span data-stu-id="33e71-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="33e71-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="33e71-118">JSON Representation</span></span>
<span data-ttu-id="33e71-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33e71-119">Here is a JSON representation of the resource.</span></span>
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




