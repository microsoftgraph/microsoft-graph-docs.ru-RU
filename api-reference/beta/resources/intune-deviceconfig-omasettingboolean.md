---
title: Тип ресурса omaSettingBoolean
description: Логическое определение параметров OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab28f26ee4898b3481ae7f24516a650a5fea414f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950930"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="9fdeb-103">Тип ресурса omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="9fdeb-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="9fdeb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fdeb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fdeb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9fdeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fdeb-106">Логическое определение параметров OMA.</span><span class="sxs-lookup"><span data-stu-id="9fdeb-106">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="9fdeb-107">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9fdeb-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9fdeb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fdeb-108">Properties</span></span>
|<span data-ttu-id="9fdeb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fdeb-109">Property</span></span>|<span data-ttu-id="9fdeb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9fdeb-110">Type</span></span>|<span data-ttu-id="9fdeb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9fdeb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fdeb-112">displayName</span><span class="sxs-lookup"><span data-stu-id="9fdeb-112">displayName</span></span>|<span data-ttu-id="9fdeb-113">Строка</span><span class="sxs-lookup"><span data-stu-id="9fdeb-113">String</span></span>|<span data-ttu-id="9fdeb-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="9fdeb-114">Display Name.</span></span> <span data-ttu-id="9fdeb-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9fdeb-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9fdeb-116">description</span><span class="sxs-lookup"><span data-stu-id="9fdeb-116">description</span></span>|<span data-ttu-id="9fdeb-117">String</span><span class="sxs-lookup"><span data-stu-id="9fdeb-117">String</span></span>|<span data-ttu-id="9fdeb-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="9fdeb-118">Description.</span></span> <span data-ttu-id="9fdeb-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9fdeb-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9fdeb-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="9fdeb-120">omaUri</span></span>|<span data-ttu-id="9fdeb-121">String</span><span class="sxs-lookup"><span data-stu-id="9fdeb-121">String</span></span>|<span data-ttu-id="9fdeb-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="9fdeb-122">OMA.</span></span> <span data-ttu-id="9fdeb-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9fdeb-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9fdeb-124">value</span><span class="sxs-lookup"><span data-stu-id="9fdeb-124">value</span></span>|<span data-ttu-id="9fdeb-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fdeb-125">Boolean</span></span>|<span data-ttu-id="9fdeb-126">Значение</span><span class="sxs-lookup"><span data-stu-id="9fdeb-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fdeb-127">Связи</span><span class="sxs-lookup"><span data-stu-id="9fdeb-127">Relationships</span></span>
<span data-ttu-id="9fdeb-128">Нет</span><span class="sxs-lookup"><span data-stu-id="9fdeb-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fdeb-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9fdeb-129">JSON Representation</span></span>
<span data-ttu-id="9fdeb-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fdeb-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```




