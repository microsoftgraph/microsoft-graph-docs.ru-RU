---
title: Тип ресурса iosHomeScreenFolderPage
description: Страница для папки, содержащей приложения и веб-клипы на домашнем экране.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 45a26205e6a4f03639984e2a72632bb8bfb5a332
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161812"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="6b02f-103">Тип ресурса iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="6b02f-103">iosHomeScreenFolderPage resource type</span></span>

<span data-ttu-id="6b02f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b02f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b02f-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b02f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b02f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b02f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b02f-107">Страница для папки, содержащей приложения и веб-клипы на домашнем экране.</span><span class="sxs-lookup"><span data-stu-id="6b02f-107">A page for a folder containing apps and web clips on the Home Screen.</span></span>

## <a name="properties"></a><span data-ttu-id="6b02f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b02f-108">Properties</span></span>
|<span data-ttu-id="6b02f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b02f-109">Property</span></span>|<span data-ttu-id="6b02f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6b02f-110">Type</span></span>|<span data-ttu-id="6b02f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6b02f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b02f-112">displayName</span><span class="sxs-lookup"><span data-stu-id="6b02f-112">displayName</span></span>|<span data-ttu-id="6b02f-113">String</span><span class="sxs-lookup"><span data-stu-id="6b02f-113">String</span></span>|<span data-ttu-id="6b02f-114">Имя страницы папки</span><span class="sxs-lookup"><span data-stu-id="6b02f-114">Name of the folder page</span></span>|
|<span data-ttu-id="6b02f-115">apps</span><span class="sxs-lookup"><span data-stu-id="6b02f-115">apps</span></span>|<span data-ttu-id="6b02f-116">Коллекция [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b02f-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="6b02f-117">Список приложений и веб-клипов, которые должны отображаться на странице в папке.</span><span class="sxs-lookup"><span data-stu-id="6b02f-117">A list of apps and web clips to appear on a page within a folder.</span></span> <span data-ttu-id="6b02f-118">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6b02f-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b02f-119">Связи</span><span class="sxs-lookup"><span data-stu-id="6b02f-119">Relationships</span></span>
<span data-ttu-id="6b02f-120">Нет</span><span class="sxs-lookup"><span data-stu-id="6b02f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b02f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b02f-121">JSON Representation</span></span>
<span data-ttu-id="6b02f-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b02f-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "displayName": "String",
      "bundleID": "String",
      "isWebClip": true
    }
  ]
}
```




