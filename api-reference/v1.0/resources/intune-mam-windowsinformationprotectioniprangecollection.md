---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
ms.openlocfilehash: 41558014ec3d48af06788e15fc40786fe7f9aea4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025492"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="ca052-103">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="ca052-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="ca052-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ca052-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca052-105">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="ca052-105">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="ca052-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca052-106">Properties</span></span>
|<span data-ttu-id="ca052-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca052-107">Property</span></span>|<span data-ttu-id="ca052-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ca052-108">Type</span></span>|<span data-ttu-id="ca052-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ca052-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca052-110">displayName</span><span class="sxs-lookup"><span data-stu-id="ca052-110">displayName</span></span>|<span data-ttu-id="ca052-111">Строка</span><span class="sxs-lookup"><span data-stu-id="ca052-111">String</span></span>|<span data-ttu-id="ca052-112">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="ca052-112">Display name</span></span>|
|<span data-ttu-id="ca052-113">ranges</span><span class="sxs-lookup"><span data-stu-id="ca052-113">ranges</span></span>|<span data-ttu-id="ca052-114">Коллекция объектов [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="ca052-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="ca052-115">Коллекция диапазонов IP-адресов</span><span class="sxs-lookup"><span data-stu-id="ca052-115">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca052-116">Связи</span><span class="sxs-lookup"><span data-stu-id="ca052-116">Relationships</span></span>
<span data-ttu-id="ca052-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ca052-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ca052-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca052-118">JSON Representation</span></span>
<span data-ttu-id="ca052-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca052-119">Here is a JSON representation of the resource.</span></span>
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



