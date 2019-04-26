---
title: Тип ресурса omaSettingString
description: Определение строки параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b32d5f6942dc5c0284e0ecaa11a27f4df0e99b3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569055"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="cd537-103">Тип ресурса omaSettingString</span><span class="sxs-lookup"><span data-stu-id="cd537-103">omaSettingString resource type</span></span>

> <span data-ttu-id="cd537-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd537-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd537-105">Определение строки параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="cd537-105">OMA Settings String definition.</span></span>


<span data-ttu-id="cd537-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cd537-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cd537-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd537-107">Properties</span></span>
|<span data-ttu-id="cd537-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd537-108">Property</span></span>|<span data-ttu-id="cd537-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cd537-109">Type</span></span>|<span data-ttu-id="cd537-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cd537-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd537-111">displayName</span><span class="sxs-lookup"><span data-stu-id="cd537-111">displayName</span></span>|<span data-ttu-id="cd537-112">String</span><span class="sxs-lookup"><span data-stu-id="cd537-112">String</span></span>|<span data-ttu-id="cd537-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="cd537-113">Display Name.</span></span> <span data-ttu-id="cd537-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cd537-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cd537-115">description</span><span class="sxs-lookup"><span data-stu-id="cd537-115">description</span></span>|<span data-ttu-id="cd537-116">String</span><span class="sxs-lookup"><span data-stu-id="cd537-116">String</span></span>|<span data-ttu-id="cd537-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="cd537-117">Description.</span></span> <span data-ttu-id="cd537-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cd537-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cd537-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="cd537-119">omaUri</span></span>|<span data-ttu-id="cd537-120">String</span><span class="sxs-lookup"><span data-stu-id="cd537-120">String</span></span>|<span data-ttu-id="cd537-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="cd537-121">OMA.</span></span> <span data-ttu-id="cd537-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cd537-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cd537-123">value</span><span class="sxs-lookup"><span data-stu-id="cd537-123">value</span></span>|<span data-ttu-id="cd537-124">Строка</span><span class="sxs-lookup"><span data-stu-id="cd537-124">String</span></span>|<span data-ttu-id="cd537-125">Значение</span><span class="sxs-lookup"><span data-stu-id="cd537-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd537-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="cd537-126">Relationships</span></span>
<span data-ttu-id="cd537-127">Нет</span><span class="sxs-lookup"><span data-stu-id="cd537-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd537-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd537-128">JSON Representation</span></span>
<span data-ttu-id="cd537-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd537-129">Here is a JSON representation of the resource.</span></span>
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



