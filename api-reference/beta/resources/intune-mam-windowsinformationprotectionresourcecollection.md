---
title: Тип ресурса windowsInformationProtectionResourceCollection
description: Коллекция ресурсов Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbeb58464ccfd7aff3dfc6066ab276a2bd73f5c6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149751"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="7e982-103">Тип ресурса windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="7e982-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="7e982-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e982-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e982-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7e982-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e982-106">Коллекция ресурсов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="7e982-106">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="7e982-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e982-107">Properties</span></span>
|<span data-ttu-id="7e982-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e982-108">Property</span></span>|<span data-ttu-id="7e982-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7e982-109">Type</span></span>|<span data-ttu-id="7e982-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7e982-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e982-111">displayName</span><span class="sxs-lookup"><span data-stu-id="7e982-111">displayName</span></span>|<span data-ttu-id="7e982-112">Строка</span><span class="sxs-lookup"><span data-stu-id="7e982-112">String</span></span>|<span data-ttu-id="7e982-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="7e982-113">Display name</span></span>|
|<span data-ttu-id="7e982-114">resources</span><span class="sxs-lookup"><span data-stu-id="7e982-114">resources</span></span>|<span data-ttu-id="7e982-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7e982-115">String collection</span></span>|<span data-ttu-id="7e982-116">Коллекция ресурсов</span><span class="sxs-lookup"><span data-stu-id="7e982-116">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e982-117">Связи</span><span class="sxs-lookup"><span data-stu-id="7e982-117">Relationships</span></span>
<span data-ttu-id="7e982-118">Нет</span><span class="sxs-lookup"><span data-stu-id="7e982-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e982-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e982-119">JSON Representation</span></span>
<span data-ttu-id="7e982-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e982-120">Here is a JSON representation of the resource.</span></span>
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




