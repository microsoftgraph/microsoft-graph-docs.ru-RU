---
title: Тип ресурса windowsInformationProtectionResourceCollection
description: Коллекция ресурсов Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74d7549f57ecc59f70aa1af4350544ec21b156ec
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254823"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="4489e-103">Тип ресурса windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="4489e-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="4489e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4489e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4489e-105">Коллекция ресурсов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="4489e-105">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="4489e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4489e-106">Properties</span></span>
|<span data-ttu-id="4489e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4489e-107">Property</span></span>|<span data-ttu-id="4489e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4489e-108">Type</span></span>|<span data-ttu-id="4489e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4489e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4489e-110">displayName</span><span class="sxs-lookup"><span data-stu-id="4489e-110">displayName</span></span>|<span data-ttu-id="4489e-111">Строка</span><span class="sxs-lookup"><span data-stu-id="4489e-111">String</span></span>|<span data-ttu-id="4489e-112">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="4489e-112">Display name</span></span>|
|<span data-ttu-id="4489e-113">resources</span><span class="sxs-lookup"><span data-stu-id="4489e-113">resources</span></span>|<span data-ttu-id="4489e-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4489e-114">String collection</span></span>|<span data-ttu-id="4489e-115">Коллекция ресурсов</span><span class="sxs-lookup"><span data-stu-id="4489e-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="4489e-116">Связи</span><span class="sxs-lookup"><span data-stu-id="4489e-116">Relationships</span></span>
<span data-ttu-id="4489e-117">Нет</span><span class="sxs-lookup"><span data-stu-id="4489e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4489e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4489e-118">JSON Representation</span></span>
<span data-ttu-id="4489e-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4489e-119">Here is a JSON representation of the resource.</span></span>
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



