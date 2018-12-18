---
title: Тип ресурса iosHomeScreenFolderPage
description: Папка, содержащая приложения с начального экрана
author: tfitzmac
ms.openlocfilehash: fc5f1899a9eadf88a1815558ed9c1dc9eff51114
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340637"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="b9a43-103">Тип ресурса iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="b9a43-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="b9a43-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b9a43-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9a43-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9a43-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9a43-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b9a43-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9a43-107">Папка, содержащая приложения с начального экрана</span><span class="sxs-lookup"><span data-stu-id="b9a43-107">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="b9a43-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9a43-108">Properties</span></span>
|<span data-ttu-id="b9a43-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9a43-109">Property</span></span>|<span data-ttu-id="b9a43-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b9a43-110">Type</span></span>|<span data-ttu-id="b9a43-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b9a43-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9a43-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b9a43-112">displayName</span></span>|<span data-ttu-id="b9a43-113">String</span><span class="sxs-lookup"><span data-stu-id="b9a43-113">String</span></span>|<span data-ttu-id="b9a43-114">Имя страницы папки</span><span class="sxs-lookup"><span data-stu-id="b9a43-114">Name of the folder page</span></span>|
|<span data-ttu-id="b9a43-115">apps</span><span class="sxs-lookup"><span data-stu-id="b9a43-115">apps</span></span>|<span data-ttu-id="b9a43-116">Коллекция [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="b9a43-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="b9a43-117">Список приложений, которые отображаются на странице в папке.</span><span class="sxs-lookup"><span data-stu-id="b9a43-117">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="b9a43-118">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="b9a43-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9a43-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b9a43-119">Relationships</span></span>
<span data-ttu-id="b9a43-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b9a43-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b9a43-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b9a43-121">JSON Representation</span></span>
<span data-ttu-id="b9a43-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9a43-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "displayName": "String",
      "bundleID": "String"
    }
  ]
}
```





