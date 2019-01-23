---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e844c2da60babdcad5fad4a522a750bb2f013721
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418787"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="bfd40-103">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="bfd40-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="bfd40-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bfd40-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bfd40-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfd40-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bfd40-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bfd40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfd40-107">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="bfd40-107">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="bfd40-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bfd40-108">Properties</span></span>
|<span data-ttu-id="bfd40-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bfd40-109">Property</span></span>|<span data-ttu-id="bfd40-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bfd40-110">Type</span></span>|<span data-ttu-id="bfd40-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bfd40-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfd40-112">displayName</span><span class="sxs-lookup"><span data-stu-id="bfd40-112">displayName</span></span>|<span data-ttu-id="bfd40-113">Строка</span><span class="sxs-lookup"><span data-stu-id="bfd40-113">String</span></span>|<span data-ttu-id="bfd40-114">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="bfd40-114">Display name</span></span>|
|<span data-ttu-id="bfd40-115">ranges</span><span class="sxs-lookup"><span data-stu-id="bfd40-115">ranges</span></span>|<span data-ttu-id="bfd40-116">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="bfd40-116">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="bfd40-117">Коллекция диапазонов IP-адресов</span><span class="sxs-lookup"><span data-stu-id="bfd40-117">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfd40-118">Связи</span><span class="sxs-lookup"><span data-stu-id="bfd40-118">Relationships</span></span>
<span data-ttu-id="bfd40-119">Нет</span><span class="sxs-lookup"><span data-stu-id="bfd40-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bfd40-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bfd40-120">JSON Representation</span></span>
<span data-ttu-id="bfd40-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bfd40-121">Here is a JSON representation of the resource.</span></span>
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




