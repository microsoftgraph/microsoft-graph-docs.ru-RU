---
title: Тип ресурса Девицеманажементсеттингбулеанконстраинт
description: Constraint — принудительно определяет конкретное логическое значение
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 40891d8d80a617f4caf97527c02b8244880faf96
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061282"
---
# <a name="devicemanagementsettingbooleanconstraint-resource-type"></a><span data-ttu-id="ff2e0-103">Тип ресурса Девицеманажементсеттингбулеанконстраинт</span><span class="sxs-lookup"><span data-stu-id="ff2e0-103">deviceManagementSettingBooleanConstraint resource type</span></span>

<span data-ttu-id="ff2e0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff2e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff2e0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff2e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff2e0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff2e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff2e0-107">Constraint — принудительно определяет конкретное логическое значение</span><span class="sxs-lookup"><span data-stu-id="ff2e0-107">Constraint the enforces a particular boolean value</span></span>


<span data-ttu-id="ff2e0-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="ff2e0-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ff2e0-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff2e0-109">Properties</span></span>
|<span data-ttu-id="ff2e0-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff2e0-110">Property</span></span>|<span data-ttu-id="ff2e0-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ff2e0-111">Type</span></span>|<span data-ttu-id="ff2e0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ff2e0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff2e0-113">значение</span><span class="sxs-lookup"><span data-stu-id="ff2e0-113">value</span></span>|<span data-ttu-id="ff2e0-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff2e0-114">Boolean</span></span>|<span data-ttu-id="ff2e0-115">Логическое значение, с которым выполняется сравнение</span><span class="sxs-lookup"><span data-stu-id="ff2e0-115">The boolean value to compare against</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff2e0-116">Связи</span><span class="sxs-lookup"><span data-stu-id="ff2e0-116">Relationships</span></span>
<span data-ttu-id="ff2e0-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ff2e0-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff2e0-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff2e0-118">JSON Representation</span></span>
<span data-ttu-id="ff2e0-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff2e0-119">Here is a JSON representation of the resource.</span></span>
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






