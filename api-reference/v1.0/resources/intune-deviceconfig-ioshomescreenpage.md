---
title: Тип ресурса iosHomeScreenPage
description: Страница, содержащая приложения, папки и веб-клипы на домашнем экране.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9bc9880f63bc27ce4cdab44b128d6d373e348fb1
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760052"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="1244a-103">Тип ресурса iosHomeScreenPage</span><span class="sxs-lookup"><span data-stu-id="1244a-103">iosHomeScreenPage resource type</span></span>

<span data-ttu-id="1244a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1244a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1244a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1244a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1244a-106">Страница, содержащая приложения, папки и веб-клипы на домашнем экране.</span><span class="sxs-lookup"><span data-stu-id="1244a-106">A page containing apps, folders, and web clips on the Home Screen.</span></span>

## <a name="properties"></a><span data-ttu-id="1244a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1244a-107">Properties</span></span>
|<span data-ttu-id="1244a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1244a-108">Property</span></span>|<span data-ttu-id="1244a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1244a-109">Type</span></span>|<span data-ttu-id="1244a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1244a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1244a-111">displayName</span><span class="sxs-lookup"><span data-stu-id="1244a-111">displayName</span></span>|<span data-ttu-id="1244a-112">String</span><span class="sxs-lookup"><span data-stu-id="1244a-112">String</span></span>|<span data-ttu-id="1244a-113">Имя страницы</span><span class="sxs-lookup"><span data-stu-id="1244a-113">Name of the page</span></span>|
|<span data-ttu-id="1244a-114">icons</span><span class="sxs-lookup"><span data-stu-id="1244a-114">icons</span></span>|<span data-ttu-id="1244a-115">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="1244a-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="1244a-116">Список приложений, папок и веб-клипов, которые будут отображаться на странице.</span><span class="sxs-lookup"><span data-stu-id="1244a-116">A list of apps, folders, and web clips to appear on a page.</span></span> <span data-ttu-id="1244a-117">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="1244a-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1244a-118">Связи</span><span class="sxs-lookup"><span data-stu-id="1244a-118">Relationships</span></span>
<span data-ttu-id="1244a-119">Нет</span><span class="sxs-lookup"><span data-stu-id="1244a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1244a-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1244a-120">JSON Representation</span></span>
<span data-ttu-id="1244a-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1244a-121">Here is a JSON representation of the resource.</span></span>
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




