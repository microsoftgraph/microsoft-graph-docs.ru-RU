---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d991ba74a269b9feaf52d8bdd5bc7ea4b2c65469
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443688"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="7a2e1-103">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="7a2e1-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

<span data-ttu-id="7a2e1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a2e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a2e1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a2e1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a2e1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a2e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a2e1-107">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="7a2e1-107">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="7a2e1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a2e1-108">Properties</span></span>
|<span data-ttu-id="7a2e1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a2e1-109">Property</span></span>|<span data-ttu-id="7a2e1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7a2e1-110">Type</span></span>|<span data-ttu-id="7a2e1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7a2e1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a2e1-112">displayName</span><span class="sxs-lookup"><span data-stu-id="7a2e1-112">displayName</span></span>|<span data-ttu-id="7a2e1-113">String</span><span class="sxs-lookup"><span data-stu-id="7a2e1-113">String</span></span>|<span data-ttu-id="7a2e1-114">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="7a2e1-114">Display name</span></span>|
|<span data-ttu-id="7a2e1-115">ranges</span><span class="sxs-lookup"><span data-stu-id="7a2e1-115">ranges</span></span>|<span data-ttu-id="7a2e1-116">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="7a2e1-116">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="7a2e1-117">Коллекция диапазонов IP-адресов</span><span class="sxs-lookup"><span data-stu-id="7a2e1-117">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a2e1-118">Связи</span><span class="sxs-lookup"><span data-stu-id="7a2e1-118">Relationships</span></span>
<span data-ttu-id="7a2e1-119">Нет</span><span class="sxs-lookup"><span data-stu-id="7a2e1-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a2e1-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7a2e1-120">JSON Representation</span></span>
<span data-ttu-id="7a2e1-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a2e1-121">Here is a JSON representation of the resource.</span></span>
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



