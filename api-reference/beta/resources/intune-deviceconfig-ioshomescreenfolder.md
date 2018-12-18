---
title: Тип ресурса iosHomeScreenFolder
description: Папка, содержащая страницы приложений на начальном экране
author: tfitzmac
ms.openlocfilehash: 983337c4376bb6212607630f96008a2c8a36b22b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306694"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="d7d72-103">Тип ресурса iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="d7d72-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="d7d72-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d7d72-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7d72-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7d72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d7d72-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d7d72-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7d72-107">Папка, содержащая страницы приложений на начальном экране</span><span class="sxs-lookup"><span data-stu-id="d7d72-107">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="d7d72-108">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="d7d72-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d7d72-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7d72-109">Properties</span></span>
|<span data-ttu-id="d7d72-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7d72-110">Property</span></span>|<span data-ttu-id="d7d72-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d7d72-111">Type</span></span>|<span data-ttu-id="d7d72-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d7d72-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7d72-113">displayName</span><span class="sxs-lookup"><span data-stu-id="d7d72-113">displayName</span></span>|<span data-ttu-id="d7d72-114">String</span><span class="sxs-lookup"><span data-stu-id="d7d72-114">String</span></span>|<span data-ttu-id="d7d72-115">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="d7d72-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="d7d72-116">pages</span><span class="sxs-lookup"><span data-stu-id="d7d72-116">pages</span></span>|<span data-ttu-id="d7d72-117">Коллекция [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="d7d72-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="d7d72-118">Страницы значков на начальном экране, которые должны относиться к типу приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d72-118">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="d7d72-119">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="d7d72-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7d72-120">Связи</span><span class="sxs-lookup"><span data-stu-id="d7d72-120">Relationships</span></span>
<span data-ttu-id="d7d72-121">Нет</span><span class="sxs-lookup"><span data-stu-id="d7d72-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d7d72-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d7d72-122">JSON Representation</span></span>
<span data-ttu-id="d7d72-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7d72-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
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
```





