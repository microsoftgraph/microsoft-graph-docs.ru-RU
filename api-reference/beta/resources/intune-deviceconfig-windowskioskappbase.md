---
title: Тип ресурса windowsKioskAppBase
description: Базовый класс для типов приложений
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fa83243959105b09707fa28a53271d8f95c5fd1f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845159"
---
# <a name="windowskioskappbase-resource-type"></a><span data-ttu-id="eb016-103">Тип ресурса windowsKioskAppBase</span><span class="sxs-lookup"><span data-stu-id="eb016-103">windowsKioskAppBase resource type</span></span>

> <span data-ttu-id="eb016-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eb016-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb016-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb016-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eb016-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="eb016-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb016-107">Базовый класс для типов приложений</span><span class="sxs-lookup"><span data-stu-id="eb016-107">The base class for a type of apps</span></span>
## <a name="properties"></a><span data-ttu-id="eb016-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb016-108">Properties</span></span>
|<span data-ttu-id="eb016-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb016-109">Property</span></span>|<span data-ttu-id="eb016-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eb016-110">Type</span></span>|<span data-ttu-id="eb016-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eb016-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb016-112">startLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="eb016-112">startLayoutTileSize</span></span>|[<span data-ttu-id="eb016-113">windowsAppStartLayoutTileSize</span><span class="sxs-lookup"><span data-stu-id="eb016-113">windowsAppStartLayoutTileSize</span></span>](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|<span data-ttu-id="eb016-114">Размер плитку приложение для макета Пуск.</span><span class="sxs-lookup"><span data-stu-id="eb016-114">The app tile size for the start layout.</span></span> <span data-ttu-id="eb016-115">Возможные значения: `hidden`, `small`, `medium`, `wide`, `large`.</span><span class="sxs-lookup"><span data-stu-id="eb016-115">Possible values are: `hidden`, `small`, `medium`, `wide`, `large`.</span></span>|
|<span data-ttu-id="eb016-116">name</span><span class="sxs-lookup"><span data-stu-id="eb016-116">name</span></span>|<span data-ttu-id="eb016-117">Строка</span><span class="sxs-lookup"><span data-stu-id="eb016-117">String</span></span>|<span data-ttu-id="eb016-118">Представляет понятное имя приложения</span><span class="sxs-lookup"><span data-stu-id="eb016-118">Represents the friendly name of an app</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb016-119">Связи</span><span class="sxs-lookup"><span data-stu-id="eb016-119">Relationships</span></span>
<span data-ttu-id="eb016-120">Нет</span><span class="sxs-lookup"><span data-stu-id="eb016-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eb016-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb016-121">JSON Representation</span></span>
<span data-ttu-id="eb016-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb016-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAppBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAppBase",
  "startLayoutTileSize": "String",
  "name": "String"
}
```





