---
title: Тип ресурса Мобилеапптраублешутингдевицечеккинхистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0fe4799e2be8d87a2c4d79a8552870e37d051ef9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371287"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="f058a-103">Тип ресурса Мобилеапптраублешутингдевицечеккинхистори</span><span class="sxs-lookup"><span data-stu-id="f058a-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="f058a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f058a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f058a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f058a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f058a-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="f058a-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="f058a-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="f058a-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f058a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f058a-108">Properties</span></span>
|<span data-ttu-id="f058a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f058a-109">Property</span></span>|<span data-ttu-id="f058a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f058a-110">Type</span></span>|<span data-ttu-id="f058a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f058a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f058a-112">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="f058a-112">occurrenceDateTime</span></span>|<span data-ttu-id="f058a-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f058a-113">DateTimeOffset</span></span>|<span data-ttu-id="f058a-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="f058a-114">Time when the history item occurred.</span></span> <span data-ttu-id="f058a-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="f058a-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="f058a-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="f058a-116">Relationships</span></span>
<span data-ttu-id="f058a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="f058a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f058a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f058a-118">JSON Representation</span></span>
<span data-ttu-id="f058a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f058a-119">Here is a JSON representation of the resource.</span></span>
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



