---
title: Тип ресурса iosHomeScreenFolderPage
description: Папка, содержащая приложения с начального экрана
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 38b1d898cb4bc1eacaa427ed412b536ba40cd0f9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941963"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="ad7a3-103">Тип ресурса iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="ad7a3-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="ad7a3-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ad7a3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad7a3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad7a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad7a3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ad7a3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad7a3-107">Папка, содержащая приложения с начального экрана</span><span class="sxs-lookup"><span data-stu-id="ad7a3-107">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="ad7a3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad7a3-108">Properties</span></span>
|<span data-ttu-id="ad7a3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad7a3-109">Property</span></span>|<span data-ttu-id="ad7a3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ad7a3-110">Type</span></span>|<span data-ttu-id="ad7a3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ad7a3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad7a3-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ad7a3-112">displayName</span></span>|<span data-ttu-id="ad7a3-113">String</span><span class="sxs-lookup"><span data-stu-id="ad7a3-113">String</span></span>|<span data-ttu-id="ad7a3-114">Имя страницы папки</span><span class="sxs-lookup"><span data-stu-id="ad7a3-114">Name of the folder page</span></span>|
|<span data-ttu-id="ad7a3-115">apps</span><span class="sxs-lookup"><span data-stu-id="ad7a3-115">apps</span></span>|<span data-ttu-id="ad7a3-116">Коллекция [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="ad7a3-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="ad7a3-117">Список приложений, которые отображаются на странице в папке.</span><span class="sxs-lookup"><span data-stu-id="ad7a3-117">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="ad7a3-118">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ad7a3-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad7a3-119">Связи</span><span class="sxs-lookup"><span data-stu-id="ad7a3-119">Relationships</span></span>
<span data-ttu-id="ad7a3-120">Нет</span><span class="sxs-lookup"><span data-stu-id="ad7a3-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ad7a3-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad7a3-121">JSON Representation</span></span>
<span data-ttu-id="ad7a3-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad7a3-122">Here is a JSON representation of the resource.</span></span>
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





