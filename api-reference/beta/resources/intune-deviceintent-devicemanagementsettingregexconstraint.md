---
title: Тип ресурса Девицеманажементсеттингрежексконстраинт
description: Ограничение, в соответствии с которым параметр соответствует заданному шаблону регулярного выражения
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 08734a71b179d55bc76e9cd82360773d7d17f3bb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061135"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a><span data-ttu-id="75aac-103">Тип ресурса Девицеманажементсеттингрежексконстраинт</span><span class="sxs-lookup"><span data-stu-id="75aac-103">deviceManagementSettingRegexConstraint resource type</span></span>

<span data-ttu-id="75aac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75aac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75aac-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75aac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75aac-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75aac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75aac-107">Ограничение, в соответствии с которым параметр соответствует заданному шаблону регулярного выражения</span><span class="sxs-lookup"><span data-stu-id="75aac-107">Constraint enforcing the setting matches against a given RegEx pattern</span></span>


<span data-ttu-id="75aac-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="75aac-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="75aac-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="75aac-109">Properties</span></span>
|<span data-ttu-id="75aac-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="75aac-110">Property</span></span>|<span data-ttu-id="75aac-111">Тип</span><span class="sxs-lookup"><span data-stu-id="75aac-111">Type</span></span>|<span data-ttu-id="75aac-112">Описание</span><span class="sxs-lookup"><span data-stu-id="75aac-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75aac-113">выражений</span><span class="sxs-lookup"><span data-stu-id="75aac-113">regex</span></span>|<span data-ttu-id="75aac-114">String</span><span class="sxs-lookup"><span data-stu-id="75aac-114">String</span></span>|<span data-ttu-id="75aac-115">Шаблон регулярного выражения, с которым выполняется сравнение</span><span class="sxs-lookup"><span data-stu-id="75aac-115">The RegEx pattern to match against</span></span>|

## <a name="relationships"></a><span data-ttu-id="75aac-116">Связи</span><span class="sxs-lookup"><span data-stu-id="75aac-116">Relationships</span></span>
<span data-ttu-id="75aac-117">Нет</span><span class="sxs-lookup"><span data-stu-id="75aac-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="75aac-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="75aac-118">JSON Representation</span></span>
<span data-ttu-id="75aac-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75aac-119">Here is a JSON representation of the resource.</span></span>
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






