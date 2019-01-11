---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2ba01b8a4385b5c06cc1e6a95441e9b7946a116d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839748"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="62a4b-103">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="62a4b-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="62a4b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="62a4b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62a4b-105">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="62a4b-105">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="62a4b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="62a4b-106">Properties</span></span>
|<span data-ttu-id="62a4b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="62a4b-107">Property</span></span>|<span data-ttu-id="62a4b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="62a4b-108">Type</span></span>|<span data-ttu-id="62a4b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="62a4b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62a4b-110">displayName</span><span class="sxs-lookup"><span data-stu-id="62a4b-110">displayName</span></span>|<span data-ttu-id="62a4b-111">Строка</span><span class="sxs-lookup"><span data-stu-id="62a4b-111">String</span></span>|<span data-ttu-id="62a4b-112">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="62a4b-112">Display name</span></span>|
|<span data-ttu-id="62a4b-113">ranges</span><span class="sxs-lookup"><span data-stu-id="62a4b-113">ranges</span></span>|<span data-ttu-id="62a4b-114">Коллекция объектов [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="62a4b-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="62a4b-115">Коллекция диапазонов IP-адресов</span><span class="sxs-lookup"><span data-stu-id="62a4b-115">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="62a4b-116">Связи</span><span class="sxs-lookup"><span data-stu-id="62a4b-116">Relationships</span></span>
<span data-ttu-id="62a4b-117">Нет</span><span class="sxs-lookup"><span data-stu-id="62a4b-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="62a4b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="62a4b-118">JSON Representation</span></span>
<span data-ttu-id="62a4b-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62a4b-119">Here is a JSON representation of the resource.</span></span>
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



