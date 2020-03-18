---
title: Тип ресурса Макослаунчитем
description: Представляет приложение в списке элементов запуска macOS
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 378b2e3f510d8d0db082e3843ea2588e5a5e161d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42789208"
---
# <a name="macoslaunchitem-resource-type"></a><span data-ttu-id="15891-103">Тип ресурса Макослаунчитем</span><span class="sxs-lookup"><span data-stu-id="15891-103">macOSLaunchItem resource type</span></span>

> <span data-ttu-id="15891-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15891-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15891-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15891-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15891-106">Представляет приложение в списке элементов запуска macOS</span><span class="sxs-lookup"><span data-stu-id="15891-106">Represents an app in the list of macOS launch items</span></span>

## <a name="properties"></a><span data-ttu-id="15891-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="15891-107">Properties</span></span>
|<span data-ttu-id="15891-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="15891-108">Property</span></span>|<span data-ttu-id="15891-109">Тип</span><span class="sxs-lookup"><span data-stu-id="15891-109">Type</span></span>|<span data-ttu-id="15891-110">Описание</span><span class="sxs-lookup"><span data-stu-id="15891-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15891-111">path</span><span class="sxs-lookup"><span data-stu-id="15891-111">path</span></span>|<span data-ttu-id="15891-112">String</span><span class="sxs-lookup"><span data-stu-id="15891-112">String</span></span>|<span data-ttu-id="15891-113">Путь к запускаемому элементу.</span><span class="sxs-lookup"><span data-stu-id="15891-113">Path to the launch item.</span></span>|
|<span data-ttu-id="15891-114">скрытых</span><span class="sxs-lookup"><span data-stu-id="15891-114">hide</span></span>|<span data-ttu-id="15891-115">Логический</span><span class="sxs-lookup"><span data-stu-id="15891-115">Boolean</span></span>|<span data-ttu-id="15891-116">Указывает, следует ли скрыть элемент в списке "пользователи и группы".</span><span class="sxs-lookup"><span data-stu-id="15891-116">Whether or not to hide the item from the Users and Groups List.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15891-117">Связи</span><span class="sxs-lookup"><span data-stu-id="15891-117">Relationships</span></span>
<span data-ttu-id="15891-118">Нет</span><span class="sxs-lookup"><span data-stu-id="15891-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15891-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15891-119">JSON Representation</span></span>
<span data-ttu-id="15891-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15891-120">Here is a JSON representation of the resource.</span></span>
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



