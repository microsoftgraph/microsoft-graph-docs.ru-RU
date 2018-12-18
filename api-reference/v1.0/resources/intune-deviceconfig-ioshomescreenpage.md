---
title: Тип ресурса iosHomeScreenPage
description: Страница, содержащая приложения и папки с начального экрана
author: tfitzmac
ms.openlocfilehash: b8aca5c671d0c8521cdf8a870a2f0ad3cd35ba1b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321464"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="f0bb6-103">Тип ресурса iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="f0bb6-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="f0bb6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f0bb6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0bb6-105">Страница, содержащая приложения и папки с начального экрана</span><span class="sxs-lookup"><span data-stu-id="f0bb6-105">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="f0bb6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0bb6-106">Properties</span></span>
|<span data-ttu-id="f0bb6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0bb6-107">Property</span></span>|<span data-ttu-id="f0bb6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f0bb6-108">Type</span></span>|<span data-ttu-id="f0bb6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f0bb6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0bb6-110">displayName</span><span class="sxs-lookup"><span data-stu-id="f0bb6-110">displayName</span></span>|<span data-ttu-id="f0bb6-111">String</span><span class="sxs-lookup"><span data-stu-id="f0bb6-111">String</span></span>|<span data-ttu-id="f0bb6-112">Имя страницы</span><span class="sxs-lookup"><span data-stu-id="f0bb6-112">Name of the page</span></span>|
|<span data-ttu-id="f0bb6-113">icons</span><span class="sxs-lookup"><span data-stu-id="f0bb6-113">icons</span></span>|<span data-ttu-id="f0bb6-114">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="f0bb6-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="f0bb6-115">Список приложений и папок, отображающихся на странице.</span><span class="sxs-lookup"><span data-stu-id="f0bb6-115">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="f0bb6-116">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f0bb6-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0bb6-117">Связи</span><span class="sxs-lookup"><span data-stu-id="f0bb6-117">Relationships</span></span>
<span data-ttu-id="f0bb6-118">Нет</span><span class="sxs-lookup"><span data-stu-id="f0bb6-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f0bb6-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0bb6-119">JSON Representation</span></span>
<span data-ttu-id="f0bb6-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0bb6-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenPage",
  "displayName": "String",
  "icons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenItem",
      "displayName": "String",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "String",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "String",
              "bundleID": "String"
            }
          ]
        }
      ]
    }
  ]
}
```



