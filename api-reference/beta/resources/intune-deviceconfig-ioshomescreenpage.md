---
title: Тип ресурса iosHomeScreenPage
description: Страница, содержащая приложения и папки с начального экрана
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a59c910f37a82e04a7ccd5050a0a03999ac567b7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961038"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="8a6da-103">Тип ресурса iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="8a6da-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="8a6da-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8a6da-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a6da-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a6da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8a6da-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8a6da-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a6da-107">Страница, содержащая приложения и папки с начального экрана</span><span class="sxs-lookup"><span data-stu-id="8a6da-107">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="8a6da-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a6da-108">Properties</span></span>
|<span data-ttu-id="8a6da-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a6da-109">Property</span></span>|<span data-ttu-id="8a6da-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8a6da-110">Type</span></span>|<span data-ttu-id="8a6da-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8a6da-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a6da-112">displayName</span><span class="sxs-lookup"><span data-stu-id="8a6da-112">displayName</span></span>|<span data-ttu-id="8a6da-113">String</span><span class="sxs-lookup"><span data-stu-id="8a6da-113">String</span></span>|<span data-ttu-id="8a6da-114">Имя страницы</span><span class="sxs-lookup"><span data-stu-id="8a6da-114">Name of the page</span></span>|
|<span data-ttu-id="8a6da-115">icons</span><span class="sxs-lookup"><span data-stu-id="8a6da-115">icons</span></span>|<span data-ttu-id="8a6da-116">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="8a6da-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="8a6da-117">Список приложений и папок, отображающихся на странице.</span><span class="sxs-lookup"><span data-stu-id="8a6da-117">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="8a6da-118">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="8a6da-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a6da-119">Связи</span><span class="sxs-lookup"><span data-stu-id="8a6da-119">Relationships</span></span>
<span data-ttu-id="8a6da-120">Нет</span><span class="sxs-lookup"><span data-stu-id="8a6da-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8a6da-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a6da-121">JSON Representation</span></span>
<span data-ttu-id="8a6da-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a6da-122">Here is a JSON representation of the resource.</span></span>
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





