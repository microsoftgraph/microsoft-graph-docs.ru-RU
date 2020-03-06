---
title: Тип ресурса iosHomeScreenPage
description: Страница, содержащая приложения и папки с начального экрана
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: abe09741cd3ed4f25f417cbb99cd144d6105acba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532489"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="f11c7-103">Тип ресурса iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="f11c7-103">iosHomeScreenPage resource type</span></span>

<span data-ttu-id="f11c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f11c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f11c7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f11c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f11c7-106">Страница, содержащая приложения и папки с начального экрана</span><span class="sxs-lookup"><span data-stu-id="f11c7-106">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="f11c7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f11c7-107">Properties</span></span>
|<span data-ttu-id="f11c7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f11c7-108">Property</span></span>|<span data-ttu-id="f11c7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f11c7-109">Type</span></span>|<span data-ttu-id="f11c7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f11c7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f11c7-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f11c7-111">displayName</span></span>|<span data-ttu-id="f11c7-112">Строка</span><span class="sxs-lookup"><span data-stu-id="f11c7-112">String</span></span>|<span data-ttu-id="f11c7-113">Имя страницы</span><span class="sxs-lookup"><span data-stu-id="f11c7-113">Name of the page</span></span>|
|<span data-ttu-id="f11c7-114">icons</span><span class="sxs-lookup"><span data-stu-id="f11c7-114">icons</span></span>|<span data-ttu-id="f11c7-115">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="f11c7-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="f11c7-116">Список приложений и папок, отображающихся на странице.</span><span class="sxs-lookup"><span data-stu-id="f11c7-116">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="f11c7-117">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f11c7-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f11c7-118">Связи</span><span class="sxs-lookup"><span data-stu-id="f11c7-118">Relationships</span></span>
<span data-ttu-id="f11c7-119">Нет</span><span class="sxs-lookup"><span data-stu-id="f11c7-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f11c7-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f11c7-120">JSON Representation</span></span>
<span data-ttu-id="f11c7-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f11c7-121">Here is a JSON representation of the resource.</span></span>
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




