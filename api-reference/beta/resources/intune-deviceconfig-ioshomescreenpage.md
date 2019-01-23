---
title: Тип ресурса iosHomeScreenPage
description: Страница, содержащая приложения и папки с начального экрана
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b2b6e4ba9cc70253e929a0f434a292aeafd24bd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398550"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="4395d-103">Тип ресурса iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="4395d-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="4395d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4395d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4395d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4395d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4395d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4395d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4395d-107">Страница, содержащая приложения и папки с начального экрана</span><span class="sxs-lookup"><span data-stu-id="4395d-107">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="4395d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4395d-108">Properties</span></span>
|<span data-ttu-id="4395d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4395d-109">Property</span></span>|<span data-ttu-id="4395d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4395d-110">Type</span></span>|<span data-ttu-id="4395d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4395d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4395d-112">displayName</span><span class="sxs-lookup"><span data-stu-id="4395d-112">displayName</span></span>|<span data-ttu-id="4395d-113">String</span><span class="sxs-lookup"><span data-stu-id="4395d-113">String</span></span>|<span data-ttu-id="4395d-114">Имя страницы</span><span class="sxs-lookup"><span data-stu-id="4395d-114">Name of the page</span></span>|
|<span data-ttu-id="4395d-115">icons</span><span class="sxs-lookup"><span data-stu-id="4395d-115">icons</span></span>|<span data-ttu-id="4395d-116">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="4395d-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="4395d-117">Список приложений и папок, отображающихся на странице.</span><span class="sxs-lookup"><span data-stu-id="4395d-117">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="4395d-118">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4395d-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4395d-119">Связи</span><span class="sxs-lookup"><span data-stu-id="4395d-119">Relationships</span></span>
<span data-ttu-id="4395d-120">Нет</span><span class="sxs-lookup"><span data-stu-id="4395d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4395d-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4395d-121">JSON Representation</span></span>
<span data-ttu-id="4395d-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4395d-122">Here is a JSON representation of the resource.</span></span>
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




