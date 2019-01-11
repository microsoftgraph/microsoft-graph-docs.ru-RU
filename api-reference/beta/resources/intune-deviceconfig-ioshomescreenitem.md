---
title: Тип ресурса iosHomeScreenItem
description: Представляет элемент на начальном экране iOS
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cc351025f81931ac7deb33bec9be973a513a51fb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809956"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="e731a-103">Тип ресурса iosHomeScreenItem</span><span class="sxs-lookup"><span data-stu-id="e731a-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="e731a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e731a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e731a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e731a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e731a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e731a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e731a-107">Представляет элемент на начальном экране iOS</span><span class="sxs-lookup"><span data-stu-id="e731a-107">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="e731a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e731a-108">Properties</span></span>
|<span data-ttu-id="e731a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e731a-109">Property</span></span>|<span data-ttu-id="e731a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e731a-110">Type</span></span>|<span data-ttu-id="e731a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e731a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e731a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e731a-112">displayName</span></span>|<span data-ttu-id="e731a-113">String</span><span class="sxs-lookup"><span data-stu-id="e731a-113">String</span></span>|<span data-ttu-id="e731a-114">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="e731a-114">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="e731a-115">Связи</span><span class="sxs-lookup"><span data-stu-id="e731a-115">Relationships</span></span>
<span data-ttu-id="e731a-116">Нет</span><span class="sxs-lookup"><span data-stu-id="e731a-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e731a-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e731a-117">JSON Representation</span></span>
<span data-ttu-id="e731a-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e731a-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```





