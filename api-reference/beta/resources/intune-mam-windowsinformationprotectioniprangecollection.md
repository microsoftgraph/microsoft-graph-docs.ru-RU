---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b894318bb0b56bb2e5fc86e47a677dd9709e1092
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524253"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="5b157-103">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="5b157-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

<span data-ttu-id="5b157-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5b157-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b157-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b157-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b157-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b157-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b157-107">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="5b157-107">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="5b157-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b157-108">Properties</span></span>
|<span data-ttu-id="5b157-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b157-109">Property</span></span>|<span data-ttu-id="5b157-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5b157-110">Type</span></span>|<span data-ttu-id="5b157-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5b157-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b157-112">displayName</span><span class="sxs-lookup"><span data-stu-id="5b157-112">displayName</span></span>|<span data-ttu-id="5b157-113">String</span><span class="sxs-lookup"><span data-stu-id="5b157-113">String</span></span>|<span data-ttu-id="5b157-114">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="5b157-114">Display name</span></span>|
|<span data-ttu-id="5b157-115">ranges</span><span class="sxs-lookup"><span data-stu-id="5b157-115">ranges</span></span>|<span data-ttu-id="5b157-116">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="5b157-116">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="5b157-117">Коллекция диапазонов IP-адресов</span><span class="sxs-lookup"><span data-stu-id="5b157-117">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b157-118">Связи</span><span class="sxs-lookup"><span data-stu-id="5b157-118">Relationships</span></span>
<span data-ttu-id="5b157-119">Нет</span><span class="sxs-lookup"><span data-stu-id="5b157-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b157-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5b157-120">JSON Representation</span></span>
<span data-ttu-id="5b157-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b157-121">Here is a JSON representation of the resource.</span></span>
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



