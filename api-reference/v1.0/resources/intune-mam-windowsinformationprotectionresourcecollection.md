---
title: Тип ресурса windowsInformationProtectionResourceCollection
description: Коллекция ресурсов Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0df0ebc3c67e7cf9bc18240f75d620442f80e0d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844354"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="59841-103">Тип ресурса windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="59841-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="59841-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="59841-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59841-105">Коллекция ресурсов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="59841-105">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="59841-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="59841-106">Properties</span></span>
|<span data-ttu-id="59841-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="59841-107">Property</span></span>|<span data-ttu-id="59841-108">Тип</span><span class="sxs-lookup"><span data-stu-id="59841-108">Type</span></span>|<span data-ttu-id="59841-109">Описание</span><span class="sxs-lookup"><span data-stu-id="59841-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59841-110">displayName</span><span class="sxs-lookup"><span data-stu-id="59841-110">displayName</span></span>|<span data-ttu-id="59841-111">Строка</span><span class="sxs-lookup"><span data-stu-id="59841-111">String</span></span>|<span data-ttu-id="59841-112">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="59841-112">Display name</span></span>|
|<span data-ttu-id="59841-113">resources</span><span class="sxs-lookup"><span data-stu-id="59841-113">resources</span></span>|<span data-ttu-id="59841-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="59841-114">String collection</span></span>|<span data-ttu-id="59841-115">Коллекция ресурсов</span><span class="sxs-lookup"><span data-stu-id="59841-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="59841-116">Связи</span><span class="sxs-lookup"><span data-stu-id="59841-116">Relationships</span></span>
<span data-ttu-id="59841-117">Нет</span><span class="sxs-lookup"><span data-stu-id="59841-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="59841-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59841-118">JSON Representation</span></span>
<span data-ttu-id="59841-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59841-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```



