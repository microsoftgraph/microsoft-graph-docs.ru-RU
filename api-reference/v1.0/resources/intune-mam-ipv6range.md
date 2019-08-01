---
title: Тип ресурса iPv6Range
description: Определение диапазона IPv6.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 04183f443d767236a1a7c0afb1d1ed9b92c37889
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038145"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="9a2fa-103">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="9a2fa-103">iPv6Range resource type</span></span>

> <span data-ttu-id="9a2fa-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a2fa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a2fa-105">Определение диапазона IPv6.</span><span class="sxs-lookup"><span data-stu-id="9a2fa-105">IPv6 Range definition.</span></span>


<span data-ttu-id="9a2fa-106">Наследуется от ресурса [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="9a2fa-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9a2fa-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a2fa-107">Properties</span></span>
|<span data-ttu-id="9a2fa-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a2fa-108">Property</span></span>|<span data-ttu-id="9a2fa-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9a2fa-109">Type</span></span>|<span data-ttu-id="9a2fa-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9a2fa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a2fa-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="9a2fa-111">lowerAddress</span></span>|<span data-ttu-id="9a2fa-112">String</span><span class="sxs-lookup"><span data-stu-id="9a2fa-112">String</span></span>|<span data-ttu-id="9a2fa-113">Понижение адреса</span><span class="sxs-lookup"><span data-stu-id="9a2fa-113">Lower address</span></span>|
|<span data-ttu-id="9a2fa-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="9a2fa-114">upperAddress</span></span>|<span data-ttu-id="9a2fa-115">String</span><span class="sxs-lookup"><span data-stu-id="9a2fa-115">String</span></span>|<span data-ttu-id="9a2fa-116">Верхний адрес</span><span class="sxs-lookup"><span data-stu-id="9a2fa-116">Upper address</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a2fa-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="9a2fa-117">Relationships</span></span>
<span data-ttu-id="9a2fa-118">Нет</span><span class="sxs-lookup"><span data-stu-id="9a2fa-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a2fa-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9a2fa-119">JSON Representation</span></span>
<span data-ttu-id="9a2fa-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a2fa-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



