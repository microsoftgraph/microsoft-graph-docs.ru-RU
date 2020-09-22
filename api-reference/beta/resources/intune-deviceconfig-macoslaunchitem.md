---
title: Тип ресурса Макослаунчитем
description: Представляет приложение в списке элементов запуска macOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 098d3f14b754e87442a259ddab878196a7be6d50
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024096"
---
# <a name="macoslaunchitem-resource-type"></a><span data-ttu-id="2aba2-103">Тип ресурса Макослаунчитем</span><span class="sxs-lookup"><span data-stu-id="2aba2-103">macOSLaunchItem resource type</span></span>

<span data-ttu-id="2aba2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2aba2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2aba2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2aba2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2aba2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2aba2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2aba2-107">Представляет приложение в списке элементов запуска macOS</span><span class="sxs-lookup"><span data-stu-id="2aba2-107">Represents an app in the list of macOS launch items</span></span>

## <a name="properties"></a><span data-ttu-id="2aba2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2aba2-108">Properties</span></span>
|<span data-ttu-id="2aba2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2aba2-109">Property</span></span>|<span data-ttu-id="2aba2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2aba2-110">Type</span></span>|<span data-ttu-id="2aba2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2aba2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2aba2-112">path</span><span class="sxs-lookup"><span data-stu-id="2aba2-112">path</span></span>|<span data-ttu-id="2aba2-113">String</span><span class="sxs-lookup"><span data-stu-id="2aba2-113">String</span></span>|<span data-ttu-id="2aba2-114">Путь к запускаемому элементу.</span><span class="sxs-lookup"><span data-stu-id="2aba2-114">Path to the launch item.</span></span>|
|<span data-ttu-id="2aba2-115">скрытых</span><span class="sxs-lookup"><span data-stu-id="2aba2-115">hide</span></span>|<span data-ttu-id="2aba2-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="2aba2-116">Boolean</span></span>|<span data-ttu-id="2aba2-117">Указывает, следует ли скрыть элемент в списке "пользователи и группы".</span><span class="sxs-lookup"><span data-stu-id="2aba2-117">Whether or not to hide the item from the Users and Groups List.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2aba2-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="2aba2-118">Relationships</span></span>
<span data-ttu-id="2aba2-119">Нет</span><span class="sxs-lookup"><span data-stu-id="2aba2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2aba2-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2aba2-120">JSON Representation</span></span>
<span data-ttu-id="2aba2-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2aba2-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLaunchItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLaunchItem",
  "path": "String",
  "hide": true
}
```






