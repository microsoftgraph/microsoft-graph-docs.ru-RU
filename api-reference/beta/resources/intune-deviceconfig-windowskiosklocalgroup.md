---
title: Тип ресурса Виндовскиосклокалграуп
description: Класс, используемый для идентификации локальной группы для конфигурации киоска
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3479226d770c7030fefed1a7f2f65a02808479d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169526"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="c9325-103">Тип ресурса Виндовскиосклокалграуп</span><span class="sxs-lookup"><span data-stu-id="c9325-103">windowsKioskLocalGroup resource type</span></span>

> <span data-ttu-id="c9325-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9325-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9325-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9325-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9325-106">Класс, используемый для идентификации локальной группы для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="c9325-106">The class used to identify a local group for the kiosk configuration</span></span>


<span data-ttu-id="c9325-107">НаСледуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="c9325-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c9325-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c9325-108">Properties</span></span>
|<span data-ttu-id="c9325-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9325-109">Property</span></span>|<span data-ttu-id="c9325-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c9325-110">Type</span></span>|<span data-ttu-id="c9325-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c9325-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9325-112">groupName</span><span class="sxs-lookup"><span data-stu-id="c9325-112">groupName</span></span>|<span data-ttu-id="c9325-113">String</span><span class="sxs-lookup"><span data-stu-id="c9325-113">String</span></span>|<span data-ttu-id="c9325-114">Имя локальной группы, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="c9325-114">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9325-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="c9325-115">Relationships</span></span>
<span data-ttu-id="c9325-116">Нет</span><span class="sxs-lookup"><span data-stu-id="c9325-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9325-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c9325-117">JSON Representation</span></span>
<span data-ttu-id="c9325-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9325-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalGroup",
  "groupName": "String"
}
```




