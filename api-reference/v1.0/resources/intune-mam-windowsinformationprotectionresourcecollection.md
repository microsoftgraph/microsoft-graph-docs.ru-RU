---
title: Тип ресурса windowsInformationProtectionResourceCollection
description: Коллекция ресурсов Windows Information Protection
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c28c63abd02cea9b0e8c883220ad2f1dafefd916
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755723"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="ad280-103">Тип ресурса windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="ad280-103">windowsInformationProtectionResourceCollection resource type</span></span>

<span data-ttu-id="ad280-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad280-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ad280-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad280-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad280-106">Коллекция ресурсов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="ad280-106">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="ad280-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad280-107">Properties</span></span>
|<span data-ttu-id="ad280-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad280-108">Property</span></span>|<span data-ttu-id="ad280-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ad280-109">Type</span></span>|<span data-ttu-id="ad280-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ad280-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad280-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ad280-111">displayName</span></span>|<span data-ttu-id="ad280-112">String</span><span class="sxs-lookup"><span data-stu-id="ad280-112">String</span></span>|<span data-ttu-id="ad280-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="ad280-113">Display name</span></span>|
|<span data-ttu-id="ad280-114">resources</span><span class="sxs-lookup"><span data-stu-id="ad280-114">resources</span></span>|<span data-ttu-id="ad280-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ad280-115">String collection</span></span>|<span data-ttu-id="ad280-116">Коллекция ресурсов</span><span class="sxs-lookup"><span data-stu-id="ad280-116">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad280-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="ad280-117">Relationships</span></span>
<span data-ttu-id="ad280-118">Нет</span><span class="sxs-lookup"><span data-stu-id="ad280-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad280-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad280-119">JSON Representation</span></span>
<span data-ttu-id="ad280-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad280-120">Here is a JSON representation of the resource.</span></span>
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




