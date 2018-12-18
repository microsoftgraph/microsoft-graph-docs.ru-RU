---
title: Тип ресурса windowsKioskLocalGroup
description: Класс, используемый для идентификации в локальную группу для базовой конфигурации
author: tfitzmac
ms.openlocfilehash: bb2e0cddd1c9b2530e1f146e966d707466c737d1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306848"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="73766-103">Тип ресурса windowsKioskLocalGroup</span><span class="sxs-lookup"><span data-stu-id="73766-103">windowsKioskLocalGroup resource type</span></span>

> <span data-ttu-id="73766-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="73766-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73766-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73766-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73766-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="73766-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73766-107">Класс, используемый для идентификации в локальную группу для базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="73766-107">The class used to identify a local group for the kiosk configuration</span></span>

<span data-ttu-id="73766-108">Наследуется от [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="73766-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="73766-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="73766-109">Properties</span></span>
|<span data-ttu-id="73766-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="73766-110">Property</span></span>|<span data-ttu-id="73766-111">Тип</span><span class="sxs-lookup"><span data-stu-id="73766-111">Type</span></span>|<span data-ttu-id="73766-112">Описание</span><span class="sxs-lookup"><span data-stu-id="73766-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73766-113">groupName</span><span class="sxs-lookup"><span data-stu-id="73766-113">groupName</span></span>|<span data-ttu-id="73766-114">String.</span><span class="sxs-lookup"><span data-stu-id="73766-114">String</span></span>|<span data-ttu-id="73766-115">Имя локальной группы, которая будет заблокирована этой базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="73766-115">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="73766-116">Связи</span><span class="sxs-lookup"><span data-stu-id="73766-116">Relationships</span></span>
<span data-ttu-id="73766-117">Нет</span><span class="sxs-lookup"><span data-stu-id="73766-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="73766-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="73766-118">JSON Representation</span></span>
<span data-ttu-id="73766-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73766-119">Here is a JSON representation of the resource.</span></span>
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





