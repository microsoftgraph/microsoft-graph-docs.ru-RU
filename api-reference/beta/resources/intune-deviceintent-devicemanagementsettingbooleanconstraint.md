---
title: Тип ресурса Девицеманажементсеттингбулеанконстраинт
description: Constraint — принудительно определяет конкретное логическое значение
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 301279028667b0d230ee016bf34cb708260d2f05
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528818"
---
# <a name="devicemanagementsettingbooleanconstraint-resource-type"></a><span data-ttu-id="ca557-103">Тип ресурса Девицеманажементсеттингбулеанконстраинт</span><span class="sxs-lookup"><span data-stu-id="ca557-103">deviceManagementSettingBooleanConstraint resource type</span></span>

<span data-ttu-id="ca557-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ca557-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca557-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca557-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca557-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca557-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca557-107">Constraint — принудительно определяет конкретное логическое значение</span><span class="sxs-lookup"><span data-stu-id="ca557-107">Constraint the enforces a particular boolean value</span></span>


<span data-ttu-id="ca557-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="ca557-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ca557-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca557-109">Properties</span></span>
|<span data-ttu-id="ca557-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca557-110">Property</span></span>|<span data-ttu-id="ca557-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ca557-111">Type</span></span>|<span data-ttu-id="ca557-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ca557-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca557-113">значение</span><span class="sxs-lookup"><span data-stu-id="ca557-113">value</span></span>|<span data-ttu-id="ca557-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca557-114">Boolean</span></span>|<span data-ttu-id="ca557-115">Логическое значение, с которым выполняется сравнение</span><span class="sxs-lookup"><span data-stu-id="ca557-115">The boolean value to compare against</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca557-116">Связи</span><span class="sxs-lookup"><span data-stu-id="ca557-116">Relationships</span></span>
<span data-ttu-id="ca557-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ca557-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca557-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca557-118">JSON Representation</span></span>
<span data-ttu-id="ca557-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca557-119">Here is a JSON representation of the resource.</span></span>
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



