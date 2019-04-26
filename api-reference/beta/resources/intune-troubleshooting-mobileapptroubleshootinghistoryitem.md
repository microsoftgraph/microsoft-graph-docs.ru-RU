---
title: Тип ресурса Мобилеапптраублешутингхисторитем
description: Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4bc87f30a970f305a309a320030cde419961660f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570070"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="a8d6e-103">Тип ресурса Мобилеапптраублешутингхисторитем</span><span class="sxs-lookup"><span data-stu-id="a8d6e-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="a8d6e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8d6e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8d6e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a8d6e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8d6e-106">Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="a8d6e-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="a8d6e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8d6e-107">Properties</span></span>
|<span data-ttu-id="a8d6e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8d6e-108">Property</span></span>|<span data-ttu-id="a8d6e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a8d6e-109">Type</span></span>|<span data-ttu-id="a8d6e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a8d6e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8d6e-111">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="a8d6e-111">occurrenceDateTime</span></span>|<span data-ttu-id="a8d6e-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8d6e-112">DateTimeOffset</span></span>|<span data-ttu-id="a8d6e-113">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="a8d6e-113">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8d6e-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="a8d6e-114">Relationships</span></span>
<span data-ttu-id="a8d6e-115">Нет</span><span class="sxs-lookup"><span data-stu-id="a8d6e-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8d6e-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8d6e-116">JSON Representation</span></span>
<span data-ttu-id="a8d6e-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8d6e-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingHistoryItem",
  "occurrenceDateTime": "String (timestamp)"
}
```



