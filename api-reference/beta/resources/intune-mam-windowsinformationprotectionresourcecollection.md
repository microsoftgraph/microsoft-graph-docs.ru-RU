---
title: Тип ресурса windowsInformationProtectionResourceCollection
description: Коллекция ресурсов Windows Information Protection
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f7d6fad5c2367ace676b67ec6f44f7ca3b082d27
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42780341"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="a24bb-103">Тип ресурса windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="a24bb-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="a24bb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a24bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a24bb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a24bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a24bb-106">Коллекция ресурсов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="a24bb-106">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="a24bb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a24bb-107">Properties</span></span>
|<span data-ttu-id="a24bb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a24bb-108">Property</span></span>|<span data-ttu-id="a24bb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a24bb-109">Type</span></span>|<span data-ttu-id="a24bb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a24bb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a24bb-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a24bb-111">displayName</span></span>|<span data-ttu-id="a24bb-112">String</span><span class="sxs-lookup"><span data-stu-id="a24bb-112">String</span></span>|<span data-ttu-id="a24bb-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="a24bb-113">Display name</span></span>|
|<span data-ttu-id="a24bb-114">resources</span><span class="sxs-lookup"><span data-stu-id="a24bb-114">resources</span></span>|<span data-ttu-id="a24bb-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a24bb-115">String collection</span></span>|<span data-ttu-id="a24bb-116">Коллекция ресурсов</span><span class="sxs-lookup"><span data-stu-id="a24bb-116">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="a24bb-117">Связи</span><span class="sxs-lookup"><span data-stu-id="a24bb-117">Relationships</span></span>
<span data-ttu-id="a24bb-118">Нет</span><span class="sxs-lookup"><span data-stu-id="a24bb-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a24bb-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a24bb-119">JSON Representation</span></span>
<span data-ttu-id="a24bb-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a24bb-120">Here is a JSON representation of the resource.</span></span>
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



