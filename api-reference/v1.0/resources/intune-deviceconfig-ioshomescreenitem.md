---
title: Тип ресурса iosHomeScreenItem
description: Представляет элемент на начальном экране iOS
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ff573a6f7ae0d78113a32514bc312c3920b216f1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987624"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="18e72-103">Тип ресурса iosHomeScreenItem</span><span class="sxs-lookup"><span data-stu-id="18e72-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="18e72-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="18e72-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18e72-105">Представляет элемент на начальном экране iOS</span><span class="sxs-lookup"><span data-stu-id="18e72-105">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="18e72-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="18e72-106">Properties</span></span>
|<span data-ttu-id="18e72-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="18e72-107">Property</span></span>|<span data-ttu-id="18e72-108">Тип</span><span class="sxs-lookup"><span data-stu-id="18e72-108">Type</span></span>|<span data-ttu-id="18e72-109">Описание</span><span class="sxs-lookup"><span data-stu-id="18e72-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18e72-110">displayName</span><span class="sxs-lookup"><span data-stu-id="18e72-110">displayName</span></span>|<span data-ttu-id="18e72-111">String</span><span class="sxs-lookup"><span data-stu-id="18e72-111">String</span></span>|<span data-ttu-id="18e72-112">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="18e72-112">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="18e72-113">Связи</span><span class="sxs-lookup"><span data-stu-id="18e72-113">Relationships</span></span>
<span data-ttu-id="18e72-114">Нет</span><span class="sxs-lookup"><span data-stu-id="18e72-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="18e72-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18e72-115">JSON Representation</span></span>
<span data-ttu-id="18e72-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18e72-116">Here is a JSON representation of the resource.</span></span>
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



