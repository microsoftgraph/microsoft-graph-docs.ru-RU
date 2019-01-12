---
title: Тип ресурса iosHomeScreenItem
description: Представляет элемент на начальном экране iOS
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 477be5c509ab4d062a695c4b8df7eb00af6f51fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962606"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="19ef7-103">Тип ресурса iosHomeScreenItem</span><span class="sxs-lookup"><span data-stu-id="19ef7-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="19ef7-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="19ef7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19ef7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19ef7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19ef7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="19ef7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19ef7-107">Представляет элемент на начальном экране iOS</span><span class="sxs-lookup"><span data-stu-id="19ef7-107">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="19ef7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="19ef7-108">Properties</span></span>
|<span data-ttu-id="19ef7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="19ef7-109">Property</span></span>|<span data-ttu-id="19ef7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="19ef7-110">Type</span></span>|<span data-ttu-id="19ef7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="19ef7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19ef7-112">displayName</span><span class="sxs-lookup"><span data-stu-id="19ef7-112">displayName</span></span>|<span data-ttu-id="19ef7-113">String</span><span class="sxs-lookup"><span data-stu-id="19ef7-113">String</span></span>|<span data-ttu-id="19ef7-114">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="19ef7-114">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="19ef7-115">Связи</span><span class="sxs-lookup"><span data-stu-id="19ef7-115">Relationships</span></span>
<span data-ttu-id="19ef7-116">Нет</span><span class="sxs-lookup"><span data-stu-id="19ef7-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="19ef7-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19ef7-117">JSON Representation</span></span>
<span data-ttu-id="19ef7-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19ef7-118">Here is a JSON representation of the resource.</span></span>
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





