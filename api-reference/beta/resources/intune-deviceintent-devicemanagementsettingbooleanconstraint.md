---
title: Тип ресурса Девицеманажементсеттингбулеанконстраинт
description: Constraint — принудительно определяет конкретное логическое значение
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9a83a0747e0960aeebaa0de472fae4d587111946
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364728"
---
# <a name="devicemanagementsettingbooleanconstraint-resource-type"></a><span data-ttu-id="f2e4a-103">Тип ресурса Девицеманажементсеттингбулеанконстраинт</span><span class="sxs-lookup"><span data-stu-id="f2e4a-103">deviceManagementSettingBooleanConstraint resource type</span></span>

> <span data-ttu-id="f2e4a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2e4a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2e4a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f2e4a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2e4a-106">Constraint — принудительно определяет конкретное логическое значение</span><span class="sxs-lookup"><span data-stu-id="f2e4a-106">Constraint the enforces a particular boolean value</span></span>


<span data-ttu-id="f2e4a-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="f2e4a-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f2e4a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2e4a-108">Properties</span></span>
|<span data-ttu-id="f2e4a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2e4a-109">Property</span></span>|<span data-ttu-id="f2e4a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f2e4a-110">Type</span></span>|<span data-ttu-id="f2e4a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f2e4a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2e4a-112">значение</span><span class="sxs-lookup"><span data-stu-id="f2e4a-112">value</span></span>|<span data-ttu-id="f2e4a-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2e4a-113">Boolean</span></span>|<span data-ttu-id="f2e4a-114">Логическое значение, с которым выполняется сравнение</span><span class="sxs-lookup"><span data-stu-id="f2e4a-114">The boolean value to compare against</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2e4a-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="f2e4a-115">Relationships</span></span>
<span data-ttu-id="f2e4a-116">Нет</span><span class="sxs-lookup"><span data-stu-id="f2e4a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2e4a-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f2e4a-117">JSON Representation</span></span>
<span data-ttu-id="f2e4a-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2e4a-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingBooleanConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingBooleanConstraint",
  "value": true
}
```



