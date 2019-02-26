---
title: Тип ресурса iosHomeScreenPage
description: Страница, содержащая приложения и папки с начального экрана
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4317ac80e7ff6273b809eb747da745f5cf5edb6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254389"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="11e81-103">Тип ресурса iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="11e81-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="11e81-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11e81-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11e81-105">Страница, содержащая приложения и папки с начального экрана</span><span class="sxs-lookup"><span data-stu-id="11e81-105">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="11e81-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="11e81-106">Properties</span></span>
|<span data-ttu-id="11e81-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="11e81-107">Property</span></span>|<span data-ttu-id="11e81-108">Тип</span><span class="sxs-lookup"><span data-stu-id="11e81-108">Type</span></span>|<span data-ttu-id="11e81-109">Описание</span><span class="sxs-lookup"><span data-stu-id="11e81-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11e81-110">displayName</span><span class="sxs-lookup"><span data-stu-id="11e81-110">displayName</span></span>|<span data-ttu-id="11e81-111">String</span><span class="sxs-lookup"><span data-stu-id="11e81-111">String</span></span>|<span data-ttu-id="11e81-112">Имя страницы</span><span class="sxs-lookup"><span data-stu-id="11e81-112">Name of the page</span></span>|
|<span data-ttu-id="11e81-113">icons</span><span class="sxs-lookup"><span data-stu-id="11e81-113">icons</span></span>|<span data-ttu-id="11e81-114">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="11e81-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="11e81-115">Список приложений и папок, отображающихся на странице.</span><span class="sxs-lookup"><span data-stu-id="11e81-115">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="11e81-116">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="11e81-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11e81-117">Связи</span><span class="sxs-lookup"><span data-stu-id="11e81-117">Relationships</span></span>
<span data-ttu-id="11e81-118">Нет</span><span class="sxs-lookup"><span data-stu-id="11e81-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11e81-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11e81-119">JSON Representation</span></span>
<span data-ttu-id="11e81-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11e81-120">Here is a JSON representation of the resource.</span></span>
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



