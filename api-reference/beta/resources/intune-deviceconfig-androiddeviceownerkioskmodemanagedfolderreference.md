---
title: Тип ресурса androidDeviceOwnerKioskModeManagedFolderReference
description: Ссылка на папку, содержащую приложения и веб-ссылки на управляемом домашнем экране
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f454abc8edb54e1ee2ed2e9a6984e8e9e39e29d2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162558"
---
# <a name="androiddeviceownerkioskmodemanagedfolderreference-resource-type"></a><span data-ttu-id="8f8b1-103">Тип ресурса androidDeviceOwnerKioskModeManagedFolderReference</span><span class="sxs-lookup"><span data-stu-id="8f8b1-103">androidDeviceOwnerKioskModeManagedFolderReference resource type</span></span>

<span data-ttu-id="8f8b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f8b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f8b1-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f8b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f8b1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f8b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f8b1-107">Ссылка на папку, содержащую приложения и веб-ссылки на управляемом домашнем экране</span><span class="sxs-lookup"><span data-stu-id="8f8b1-107">A reference to folder containing apps and weblinks on the Managed Home Screen</span></span>


<span data-ttu-id="8f8b1-108">Наследуется [от androidDeviceOwnerKioskModeHomeScreenItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodehomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="8f8b1-108">Inherits from [androidDeviceOwnerKioskModeHomeScreenItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodehomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8f8b1-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f8b1-109">Properties</span></span>
|<span data-ttu-id="8f8b1-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f8b1-110">Property</span></span>|<span data-ttu-id="8f8b1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8f8b1-111">Type</span></span>|<span data-ttu-id="8f8b1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8f8b1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f8b1-113">folderName</span><span class="sxs-lookup"><span data-stu-id="8f8b1-113">folderName</span></span>|<span data-ttu-id="8f8b1-114">String</span><span class="sxs-lookup"><span data-stu-id="8f8b1-114">String</span></span>|<span data-ttu-id="8f8b1-115">Имя папки</span><span class="sxs-lookup"><span data-stu-id="8f8b1-115">Name of the folder</span></span>|
|<span data-ttu-id="8f8b1-116">folderIdentifier</span><span class="sxs-lookup"><span data-stu-id="8f8b1-116">folderIdentifier</span></span>|<span data-ttu-id="8f8b1-117">String</span><span class="sxs-lookup"><span data-stu-id="8f8b1-117">String</span></span>|<span data-ttu-id="8f8b1-118">Уникальный идентификатор папки</span><span class="sxs-lookup"><span data-stu-id="8f8b1-118">Unique identifier for the folder</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f8b1-119">Связи</span><span class="sxs-lookup"><span data-stu-id="8f8b1-119">Relationships</span></span>
<span data-ttu-id="8f8b1-120">Нет</span><span class="sxs-lookup"><span data-stu-id="8f8b1-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f8b1-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f8b1-121">JSON Representation</span></span>
<span data-ttu-id="8f8b1-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f8b1-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolderReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeManagedFolderReference",
  "folderName": "String",
  "folderIdentifier": "String"
}
```




