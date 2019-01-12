---
title: Тип ресурса iosHomeScreenPage
description: Страница, содержащая приложения и папки с начального экрана
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9787a88c28d410f4961657738236d6a27a6621ca
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925947"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="577d1-103">Тип ресурса iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="577d1-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="577d1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="577d1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="577d1-105">Страница, содержащая приложения и папки с начального экрана</span><span class="sxs-lookup"><span data-stu-id="577d1-105">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="577d1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="577d1-106">Properties</span></span>
|<span data-ttu-id="577d1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="577d1-107">Property</span></span>|<span data-ttu-id="577d1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="577d1-108">Type</span></span>|<span data-ttu-id="577d1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="577d1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="577d1-110">displayName</span><span class="sxs-lookup"><span data-stu-id="577d1-110">displayName</span></span>|<span data-ttu-id="577d1-111">String</span><span class="sxs-lookup"><span data-stu-id="577d1-111">String</span></span>|<span data-ttu-id="577d1-112">Имя страницы</span><span class="sxs-lookup"><span data-stu-id="577d1-112">Name of the page</span></span>|
|<span data-ttu-id="577d1-113">icons</span><span class="sxs-lookup"><span data-stu-id="577d1-113">icons</span></span>|<span data-ttu-id="577d1-114">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="577d1-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="577d1-115">Список приложений и папок, отображающихся на странице.</span><span class="sxs-lookup"><span data-stu-id="577d1-115">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="577d1-116">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="577d1-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="577d1-117">Связи</span><span class="sxs-lookup"><span data-stu-id="577d1-117">Relationships</span></span>
<span data-ttu-id="577d1-118">Нет</span><span class="sxs-lookup"><span data-stu-id="577d1-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="577d1-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="577d1-119">JSON Representation</span></span>
<span data-ttu-id="577d1-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="577d1-120">Here is a JSON representation of the resource.</span></span>
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



