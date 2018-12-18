---
title: Тип ресурса omaSetting
description: Определение параметра OMA.
author: tfitzmac
ms.openlocfilehash: 564912635fbcd5e2846965d3546a3830119db252
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340889"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="c21f7-103">Тип ресурса omaSetting</span><span class="sxs-lookup"><span data-stu-id="c21f7-103">omaSetting resource type</span></span>

> <span data-ttu-id="c21f7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c21f7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c21f7-105">Определение параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="c21f7-105">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="c21f7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c21f7-106">Properties</span></span>
|<span data-ttu-id="c21f7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c21f7-107">Property</span></span>|<span data-ttu-id="c21f7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c21f7-108">Type</span></span>|<span data-ttu-id="c21f7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c21f7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c21f7-110">displayName</span><span class="sxs-lookup"><span data-stu-id="c21f7-110">displayName</span></span>|<span data-ttu-id="c21f7-111">Строка</span><span class="sxs-lookup"><span data-stu-id="c21f7-111">String</span></span>|<span data-ttu-id="c21f7-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="c21f7-112">Display Name.</span></span>|
|<span data-ttu-id="c21f7-113">описание</span><span class="sxs-lookup"><span data-stu-id="c21f7-113">description</span></span>|<span data-ttu-id="c21f7-114">Строка</span><span class="sxs-lookup"><span data-stu-id="c21f7-114">String</span></span>|<span data-ttu-id="c21f7-115">Описание.</span><span class="sxs-lookup"><span data-stu-id="c21f7-115">Description.</span></span>|
|<span data-ttu-id="c21f7-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="c21f7-116">omaUri</span></span>|<span data-ttu-id="c21f7-117">Строка</span><span class="sxs-lookup"><span data-stu-id="c21f7-117">String</span></span>|<span data-ttu-id="c21f7-118">OMA.</span><span class="sxs-lookup"><span data-stu-id="c21f7-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c21f7-119">Связи</span><span class="sxs-lookup"><span data-stu-id="c21f7-119">Relationships</span></span>
<span data-ttu-id="c21f7-120">Нет</span><span class="sxs-lookup"><span data-stu-id="c21f7-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c21f7-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c21f7-121">JSON Representation</span></span>
<span data-ttu-id="c21f7-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c21f7-122">Here is a JSON representation of the resource.</span></span>
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



