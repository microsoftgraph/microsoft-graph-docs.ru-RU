---
title: Тип ресурса omaSettingString
description: Определение строки параметра OMA.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c1e0c0fe3f020519770c6770fe515f0349cd6994
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472974"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="9be89-103">Тип ресурса omaSettingString</span><span class="sxs-lookup"><span data-stu-id="9be89-103">omaSettingString resource type</span></span>

<span data-ttu-id="9be89-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9be89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9be89-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9be89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9be89-106">Определение строки параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="9be89-106">OMA Settings String definition.</span></span>


<span data-ttu-id="9be89-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9be89-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9be89-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9be89-108">Properties</span></span>
|<span data-ttu-id="9be89-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9be89-109">Property</span></span>|<span data-ttu-id="9be89-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9be89-110">Type</span></span>|<span data-ttu-id="9be89-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9be89-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9be89-112">displayName</span><span class="sxs-lookup"><span data-stu-id="9be89-112">displayName</span></span>|<span data-ttu-id="9be89-113">Строка</span><span class="sxs-lookup"><span data-stu-id="9be89-113">String</span></span>|<span data-ttu-id="9be89-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="9be89-114">Display Name.</span></span> <span data-ttu-id="9be89-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9be89-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9be89-116">description</span><span class="sxs-lookup"><span data-stu-id="9be89-116">description</span></span>|<span data-ttu-id="9be89-117">String</span><span class="sxs-lookup"><span data-stu-id="9be89-117">String</span></span>|<span data-ttu-id="9be89-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="9be89-118">Description.</span></span> <span data-ttu-id="9be89-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9be89-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9be89-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="9be89-120">omaUri</span></span>|<span data-ttu-id="9be89-121">String</span><span class="sxs-lookup"><span data-stu-id="9be89-121">String</span></span>|<span data-ttu-id="9be89-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="9be89-122">OMA.</span></span> <span data-ttu-id="9be89-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9be89-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9be89-124">value</span><span class="sxs-lookup"><span data-stu-id="9be89-124">value</span></span>|<span data-ttu-id="9be89-125">Строка</span><span class="sxs-lookup"><span data-stu-id="9be89-125">String</span></span>|<span data-ttu-id="9be89-126">Значение</span><span class="sxs-lookup"><span data-stu-id="9be89-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9be89-127">Связи</span><span class="sxs-lookup"><span data-stu-id="9be89-127">Relationships</span></span>
<span data-ttu-id="9be89-128">Нет</span><span class="sxs-lookup"><span data-stu-id="9be89-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9be89-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9be89-129">JSON Representation</span></span>
<span data-ttu-id="9be89-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9be89-130">Here is a JSON representation of the resource.</span></span>
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







