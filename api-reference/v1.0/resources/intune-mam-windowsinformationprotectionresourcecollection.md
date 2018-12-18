---
title: Тип ресурса windowsInformationProtectionResourceCollection
description: Коллекция ресурсов Windows Information Protection
author: tfitzmac
ms.openlocfilehash: 8e037ff53e11566aee7d79d2c3bbe5b1075b83a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327834"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="7dcf8-103">Тип ресурса windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="7dcf8-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="7dcf8-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7dcf8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7dcf8-105">Коллекция ресурсов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="7dcf8-105">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="7dcf8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7dcf8-106">Properties</span></span>
|<span data-ttu-id="7dcf8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7dcf8-107">Property</span></span>|<span data-ttu-id="7dcf8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7dcf8-108">Type</span></span>|<span data-ttu-id="7dcf8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7dcf8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dcf8-110">displayName</span><span class="sxs-lookup"><span data-stu-id="7dcf8-110">displayName</span></span>|<span data-ttu-id="7dcf8-111">Строка</span><span class="sxs-lookup"><span data-stu-id="7dcf8-111">String</span></span>|<span data-ttu-id="7dcf8-112">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="7dcf8-112">Display name</span></span>|
|<span data-ttu-id="7dcf8-113">resources</span><span class="sxs-lookup"><span data-stu-id="7dcf8-113">resources</span></span>|<span data-ttu-id="7dcf8-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7dcf8-114">String collection</span></span>|<span data-ttu-id="7dcf8-115">Коллекция ресурсов</span><span class="sxs-lookup"><span data-stu-id="7dcf8-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="7dcf8-116">Связи</span><span class="sxs-lookup"><span data-stu-id="7dcf8-116">Relationships</span></span>
<span data-ttu-id="7dcf8-117">Нет</span><span class="sxs-lookup"><span data-stu-id="7dcf8-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7dcf8-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7dcf8-118">JSON Representation</span></span>
<span data-ttu-id="7dcf8-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7dcf8-119">Here is a JSON representation of the resource.</span></span>
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



