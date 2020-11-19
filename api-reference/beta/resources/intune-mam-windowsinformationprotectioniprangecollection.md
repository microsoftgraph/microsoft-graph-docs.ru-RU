---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e57e8024365a3209f8d60d9558f76fed454a41a8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49207241"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="8ea0c-103">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="8ea0c-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

<span data-ttu-id="8ea0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ea0c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ea0c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ea0c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ea0c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ea0c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ea0c-107">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="8ea0c-107">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="8ea0c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ea0c-108">Properties</span></span>
|<span data-ttu-id="8ea0c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ea0c-109">Property</span></span>|<span data-ttu-id="8ea0c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8ea0c-110">Type</span></span>|<span data-ttu-id="8ea0c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8ea0c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ea0c-112">displayName</span><span class="sxs-lookup"><span data-stu-id="8ea0c-112">displayName</span></span>|<span data-ttu-id="8ea0c-113">String</span><span class="sxs-lookup"><span data-stu-id="8ea0c-113">String</span></span>|<span data-ttu-id="8ea0c-114">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="8ea0c-114">Display name</span></span>|
|<span data-ttu-id="8ea0c-115">ranges</span><span class="sxs-lookup"><span data-stu-id="8ea0c-115">ranges</span></span>|<span data-ttu-id="8ea0c-116">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="8ea0c-116">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="8ea0c-117">Коллекция диапазонов IP-адресов</span><span class="sxs-lookup"><span data-stu-id="8ea0c-117">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ea0c-118">Связи</span><span class="sxs-lookup"><span data-stu-id="8ea0c-118">Relationships</span></span>
<span data-ttu-id="8ea0c-119">Нет</span><span class="sxs-lookup"><span data-stu-id="8ea0c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ea0c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ea0c-120">JSON Representation</span></span>
<span data-ttu-id="8ea0c-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ea0c-121">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.ipRange"
    }
  ]
}
```




