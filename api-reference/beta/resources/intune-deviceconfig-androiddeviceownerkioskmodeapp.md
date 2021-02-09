---
title: Тип ресурса androidDeviceOwnerKioskModeApp
description: Приложение на управляемом домашнем экране владельца устройства Android
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da6adb416c8fd20406c295e56a5d15177e625c30
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161028"
---
# <a name="androiddeviceownerkioskmodeapp-resource-type"></a><span data-ttu-id="228e9-103">Тип ресурса androidDeviceOwnerKioskModeApp</span><span class="sxs-lookup"><span data-stu-id="228e9-103">androidDeviceOwnerKioskModeApp resource type</span></span>

<span data-ttu-id="228e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="228e9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="228e9-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="228e9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="228e9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="228e9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="228e9-107">Приложение на управляемом домашнем экране владельца устройства Android</span><span class="sxs-lookup"><span data-stu-id="228e9-107">An application on the Android Device Owner Managed Home Screen</span></span>


<span data-ttu-id="228e9-108">Наследуется [от androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)</span><span class="sxs-lookup"><span data-stu-id="228e9-108">Inherits from [androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="228e9-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="228e9-109">Properties</span></span>
|<span data-ttu-id="228e9-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="228e9-110">Property</span></span>|<span data-ttu-id="228e9-111">Тип</span><span class="sxs-lookup"><span data-stu-id="228e9-111">Type</span></span>|<span data-ttu-id="228e9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="228e9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="228e9-113">package</span><span class="sxs-lookup"><span data-stu-id="228e9-113">package</span></span>|<span data-ttu-id="228e9-114">String</span><span class="sxs-lookup"><span data-stu-id="228e9-114">String</span></span>|<span data-ttu-id="228e9-115">Имя пакета приложения</span><span class="sxs-lookup"><span data-stu-id="228e9-115">Package name of application</span></span>|
|<span data-ttu-id="228e9-116">className</span><span class="sxs-lookup"><span data-stu-id="228e9-116">className</span></span>|<span data-ttu-id="228e9-117">String</span><span class="sxs-lookup"><span data-stu-id="228e9-117">String</span></span>|<span data-ttu-id="228e9-118">Имя класса приложения</span><span class="sxs-lookup"><span data-stu-id="228e9-118">Class name of application</span></span>|

## <a name="relationships"></a><span data-ttu-id="228e9-119">Связи</span><span class="sxs-lookup"><span data-stu-id="228e9-119">Relationships</span></span>
<span data-ttu-id="228e9-120">Нет</span><span class="sxs-lookup"><span data-stu-id="228e9-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="228e9-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="228e9-121">JSON Representation</span></span>
<span data-ttu-id="228e9-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="228e9-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeApp",
  "package": "String",
  "className": "String"
}
```




