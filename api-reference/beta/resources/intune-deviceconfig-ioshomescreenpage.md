---
title: Тип ресурса iosHomeScreenPage
description: Страница, содержащая приложения и папки с начального экрана
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c958570caa81cff7add1e174cbb678fc68cecd87
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149541"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="a8d47-103">Тип ресурса iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="a8d47-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="a8d47-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8d47-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8d47-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a8d47-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8d47-106">Страница, содержащая приложения и папки с начального экрана</span><span class="sxs-lookup"><span data-stu-id="a8d47-106">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="a8d47-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8d47-107">Properties</span></span>
|<span data-ttu-id="a8d47-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8d47-108">Property</span></span>|<span data-ttu-id="a8d47-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a8d47-109">Type</span></span>|<span data-ttu-id="a8d47-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a8d47-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8d47-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a8d47-111">displayName</span></span>|<span data-ttu-id="a8d47-112">String</span><span class="sxs-lookup"><span data-stu-id="a8d47-112">String</span></span>|<span data-ttu-id="a8d47-113">Имя страницы</span><span class="sxs-lookup"><span data-stu-id="a8d47-113">Name of the page</span></span>|
|<span data-ttu-id="a8d47-114">icons</span><span class="sxs-lookup"><span data-stu-id="a8d47-114">icons</span></span>|<span data-ttu-id="a8d47-115">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="a8d47-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="a8d47-116">Список приложений и папок, отображающихся на странице.</span><span class="sxs-lookup"><span data-stu-id="a8d47-116">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="a8d47-117">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a8d47-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8d47-118">Связи</span><span class="sxs-lookup"><span data-stu-id="a8d47-118">Relationships</span></span>
<span data-ttu-id="a8d47-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a8d47-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8d47-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8d47-120">JSON Representation</span></span>
<span data-ttu-id="a8d47-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8d47-121">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
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




