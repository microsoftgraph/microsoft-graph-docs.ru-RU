---
title: Тип ресурса Девицеманажементсеттингрежексконстраинт
description: Ограничение, в соответствии с которым параметр соответствует заданному шаблону регулярного выражения
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d0f9a04583bfb9b28546e9057f0530f72558a0be
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364637"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a><span data-ttu-id="fde37-103">Тип ресурса Девицеманажементсеттингрежексконстраинт</span><span class="sxs-lookup"><span data-stu-id="fde37-103">deviceManagementSettingRegexConstraint resource type</span></span>

> <span data-ttu-id="fde37-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fde37-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fde37-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fde37-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fde37-106">Ограничение, в соответствии с которым параметр соответствует заданному шаблону регулярного выражения</span><span class="sxs-lookup"><span data-stu-id="fde37-106">Constraint enforcing the setting matches against a given RegEx pattern</span></span>


<span data-ttu-id="fde37-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="fde37-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fde37-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fde37-108">Properties</span></span>
|<span data-ttu-id="fde37-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fde37-109">Property</span></span>|<span data-ttu-id="fde37-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fde37-110">Type</span></span>|<span data-ttu-id="fde37-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fde37-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fde37-112">выражений</span><span class="sxs-lookup"><span data-stu-id="fde37-112">regex</span></span>|<span data-ttu-id="fde37-113">String</span><span class="sxs-lookup"><span data-stu-id="fde37-113">String</span></span>|<span data-ttu-id="fde37-114">Шаблон регулярного выражения, с которым выполняется сравнение</span><span class="sxs-lookup"><span data-stu-id="fde37-114">The RegEx pattern to match against</span></span>|

## <a name="relationships"></a><span data-ttu-id="fde37-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="fde37-115">Relationships</span></span>
<span data-ttu-id="fde37-116">Нет</span><span class="sxs-lookup"><span data-stu-id="fde37-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fde37-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fde37-117">JSON Representation</span></span>
<span data-ttu-id="fde37-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fde37-118">Here is a JSON representation of the resource.</span></span>
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



