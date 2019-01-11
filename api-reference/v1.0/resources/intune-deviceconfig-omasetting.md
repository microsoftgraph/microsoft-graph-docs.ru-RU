---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 86cb06b35a0f64052860c268764696a1db8459e3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888384"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="76860-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="76860-103">omaSetting resource type</span></span>

> <span data-ttu-id="76860-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="76860-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="76860-105">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="76860-105">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="76860-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="76860-106">Properties</span></span>
|<span data-ttu-id="76860-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="76860-107">Property</span></span>|<span data-ttu-id="76860-108">Тип</span><span class="sxs-lookup"><span data-stu-id="76860-108">Type</span></span>|<span data-ttu-id="76860-109">Описание</span><span class="sxs-lookup"><span data-stu-id="76860-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76860-110">displayName</span><span class="sxs-lookup"><span data-stu-id="76860-110">displayName</span></span>|<span data-ttu-id="76860-111">Строка</span><span class="sxs-lookup"><span data-stu-id="76860-111">String</span></span>|<span data-ttu-id="76860-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="76860-112">Display Name.</span></span>|
|<span data-ttu-id="76860-113">описание</span><span class="sxs-lookup"><span data-stu-id="76860-113">description</span></span>|<span data-ttu-id="76860-114">Строка</span><span class="sxs-lookup"><span data-stu-id="76860-114">String</span></span>|<span data-ttu-id="76860-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="76860-115">Description.</span></span>|
|<span data-ttu-id="76860-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="76860-116">omaUri</span></span>|<span data-ttu-id="76860-117">Строка</span><span class="sxs-lookup"><span data-stu-id="76860-117">String</span></span>|<span data-ttu-id="76860-118">OMA.</span><span class="sxs-lookup"><span data-stu-id="76860-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76860-119">Связи</span><span class="sxs-lookup"><span data-stu-id="76860-119">Relationships</span></span>
<span data-ttu-id="76860-120">Нет</span><span class="sxs-lookup"><span data-stu-id="76860-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="76860-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76860-121">JSON Representation</span></span>
<span data-ttu-id="76860-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76860-122">Here is a JSON representation of the resource.</span></span>
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



