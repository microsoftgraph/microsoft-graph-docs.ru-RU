---
title: Тип ресурса Мобилеапптраублешутингдевицечеккинхистори
description: Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f8bbcbd3b8291b16fa1cae1eb7c4b3fba30baf6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570028"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="45ddd-103">Тип ресурса Мобилеапптраублешутингдевицечеккинхистори</span><span class="sxs-lookup"><span data-stu-id="45ddd-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="45ddd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45ddd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45ddd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45ddd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45ddd-106">Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="45ddd-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="45ddd-107">НаСледуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="45ddd-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="45ddd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="45ddd-108">Properties</span></span>
|<span data-ttu-id="45ddd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="45ddd-109">Property</span></span>|<span data-ttu-id="45ddd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="45ddd-110">Type</span></span>|<span data-ttu-id="45ddd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="45ddd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45ddd-112">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="45ddd-112">occurrenceDateTime</span></span>|<span data-ttu-id="45ddd-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45ddd-113">DateTimeOffset</span></span>|<span data-ttu-id="45ddd-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="45ddd-114">Time when the history item occurred.</span></span> <span data-ttu-id="45ddd-115">НаСледуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="45ddd-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="45ddd-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="45ddd-116">Relationships</span></span>
<span data-ttu-id="45ddd-117">Нет</span><span class="sxs-lookup"><span data-stu-id="45ddd-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45ddd-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45ddd-118">JSON Representation</span></span>
<span data-ttu-id="45ddd-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45ddd-119">Here is a JSON representation of the resource.</span></span>
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



