---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9981b585818bb6db712b0088b2fde275179917ef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911828"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="07c29-103">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="07c29-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="07c29-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="07c29-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07c29-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07c29-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07c29-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="07c29-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07c29-107">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="07c29-107">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="07c29-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="07c29-108">Properties</span></span>
|<span data-ttu-id="07c29-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="07c29-109">Property</span></span>|<span data-ttu-id="07c29-110">Тип</span><span class="sxs-lookup"><span data-stu-id="07c29-110">Type</span></span>|<span data-ttu-id="07c29-111">Описание</span><span class="sxs-lookup"><span data-stu-id="07c29-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07c29-112">displayName</span><span class="sxs-lookup"><span data-stu-id="07c29-112">displayName</span></span>|<span data-ttu-id="07c29-113">Строка</span><span class="sxs-lookup"><span data-stu-id="07c29-113">String</span></span>|<span data-ttu-id="07c29-114">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="07c29-114">Display name</span></span>|
|<span data-ttu-id="07c29-115">ranges</span><span class="sxs-lookup"><span data-stu-id="07c29-115">ranges</span></span>|<span data-ttu-id="07c29-116">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="07c29-116">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="07c29-117">Коллекция диапазонов IP-адресов</span><span class="sxs-lookup"><span data-stu-id="07c29-117">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="07c29-118">Связи</span><span class="sxs-lookup"><span data-stu-id="07c29-118">Relationships</span></span>
<span data-ttu-id="07c29-119">Нет</span><span class="sxs-lookup"><span data-stu-id="07c29-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="07c29-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07c29-120">JSON Representation</span></span>
<span data-ttu-id="07c29-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07c29-121">Here is a JSON representation of the resource.</span></span>
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





