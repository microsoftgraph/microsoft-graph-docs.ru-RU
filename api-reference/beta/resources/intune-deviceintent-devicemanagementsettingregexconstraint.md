---
title: Тип ресурса Девицеманажементсеттингрежексконстраинт
description: Ограничение, в соответствии с которым параметр соответствует заданному шаблону регулярного выражения
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3d6f811330ceaa282a547de0f51d075598bd16fc
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730448"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a><span data-ttu-id="ca2f8-103">Тип ресурса Девицеманажементсеттингрежексконстраинт</span><span class="sxs-lookup"><span data-stu-id="ca2f8-103">deviceManagementSettingRegexConstraint resource type</span></span>

<span data-ttu-id="ca2f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca2f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca2f8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca2f8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca2f8-107">Ограничение, в соответствии с которым параметр соответствует заданному шаблону регулярного выражения</span><span class="sxs-lookup"><span data-stu-id="ca2f8-107">Constraint enforcing the setting matches against a given RegEx pattern</span></span>


<span data-ttu-id="ca2f8-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="ca2f8-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ca2f8-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca2f8-109">Properties</span></span>
|<span data-ttu-id="ca2f8-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca2f8-110">Property</span></span>|<span data-ttu-id="ca2f8-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ca2f8-111">Type</span></span>|<span data-ttu-id="ca2f8-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ca2f8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca2f8-113">выражений</span><span class="sxs-lookup"><span data-stu-id="ca2f8-113">regex</span></span>|<span data-ttu-id="ca2f8-114">Строка</span><span class="sxs-lookup"><span data-stu-id="ca2f8-114">String</span></span>|<span data-ttu-id="ca2f8-115">Шаблон регулярного выражения, с которым выполняется сравнение</span><span class="sxs-lookup"><span data-stu-id="ca2f8-115">The RegEx pattern to match against</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca2f8-116">Связи</span><span class="sxs-lookup"><span data-stu-id="ca2f8-116">Relationships</span></span>
<span data-ttu-id="ca2f8-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ca2f8-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca2f8-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca2f8-118">JSON Representation</span></span>
<span data-ttu-id="ca2f8-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca2f8-119">Here is a JSON representation of the resource.</span></span>
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





