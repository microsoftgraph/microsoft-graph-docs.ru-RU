---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
author: tfitzmac
ms.openlocfilehash: 12030ab0b71448c644e4e664f9095dea3e48a26c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319756"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="10b27-103">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="10b27-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="10b27-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="10b27-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10b27-105">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="10b27-105">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="10b27-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="10b27-106">Properties</span></span>
|<span data-ttu-id="10b27-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="10b27-107">Property</span></span>|<span data-ttu-id="10b27-108">Тип</span><span class="sxs-lookup"><span data-stu-id="10b27-108">Type</span></span>|<span data-ttu-id="10b27-109">Описание</span><span class="sxs-lookup"><span data-stu-id="10b27-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10b27-110">displayName</span><span class="sxs-lookup"><span data-stu-id="10b27-110">displayName</span></span>|<span data-ttu-id="10b27-111">Строка</span><span class="sxs-lookup"><span data-stu-id="10b27-111">String</span></span>|<span data-ttu-id="10b27-112">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="10b27-112">Display name</span></span>|
|<span data-ttu-id="10b27-113">ranges</span><span class="sxs-lookup"><span data-stu-id="10b27-113">ranges</span></span>|<span data-ttu-id="10b27-114">Коллекция объектов [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="10b27-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="10b27-115">Коллекция диапазонов IP-адресов</span><span class="sxs-lookup"><span data-stu-id="10b27-115">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="10b27-116">Связи</span><span class="sxs-lookup"><span data-stu-id="10b27-116">Relationships</span></span>
<span data-ttu-id="10b27-117">Нет</span><span class="sxs-lookup"><span data-stu-id="10b27-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="10b27-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="10b27-118">JSON Representation</span></span>
<span data-ttu-id="10b27-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10b27-119">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.ipRange",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```



