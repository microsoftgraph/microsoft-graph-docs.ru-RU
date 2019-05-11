---
title: Тип ресурса iosHomeScreenPage
description: Страница, содержащая приложения и папки с начального экрана
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 570dcf430824601383ba9348b721df7862f6eef6
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946548"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="65622-103">Тип ресурса iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="65622-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="65622-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65622-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65622-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="65622-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65622-106">Страница, содержащая приложения и папки с начального экрана</span><span class="sxs-lookup"><span data-stu-id="65622-106">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="65622-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="65622-107">Properties</span></span>
|<span data-ttu-id="65622-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="65622-108">Property</span></span>|<span data-ttu-id="65622-109">Тип</span><span class="sxs-lookup"><span data-stu-id="65622-109">Type</span></span>|<span data-ttu-id="65622-110">Описание</span><span class="sxs-lookup"><span data-stu-id="65622-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65622-111">displayName</span><span class="sxs-lookup"><span data-stu-id="65622-111">displayName</span></span>|<span data-ttu-id="65622-112">Строка</span><span class="sxs-lookup"><span data-stu-id="65622-112">String</span></span>|<span data-ttu-id="65622-113">Имя страницы</span><span class="sxs-lookup"><span data-stu-id="65622-113">Name of the page</span></span>|
|<span data-ttu-id="65622-114">icons</span><span class="sxs-lookup"><span data-stu-id="65622-114">icons</span></span>|<span data-ttu-id="65622-115">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="65622-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="65622-116">Список приложений и папок, отображающихся на странице.</span><span class="sxs-lookup"><span data-stu-id="65622-116">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="65622-117">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="65622-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65622-118">Связи</span><span class="sxs-lookup"><span data-stu-id="65622-118">Relationships</span></span>
<span data-ttu-id="65622-119">Нет</span><span class="sxs-lookup"><span data-stu-id="65622-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65622-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65622-120">JSON Representation</span></span>
<span data-ttu-id="65622-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65622-121">Here is a JSON representation of the resource.</span></span>
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




