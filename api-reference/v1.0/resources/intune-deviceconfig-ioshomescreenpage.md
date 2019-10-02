---
title: Тип ресурса iosHomeScreenPage
description: Страница, содержащая приложения и папки с начального экрана
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a6024ba4d097c99a7abf501b89803dba13bcb096
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359077"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="a5fec-103">Тип ресурса iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="a5fec-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="a5fec-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5fec-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5fec-105">Страница, содержащая приложения и папки с начального экрана</span><span class="sxs-lookup"><span data-stu-id="a5fec-105">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="a5fec-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5fec-106">Properties</span></span>
|<span data-ttu-id="a5fec-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5fec-107">Property</span></span>|<span data-ttu-id="a5fec-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a5fec-108">Type</span></span>|<span data-ttu-id="a5fec-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a5fec-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5fec-110">displayName</span><span class="sxs-lookup"><span data-stu-id="a5fec-110">displayName</span></span>|<span data-ttu-id="a5fec-111">String</span><span class="sxs-lookup"><span data-stu-id="a5fec-111">String</span></span>|<span data-ttu-id="a5fec-112">Имя страницы</span><span class="sxs-lookup"><span data-stu-id="a5fec-112">Name of the page</span></span>|
|<span data-ttu-id="a5fec-113">icons</span><span class="sxs-lookup"><span data-stu-id="a5fec-113">icons</span></span>|<span data-ttu-id="a5fec-114">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="a5fec-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="a5fec-115">Список приложений и папок, отображающихся на странице.</span><span class="sxs-lookup"><span data-stu-id="a5fec-115">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="a5fec-116">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a5fec-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5fec-117">Связи</span><span class="sxs-lookup"><span data-stu-id="a5fec-117">Relationships</span></span>
<span data-ttu-id="a5fec-118">Нет</span><span class="sxs-lookup"><span data-stu-id="a5fec-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5fec-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5fec-119">JSON Representation</span></span>
<span data-ttu-id="a5fec-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5fec-120">Here is a JSON representation of the resource.</span></span>
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




