---
title: Тип ресурса windowsKioskLocalGroup
description: Класс, используемый для идентификации в локальную группу для базовой конфигурации
ms.openlocfilehash: 456460e60bbf21130fc918f38922893e5430abe8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075287"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="c0527-103">Тип ресурса windowsKioskLocalGroup</span><span class="sxs-lookup"><span data-stu-id="c0527-103">windowsKioskLocalGroup resource type</span></span>

> <span data-ttu-id="c0527-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c0527-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0527-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0527-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0527-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c0527-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0527-107">Класс, используемый для идентификации в локальную группу для базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="c0527-107">The class used to identify a local group for the kiosk configuration</span></span>

<span data-ttu-id="c0527-108">Наследуется от [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="c0527-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c0527-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0527-109">Properties</span></span>
|<span data-ttu-id="c0527-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0527-110">Property</span></span>|<span data-ttu-id="c0527-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c0527-111">Type</span></span>|<span data-ttu-id="c0527-112">Description</span><span class="sxs-lookup"><span data-stu-id="c0527-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0527-113">groupName</span><span class="sxs-lookup"><span data-stu-id="c0527-113">groupName</span></span>|<span data-ttu-id="c0527-114">String</span><span class="sxs-lookup"><span data-stu-id="c0527-114">String</span></span>|<span data-ttu-id="c0527-115">Имя локальной группы, которая будет заблокирована этой базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="c0527-115">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0527-116">Связи</span><span class="sxs-lookup"><span data-stu-id="c0527-116">Relationships</span></span>
<span data-ttu-id="c0527-117">Нет</span><span class="sxs-lookup"><span data-stu-id="c0527-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c0527-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0527-118">JSON Representation</span></span>
<span data-ttu-id="c0527-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0527-119">Here is a JSON representation of the resource.</span></span>
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





