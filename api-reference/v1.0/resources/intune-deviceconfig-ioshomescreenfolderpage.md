---
title: Тип ресурса iosHomeScreenFolderPage
description: Страница для папки, содержащей приложения и веб-клипы на домашнем экране.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9a8fc93d365dc842886f3346b86ff632f3ced7cb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760066"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="e962c-103">Тип ресурса iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="e962c-103">iosHomeScreenFolderPage resource type</span></span>

<span data-ttu-id="e962c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e962c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e962c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e962c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e962c-106">Страница для папки, содержащей приложения и веб-клипы на домашнем экране.</span><span class="sxs-lookup"><span data-stu-id="e962c-106">A page for a folder containing apps and web clips on the Home Screen.</span></span>

## <a name="properties"></a><span data-ttu-id="e962c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e962c-107">Properties</span></span>
|<span data-ttu-id="e962c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e962c-108">Property</span></span>|<span data-ttu-id="e962c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e962c-109">Type</span></span>|<span data-ttu-id="e962c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e962c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e962c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e962c-111">displayName</span></span>|<span data-ttu-id="e962c-112">String</span><span class="sxs-lookup"><span data-stu-id="e962c-112">String</span></span>|<span data-ttu-id="e962c-113">Имя страницы папки</span><span class="sxs-lookup"><span data-stu-id="e962c-113">Name of the folder page</span></span>|
|<span data-ttu-id="e962c-114">apps</span><span class="sxs-lookup"><span data-stu-id="e962c-114">apps</span></span>|<span data-ttu-id="e962c-115">Коллекция [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="e962c-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="e962c-116">Список приложений и веб-клипов, которые будут отображаться на странице в папке.</span><span class="sxs-lookup"><span data-stu-id="e962c-116">A list of apps and web clips to appear on a page within a folder.</span></span> <span data-ttu-id="e962c-117">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e962c-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e962c-118">Связи</span><span class="sxs-lookup"><span data-stu-id="e962c-118">Relationships</span></span>
<span data-ttu-id="e962c-119">Нет</span><span class="sxs-lookup"><span data-stu-id="e962c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e962c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e962c-120">JSON Representation</span></span>
<span data-ttu-id="e962c-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e962c-121">Here is a JSON representation of the resource.</span></span>
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
      "bundleID": "String"
    }
  ]
}
```




