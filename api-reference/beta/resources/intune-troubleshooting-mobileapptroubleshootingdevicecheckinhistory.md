---
title: Тип ресурса Мобилеапптраублешутингдевицечеккинхистори
description: Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f8bbcbd3b8291b16fa1cae1eb7c4b3fba30baf6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784861"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="b2e48-103">Тип ресурса Мобилеапптраублешутингдевицечеккинхистори</span><span class="sxs-lookup"><span data-stu-id="b2e48-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="b2e48-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2e48-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2e48-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2e48-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2e48-106">Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="b2e48-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="b2e48-107">НаСледуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="b2e48-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b2e48-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2e48-108">Properties</span></span>
|<span data-ttu-id="b2e48-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2e48-109">Property</span></span>|<span data-ttu-id="b2e48-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b2e48-110">Type</span></span>|<span data-ttu-id="b2e48-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b2e48-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2e48-112">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="b2e48-112">occurrenceDateTime</span></span>|<span data-ttu-id="b2e48-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2e48-113">DateTimeOffset</span></span>|<span data-ttu-id="b2e48-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="b2e48-114">Time when the history item occurred.</span></span> <span data-ttu-id="b2e48-115">НаСледуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="b2e48-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2e48-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="b2e48-116">Relationships</span></span>
<span data-ttu-id="b2e48-117">Нет</span><span class="sxs-lookup"><span data-stu-id="b2e48-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2e48-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2e48-118">JSON Representation</span></span>
<span data-ttu-id="b2e48-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2e48-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory",
  "occurrenceDateTime": "String (timestamp)"
}
```



