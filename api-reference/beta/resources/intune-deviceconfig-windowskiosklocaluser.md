---
title: Тип ресурса Виндовскиосклокалусер
description: Класс, используемый для определения локальной учетной записи для конфигурации киоска
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1c375de52d9fc294a308eb7c5b2652ef13db0c4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31777111"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="31edc-103">Тип ресурса Виндовскиосклокалусер</span><span class="sxs-lookup"><span data-stu-id="31edc-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="31edc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31edc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31edc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31edc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31edc-106">Класс, используемый для определения локальной учетной записи для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="31edc-106">The class used to identify a local account for the kiosk configuration</span></span>


<span data-ttu-id="31edc-107">НаСледуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="31edc-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="31edc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="31edc-108">Properties</span></span>
|<span data-ttu-id="31edc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="31edc-109">Property</span></span>|<span data-ttu-id="31edc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="31edc-110">Type</span></span>|<span data-ttu-id="31edc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="31edc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31edc-112">userName</span><span class="sxs-lookup"><span data-stu-id="31edc-112">userName</span></span>|<span data-ttu-id="31edc-113">String</span><span class="sxs-lookup"><span data-stu-id="31edc-113">String</span></span>|<span data-ttu-id="31edc-114">Локальный пользователь, который будет заблокирован для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="31edc-114">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="31edc-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="31edc-115">Relationships</span></span>
<span data-ttu-id="31edc-116">Нет</span><span class="sxs-lookup"><span data-stu-id="31edc-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="31edc-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31edc-117">JSON Representation</span></span>
<span data-ttu-id="31edc-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31edc-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalUser",
  "userName": "String"
}
```





