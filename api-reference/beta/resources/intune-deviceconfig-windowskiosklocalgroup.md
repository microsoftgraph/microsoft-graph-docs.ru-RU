---
title: Тип ресурса windowsKioskLocalGroup
description: Класс, используемый для идентификации в локальную группу для базовой конфигурации
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f9c5d467e70b4e2e7f60bc4898be35a2e9fefadc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964755"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="ccf4d-103">Тип ресурса windowsKioskLocalGroup</span><span class="sxs-lookup"><span data-stu-id="ccf4d-103">windowsKioskLocalGroup resource type</span></span>

> <span data-ttu-id="ccf4d-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ccf4d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ccf4d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccf4d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ccf4d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ccf4d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ccf4d-107">Класс, используемый для идентификации в локальную группу для базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="ccf4d-107">The class used to identify a local group for the kiosk configuration</span></span>

<span data-ttu-id="ccf4d-108">Наследуется от [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="ccf4d-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ccf4d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ccf4d-109">Properties</span></span>
|<span data-ttu-id="ccf4d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ccf4d-110">Property</span></span>|<span data-ttu-id="ccf4d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ccf4d-111">Type</span></span>|<span data-ttu-id="ccf4d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ccf4d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccf4d-113">groupName</span><span class="sxs-lookup"><span data-stu-id="ccf4d-113">groupName</span></span>|<span data-ttu-id="ccf4d-114">Строка</span><span class="sxs-lookup"><span data-stu-id="ccf4d-114">String</span></span>|<span data-ttu-id="ccf4d-115">Имя локальной группы, которая будет заблокирована этой базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="ccf4d-115">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccf4d-116">Связи</span><span class="sxs-lookup"><span data-stu-id="ccf4d-116">Relationships</span></span>
<span data-ttu-id="ccf4d-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ccf4d-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ccf4d-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ccf4d-118">JSON Representation</span></span>
<span data-ttu-id="ccf4d-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ccf4d-119">Here is a JSON representation of the resource.</span></span>
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





