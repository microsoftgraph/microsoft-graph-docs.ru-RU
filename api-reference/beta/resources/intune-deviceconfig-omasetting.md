---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0bb5df5f786eefc1b7b7159b1643f9d3d46d8300
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958706"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="2202b-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="2202b-103">omaSetting resource type</span></span>

> <span data-ttu-id="2202b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2202b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2202b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2202b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2202b-106">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="2202b-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="2202b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2202b-107">Properties</span></span>
|<span data-ttu-id="2202b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2202b-108">Property</span></span>|<span data-ttu-id="2202b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2202b-109">Type</span></span>|<span data-ttu-id="2202b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2202b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2202b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="2202b-111">displayName</span></span>|<span data-ttu-id="2202b-112">Строка</span><span class="sxs-lookup"><span data-stu-id="2202b-112">String</span></span>|<span data-ttu-id="2202b-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="2202b-113">Display Name.</span></span>|
|<span data-ttu-id="2202b-114">description</span><span class="sxs-lookup"><span data-stu-id="2202b-114">description</span></span>|<span data-ttu-id="2202b-115">String</span><span class="sxs-lookup"><span data-stu-id="2202b-115">String</span></span>|<span data-ttu-id="2202b-116">Описание.</span><span class="sxs-lookup"><span data-stu-id="2202b-116">Description.</span></span>|
|<span data-ttu-id="2202b-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="2202b-117">omaUri</span></span>|<span data-ttu-id="2202b-118">String</span><span class="sxs-lookup"><span data-stu-id="2202b-118">String</span></span>|<span data-ttu-id="2202b-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="2202b-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2202b-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="2202b-120">Relationships</span></span>
<span data-ttu-id="2202b-121">Нет</span><span class="sxs-lookup"><span data-stu-id="2202b-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2202b-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2202b-122">JSON Representation</span></span>
<span data-ttu-id="2202b-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2202b-123">Here is a JSON representation of the resource.</span></span>
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





