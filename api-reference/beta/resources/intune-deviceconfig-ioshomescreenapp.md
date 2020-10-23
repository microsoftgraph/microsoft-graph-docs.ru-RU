---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5de701829a622fe73680a7c5bf3108e3c1693942
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705857"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="c5422-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="c5422-103">iosHomeScreenApp resource type</span></span>

<span data-ttu-id="c5422-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5422-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5422-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5422-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5422-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5422-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5422-107">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="c5422-107">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="c5422-108">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="c5422-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c5422-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5422-109">Properties</span></span>
|<span data-ttu-id="c5422-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5422-110">Property</span></span>|<span data-ttu-id="c5422-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c5422-111">Type</span></span>|<span data-ttu-id="c5422-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c5422-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5422-113">displayName</span><span class="sxs-lookup"><span data-stu-id="c5422-113">displayName</span></span>|<span data-ttu-id="c5422-114">Строка</span><span class="sxs-lookup"><span data-stu-id="c5422-114">String</span></span>|<span data-ttu-id="c5422-115">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="c5422-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="c5422-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="c5422-116">bundleID</span></span>|<span data-ttu-id="c5422-117">String</span><span class="sxs-lookup"><span data-stu-id="c5422-117">String</span></span>|<span data-ttu-id="c5422-118">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="c5422-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5422-119">Связи</span><span class="sxs-lookup"><span data-stu-id="c5422-119">Relationships</span></span>
<span data-ttu-id="c5422-120">Нет</span><span class="sxs-lookup"><span data-stu-id="c5422-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5422-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c5422-121">JSON Representation</span></span>
<span data-ttu-id="c5422-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5422-122">Here is a JSON representation of the resource.</span></span>
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





