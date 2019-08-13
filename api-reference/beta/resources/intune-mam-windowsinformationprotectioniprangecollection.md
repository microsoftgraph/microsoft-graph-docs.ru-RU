---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f52af0fb969846f645d1cda15c952cf248852f80
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372897"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="7e805-103">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="7e805-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="7e805-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e805-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e805-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e805-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e805-106">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="7e805-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="7e805-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e805-107">Properties</span></span>
|<span data-ttu-id="7e805-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e805-108">Property</span></span>|<span data-ttu-id="7e805-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7e805-109">Type</span></span>|<span data-ttu-id="7e805-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7e805-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e805-111">displayName</span><span class="sxs-lookup"><span data-stu-id="7e805-111">displayName</span></span>|<span data-ttu-id="7e805-112">String</span><span class="sxs-lookup"><span data-stu-id="7e805-112">String</span></span>|<span data-ttu-id="7e805-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="7e805-113">Display name</span></span>|
|<span data-ttu-id="7e805-114">ranges</span><span class="sxs-lookup"><span data-stu-id="7e805-114">ranges</span></span>|<span data-ttu-id="7e805-115">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="7e805-115">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="7e805-116">Коллекция диапазонов IP-адресов</span><span class="sxs-lookup"><span data-stu-id="7e805-116">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e805-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="7e805-117">Relationships</span></span>
<span data-ttu-id="7e805-118">Нет</span><span class="sxs-lookup"><span data-stu-id="7e805-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e805-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e805-119">JSON Representation</span></span>
<span data-ttu-id="7e805-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e805-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionIPRangeCollection",
  "displayName": "String",
  "ranges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```



