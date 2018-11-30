---
title: Тип ресурса iosHomeScreenItem
description: Представляет элемент на начальном экране iOS
ms.openlocfilehash: 705849569dd91d339633e52187d16dfdd25b5ab3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080120"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="05862-103">Тип ресурса iosHomeScreenItem</span><span class="sxs-lookup"><span data-stu-id="05862-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="05862-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="05862-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05862-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05862-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05862-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="05862-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05862-107">Представляет элемент на начальном экране iOS</span><span class="sxs-lookup"><span data-stu-id="05862-107">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="05862-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="05862-108">Properties</span></span>
|<span data-ttu-id="05862-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="05862-109">Property</span></span>|<span data-ttu-id="05862-110">Тип</span><span class="sxs-lookup"><span data-stu-id="05862-110">Type</span></span>|<span data-ttu-id="05862-111">Описание</span><span class="sxs-lookup"><span data-stu-id="05862-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05862-112">displayName</span><span class="sxs-lookup"><span data-stu-id="05862-112">displayName</span></span>|<span data-ttu-id="05862-113">String</span><span class="sxs-lookup"><span data-stu-id="05862-113">String</span></span>|<span data-ttu-id="05862-114">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="05862-114">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="05862-115">Связи</span><span class="sxs-lookup"><span data-stu-id="05862-115">Relationships</span></span>
<span data-ttu-id="05862-116">Нет</span><span class="sxs-lookup"><span data-stu-id="05862-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="05862-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05862-117">JSON Representation</span></span>
<span data-ttu-id="05862-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05862-118">Here is a JSON representation of the resource.</span></span>
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





