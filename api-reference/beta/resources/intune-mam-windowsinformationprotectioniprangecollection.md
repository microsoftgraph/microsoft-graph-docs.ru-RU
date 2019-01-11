---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 73995f6b8f5e376de53ec88772dc3713cc179f3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838607"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="290c3-103">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="290c3-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="290c3-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="290c3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="290c3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="290c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="290c3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="290c3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="290c3-107">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="290c3-107">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="290c3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="290c3-108">Properties</span></span>
|<span data-ttu-id="290c3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="290c3-109">Property</span></span>|<span data-ttu-id="290c3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="290c3-110">Type</span></span>|<span data-ttu-id="290c3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="290c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="290c3-112">displayName</span><span class="sxs-lookup"><span data-stu-id="290c3-112">displayName</span></span>|<span data-ttu-id="290c3-113">Строка</span><span class="sxs-lookup"><span data-stu-id="290c3-113">String</span></span>|<span data-ttu-id="290c3-114">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="290c3-114">Display name</span></span>|
|<span data-ttu-id="290c3-115">ranges</span><span class="sxs-lookup"><span data-stu-id="290c3-115">ranges</span></span>|<span data-ttu-id="290c3-116">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="290c3-116">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="290c3-117">Коллекция диапазонов IP-адресов</span><span class="sxs-lookup"><span data-stu-id="290c3-117">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="290c3-118">Связи</span><span class="sxs-lookup"><span data-stu-id="290c3-118">Relationships</span></span>
<span data-ttu-id="290c3-119">Нет</span><span class="sxs-lookup"><span data-stu-id="290c3-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="290c3-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="290c3-120">JSON Representation</span></span>
<span data-ttu-id="290c3-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="290c3-121">Here is a JSON representation of the resource.</span></span>
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





