---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5d4c232f346e9966c72bcd60e0fd08af139db068
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783229"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="b87bd-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="b87bd-103">omaSetting resource type</span></span>

> <span data-ttu-id="b87bd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b87bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b87bd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b87bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b87bd-106">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="b87bd-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="b87bd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b87bd-107">Properties</span></span>
|<span data-ttu-id="b87bd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b87bd-108">Property</span></span>|<span data-ttu-id="b87bd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b87bd-109">Type</span></span>|<span data-ttu-id="b87bd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b87bd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b87bd-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b87bd-111">displayName</span></span>|<span data-ttu-id="b87bd-112">String</span><span class="sxs-lookup"><span data-stu-id="b87bd-112">String</span></span>|<span data-ttu-id="b87bd-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="b87bd-113">Display Name.</span></span>|
|<span data-ttu-id="b87bd-114">description</span><span class="sxs-lookup"><span data-stu-id="b87bd-114">description</span></span>|<span data-ttu-id="b87bd-115">String</span><span class="sxs-lookup"><span data-stu-id="b87bd-115">String</span></span>|<span data-ttu-id="b87bd-116">Описание.</span><span class="sxs-lookup"><span data-stu-id="b87bd-116">Description.</span></span>|
|<span data-ttu-id="b87bd-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="b87bd-117">omaUri</span></span>|<span data-ttu-id="b87bd-118">String</span><span class="sxs-lookup"><span data-stu-id="b87bd-118">String</span></span>|<span data-ttu-id="b87bd-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="b87bd-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b87bd-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="b87bd-120">Relationships</span></span>
<span data-ttu-id="b87bd-121">Нет</span><span class="sxs-lookup"><span data-stu-id="b87bd-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b87bd-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b87bd-122">JSON Representation</span></span>
<span data-ttu-id="b87bd-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b87bd-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```





