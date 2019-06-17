---
title: Тип ресурса Макослаунчитем
description: Представляет приложение в списке элементов запуска macOS
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2752abd8d76c08e1da162d58aa8863d2f8b63940
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992124"
---
# <a name="macoslaunchitem-resource-type"></a><span data-ttu-id="b941f-103">Тип ресурса Макослаунчитем</span><span class="sxs-lookup"><span data-stu-id="b941f-103">macOSLaunchItem resource type</span></span>

> <span data-ttu-id="b941f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b941f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b941f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b941f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b941f-106">Представляет приложение в списке элементов запуска macOS</span><span class="sxs-lookup"><span data-stu-id="b941f-106">Represents an app in the list of macOS launch items</span></span>

## <a name="properties"></a><span data-ttu-id="b941f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b941f-107">Properties</span></span>
|<span data-ttu-id="b941f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b941f-108">Property</span></span>|<span data-ttu-id="b941f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b941f-109">Type</span></span>|<span data-ttu-id="b941f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b941f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b941f-111">path</span><span class="sxs-lookup"><span data-stu-id="b941f-111">path</span></span>|<span data-ttu-id="b941f-112">String</span><span class="sxs-lookup"><span data-stu-id="b941f-112">String</span></span>|<span data-ttu-id="b941f-113">Путь к запускаемому элементу.</span><span class="sxs-lookup"><span data-stu-id="b941f-113">Path to the launch item.</span></span>|
|<span data-ttu-id="b941f-114">скрытых</span><span class="sxs-lookup"><span data-stu-id="b941f-114">hide</span></span>|<span data-ttu-id="b941f-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="b941f-115">Boolean</span></span>|<span data-ttu-id="b941f-116">Указывает, следует ли скрыть элемент в списке "пользователи и группы".</span><span class="sxs-lookup"><span data-stu-id="b941f-116">Whether or not to hide the item from the Users and Groups List.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b941f-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="b941f-117">Relationships</span></span>
<span data-ttu-id="b941f-118">Нет</span><span class="sxs-lookup"><span data-stu-id="b941f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b941f-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b941f-119">JSON Representation</span></span>
<span data-ttu-id="b941f-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b941f-120">Here is a JSON representation of the resource.</span></span>
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





