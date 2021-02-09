---
title: Тип ресурса androidDeviceOwnerKioskModeWeblink
description: Веб-связь на управляемом домашнем экране владельца устройства Android
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 076e1fc6630856ff937bf85396c70e4461fda2b1
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162555"
---
# <a name="androiddeviceownerkioskmodeweblink-resource-type"></a><span data-ttu-id="47a1d-103">Тип ресурса androidDeviceOwnerKioskModeWeblink</span><span class="sxs-lookup"><span data-stu-id="47a1d-103">androidDeviceOwnerKioskModeWeblink resource type</span></span>

<span data-ttu-id="47a1d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47a1d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47a1d-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47a1d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47a1d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47a1d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47a1d-107">Веб-связь на управляемом домашнем экране владельца устройства Android</span><span class="sxs-lookup"><span data-stu-id="47a1d-107">A weblink on the Android Device Owner Managed Home Screen</span></span>


<span data-ttu-id="47a1d-108">Наследуется [от androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)</span><span class="sxs-lookup"><span data-stu-id="47a1d-108">Inherits from [androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="47a1d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="47a1d-109">Properties</span></span>
|<span data-ttu-id="47a1d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="47a1d-110">Property</span></span>|<span data-ttu-id="47a1d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="47a1d-111">Type</span></span>|<span data-ttu-id="47a1d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="47a1d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47a1d-113">label</span><span class="sxs-lookup"><span data-stu-id="47a1d-113">label</span></span>|<span data-ttu-id="47a1d-114">String</span><span class="sxs-lookup"><span data-stu-id="47a1d-114">String</span></span>|<span data-ttu-id="47a1d-115">Отображаемая имя для веб-ссылки</span><span class="sxs-lookup"><span data-stu-id="47a1d-115">Display name for weblink</span></span>|
|<span data-ttu-id="47a1d-116">ссылка</span><span class="sxs-lookup"><span data-stu-id="47a1d-116">link</span></span>|<span data-ttu-id="47a1d-117">String</span><span class="sxs-lookup"><span data-stu-id="47a1d-117">String</span></span>|<span data-ttu-id="47a1d-118">Ссылка для веб-ссылки</span><span class="sxs-lookup"><span data-stu-id="47a1d-118">Link for weblink</span></span>|

## <a name="relationships"></a><span data-ttu-id="47a1d-119">Связи</span><span class="sxs-lookup"><span data-stu-id="47a1d-119">Relationships</span></span>
<span data-ttu-id="47a1d-120">Нет</span><span class="sxs-lookup"><span data-stu-id="47a1d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47a1d-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47a1d-121">JSON Representation</span></span>
<span data-ttu-id="47a1d-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47a1d-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeWeblink",
  "label": "String",
  "link": "String"
}
```




