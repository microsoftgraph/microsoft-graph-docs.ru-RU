---
title: Тип ресурса omaSettingString
description: Определение строки параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c24e9a0f04e039870d14ebfc33a9462e9e911209
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722952"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="eb511-103">Тип ресурса omaSettingString</span><span class="sxs-lookup"><span data-stu-id="eb511-103">omaSettingString resource type</span></span>

<span data-ttu-id="eb511-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb511-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb511-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb511-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb511-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eb511-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb511-107">Определение строки параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="eb511-107">OMA Settings String definition.</span></span>


<span data-ttu-id="eb511-108">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="eb511-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eb511-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb511-109">Properties</span></span>
|<span data-ttu-id="eb511-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb511-110">Property</span></span>|<span data-ttu-id="eb511-111">Тип</span><span class="sxs-lookup"><span data-stu-id="eb511-111">Type</span></span>|<span data-ttu-id="eb511-112">Описание</span><span class="sxs-lookup"><span data-stu-id="eb511-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb511-113">displayName</span><span class="sxs-lookup"><span data-stu-id="eb511-113">displayName</span></span>|<span data-ttu-id="eb511-114">Строка</span><span class="sxs-lookup"><span data-stu-id="eb511-114">String</span></span>|<span data-ttu-id="eb511-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="eb511-115">Display Name.</span></span> <span data-ttu-id="eb511-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="eb511-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="eb511-117">description</span><span class="sxs-lookup"><span data-stu-id="eb511-117">description</span></span>|<span data-ttu-id="eb511-118">Строка</span><span class="sxs-lookup"><span data-stu-id="eb511-118">String</span></span>|<span data-ttu-id="eb511-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="eb511-119">Description.</span></span> <span data-ttu-id="eb511-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="eb511-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="eb511-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="eb511-121">omaUri</span></span>|<span data-ttu-id="eb511-122">String</span><span class="sxs-lookup"><span data-stu-id="eb511-122">String</span></span>|<span data-ttu-id="eb511-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="eb511-123">OMA.</span></span> <span data-ttu-id="eb511-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="eb511-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="eb511-125">value</span><span class="sxs-lookup"><span data-stu-id="eb511-125">value</span></span>|<span data-ttu-id="eb511-126">String</span><span class="sxs-lookup"><span data-stu-id="eb511-126">String</span></span>|<span data-ttu-id="eb511-127">Значение</span><span class="sxs-lookup"><span data-stu-id="eb511-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb511-128">Связи</span><span class="sxs-lookup"><span data-stu-id="eb511-128">Relationships</span></span>
<span data-ttu-id="eb511-129">Нет</span><span class="sxs-lookup"><span data-stu-id="eb511-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb511-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb511-130">JSON Representation</span></span>
<span data-ttu-id="eb511-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb511-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```





