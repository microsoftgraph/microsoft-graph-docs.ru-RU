---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c26f1237061914e66653509cd22b734fef854f27
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993919"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="d9a6b-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="d9a6b-103">iosHomeScreenApp resource type</span></span>

<span data-ttu-id="d9a6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9a6b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9a6b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9a6b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9a6b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9a6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9a6b-107">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="d9a6b-107">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="d9a6b-108">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="d9a6b-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d9a6b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9a6b-109">Properties</span></span>
|<span data-ttu-id="d9a6b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9a6b-110">Property</span></span>|<span data-ttu-id="d9a6b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d9a6b-111">Type</span></span>|<span data-ttu-id="d9a6b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d9a6b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9a6b-113">displayName</span><span class="sxs-lookup"><span data-stu-id="d9a6b-113">displayName</span></span>|<span data-ttu-id="d9a6b-114">String</span><span class="sxs-lookup"><span data-stu-id="d9a6b-114">String</span></span>|<span data-ttu-id="d9a6b-115">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="d9a6b-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="d9a6b-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="d9a6b-116">bundleID</span></span>|<span data-ttu-id="d9a6b-117">String</span><span class="sxs-lookup"><span data-stu-id="d9a6b-117">String</span></span>|<span data-ttu-id="d9a6b-118">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="d9a6b-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9a6b-119">Связи</span><span class="sxs-lookup"><span data-stu-id="d9a6b-119">Relationships</span></span>
<span data-ttu-id="d9a6b-120">Нет</span><span class="sxs-lookup"><span data-stu-id="d9a6b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9a6b-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9a6b-121">JSON Representation</span></span>
<span data-ttu-id="d9a6b-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9a6b-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```






