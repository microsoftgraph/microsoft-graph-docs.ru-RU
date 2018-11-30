---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
ms.openlocfilehash: 72b7c982197701f936a11b7b474a8acd86393260
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081789"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="6da8e-103">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="6da8e-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="6da8e-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6da8e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6da8e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6da8e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6da8e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6da8e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6da8e-107">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="6da8e-107">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="6da8e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6da8e-108">Properties</span></span>
|<span data-ttu-id="6da8e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6da8e-109">Property</span></span>|<span data-ttu-id="6da8e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6da8e-110">Type</span></span>|<span data-ttu-id="6da8e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6da8e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6da8e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="6da8e-112">displayName</span></span>|<span data-ttu-id="6da8e-113">Строка</span><span class="sxs-lookup"><span data-stu-id="6da8e-113">String</span></span>|<span data-ttu-id="6da8e-114">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="6da8e-114">Display name</span></span>|
|<span data-ttu-id="6da8e-115">ranges</span><span class="sxs-lookup"><span data-stu-id="6da8e-115">ranges</span></span>|<span data-ttu-id="6da8e-116">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="6da8e-116">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="6da8e-117">Коллекция диапазонов IP-адресов</span><span class="sxs-lookup"><span data-stu-id="6da8e-117">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="6da8e-118">Связи</span><span class="sxs-lookup"><span data-stu-id="6da8e-118">Relationships</span></span>
<span data-ttu-id="6da8e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="6da8e-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6da8e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6da8e-120">JSON Representation</span></span>
<span data-ttu-id="6da8e-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6da8e-121">Here is a JSON representation of the resource.</span></span>
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





