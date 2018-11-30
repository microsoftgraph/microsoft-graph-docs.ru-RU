---
title: Тип ресурса iosHomeScreenPage
description: Страница, содержащая приложения и папки с начального экрана
ms.openlocfilehash: 4ef336bc104a203739904b67e301b489627e7ff1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025988"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="e421c-103">Тип ресурса iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="e421c-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="e421c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e421c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e421c-105">Страница, содержащая приложения и папки с начального экрана</span><span class="sxs-lookup"><span data-stu-id="e421c-105">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="e421c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e421c-106">Properties</span></span>
|<span data-ttu-id="e421c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e421c-107">Property</span></span>|<span data-ttu-id="e421c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e421c-108">Type</span></span>|<span data-ttu-id="e421c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e421c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e421c-110">displayName</span><span class="sxs-lookup"><span data-stu-id="e421c-110">displayName</span></span>|<span data-ttu-id="e421c-111">String</span><span class="sxs-lookup"><span data-stu-id="e421c-111">String</span></span>|<span data-ttu-id="e421c-112">Имя страницы</span><span class="sxs-lookup"><span data-stu-id="e421c-112">Name of the page</span></span>|
|<span data-ttu-id="e421c-113">icons</span><span class="sxs-lookup"><span data-stu-id="e421c-113">icons</span></span>|<span data-ttu-id="e421c-114">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="e421c-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="e421c-115">Список приложений и папок, отображающихся на странице.</span><span class="sxs-lookup"><span data-stu-id="e421c-115">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="e421c-116">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e421c-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e421c-117">Связи</span><span class="sxs-lookup"><span data-stu-id="e421c-117">Relationships</span></span>
<span data-ttu-id="e421c-118">Нет</span><span class="sxs-lookup"><span data-stu-id="e421c-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e421c-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e421c-119">JSON Representation</span></span>
<span data-ttu-id="e421c-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e421c-120">Here is a JSON representation of the resource.</span></span>
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



