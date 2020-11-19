---
title: Тип ресурса iosHomeScreenPage
description: Страница, содержащая приложения и папки с начального экрана
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 124c457cdbda94fae86dfcfc43a2119e61fb156a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280370"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="e970a-103">Тип ресурса iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="e970a-103">iosHomeScreenPage resource type</span></span>

<span data-ttu-id="e970a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e970a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e970a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e970a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e970a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e970a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e970a-107">Страница, содержащая приложения и папки с начального экрана</span><span class="sxs-lookup"><span data-stu-id="e970a-107">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="e970a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e970a-108">Properties</span></span>
|<span data-ttu-id="e970a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e970a-109">Property</span></span>|<span data-ttu-id="e970a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e970a-110">Type</span></span>|<span data-ttu-id="e970a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e970a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e970a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e970a-112">displayName</span></span>|<span data-ttu-id="e970a-113">String</span><span class="sxs-lookup"><span data-stu-id="e970a-113">String</span></span>|<span data-ttu-id="e970a-114">Имя страницы</span><span class="sxs-lookup"><span data-stu-id="e970a-114">Name of the page</span></span>|
|<span data-ttu-id="e970a-115">icons</span><span class="sxs-lookup"><span data-stu-id="e970a-115">icons</span></span>|<span data-ttu-id="e970a-116">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="e970a-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="e970a-117">Список приложений и папок, отображающихся на странице.</span><span class="sxs-lookup"><span data-stu-id="e970a-117">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="e970a-118">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e970a-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e970a-119">Связи</span><span class="sxs-lookup"><span data-stu-id="e970a-119">Relationships</span></span>
<span data-ttu-id="e970a-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e970a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e970a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e970a-121">JSON Representation</span></span>
<span data-ttu-id="e970a-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e970a-122">Here is a JSON representation of the resource.</span></span>
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




