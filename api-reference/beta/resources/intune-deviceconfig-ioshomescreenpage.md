---
title: Тип ресурса iosHomeScreenPage
description: Страница, содержащая приложения и папки с начального экрана
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db8ca7082544bc9ffe517cad9fee1ab453ebc0fa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993856"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="30b72-103">Тип ресурса iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="30b72-103">iosHomeScreenPage resource type</span></span>

<span data-ttu-id="30b72-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30b72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30b72-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30b72-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30b72-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30b72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30b72-107">Страница, содержащая приложения и папки с начального экрана</span><span class="sxs-lookup"><span data-stu-id="30b72-107">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="30b72-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="30b72-108">Properties</span></span>
|<span data-ttu-id="30b72-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="30b72-109">Property</span></span>|<span data-ttu-id="30b72-110">Тип</span><span class="sxs-lookup"><span data-stu-id="30b72-110">Type</span></span>|<span data-ttu-id="30b72-111">Описание</span><span class="sxs-lookup"><span data-stu-id="30b72-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30b72-112">displayName</span><span class="sxs-lookup"><span data-stu-id="30b72-112">displayName</span></span>|<span data-ttu-id="30b72-113">String</span><span class="sxs-lookup"><span data-stu-id="30b72-113">String</span></span>|<span data-ttu-id="30b72-114">Имя страницы</span><span class="sxs-lookup"><span data-stu-id="30b72-114">Name of the page</span></span>|
|<span data-ttu-id="30b72-115">icons</span><span class="sxs-lookup"><span data-stu-id="30b72-115">icons</span></span>|<span data-ttu-id="30b72-116">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="30b72-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="30b72-117">Список приложений и папок, отображающихся на странице.</span><span class="sxs-lookup"><span data-stu-id="30b72-117">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="30b72-118">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="30b72-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30b72-119">Связи</span><span class="sxs-lookup"><span data-stu-id="30b72-119">Relationships</span></span>
<span data-ttu-id="30b72-120">Нет</span><span class="sxs-lookup"><span data-stu-id="30b72-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="30b72-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="30b72-121">JSON Representation</span></span>
<span data-ttu-id="30b72-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30b72-122">Here is a JSON representation of the resource.</span></span>
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






