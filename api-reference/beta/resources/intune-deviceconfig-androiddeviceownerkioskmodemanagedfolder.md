---
title: Тип ресурса androidDeviceOwnerKioskModeManagedFolder
description: Папка, содержащая страницы приложений и веб-ссылок на управляемом домашнем экране
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d4e6b373729ffebb3fc7a08ee29e98f3471c8c27
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162561"
---
# <a name="androiddeviceownerkioskmodemanagedfolder-resource-type"></a><span data-ttu-id="d9e7e-103">Тип ресурса androidDeviceOwnerKioskModeManagedFolder</span><span class="sxs-lookup"><span data-stu-id="d9e7e-103">androidDeviceOwnerKioskModeManagedFolder resource type</span></span>

<span data-ttu-id="d9e7e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9e7e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9e7e-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9e7e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9e7e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9e7e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9e7e-107">Папка, содержащая страницы приложений и веб-ссылок на управляемом домашнем экране</span><span class="sxs-lookup"><span data-stu-id="d9e7e-107">A folder containing pages of apps and weblinks on the Managed Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="d9e7e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9e7e-108">Properties</span></span>
|<span data-ttu-id="d9e7e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9e7e-109">Property</span></span>|<span data-ttu-id="d9e7e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d9e7e-110">Type</span></span>|<span data-ttu-id="d9e7e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d9e7e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9e7e-112">folderName</span><span class="sxs-lookup"><span data-stu-id="d9e7e-112">folderName</span></span>|<span data-ttu-id="d9e7e-113">String</span><span class="sxs-lookup"><span data-stu-id="d9e7e-113">String</span></span>|<span data-ttu-id="d9e7e-114">Отображаемая имя папки</span><span class="sxs-lookup"><span data-stu-id="d9e7e-114">Display name for the folder</span></span>|
|<span data-ttu-id="d9e7e-115">folderIdentifier</span><span class="sxs-lookup"><span data-stu-id="d9e7e-115">folderIdentifier</span></span>|<span data-ttu-id="d9e7e-116">String</span><span class="sxs-lookup"><span data-stu-id="d9e7e-116">String</span></span>|<span data-ttu-id="d9e7e-117">Уникальный идентификатор папки</span><span class="sxs-lookup"><span data-stu-id="d9e7e-117">Unique identifier for the folder</span></span>|
|<span data-ttu-id="d9e7e-118">items</span><span class="sxs-lookup"><span data-stu-id="d9e7e-118">items</span></span>|<span data-ttu-id="d9e7e-119">[Коллекция androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md)</span><span class="sxs-lookup"><span data-stu-id="d9e7e-119">[androidDeviceOwnerKioskModeFolderItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodefolderitem.md) collection</span></span>|<span data-ttu-id="d9e7e-120">Элементы, добавляемые в управлую папку.</span><span class="sxs-lookup"><span data-stu-id="d9e7e-120">Items to be added to managed folder.</span></span> <span data-ttu-id="d9e7e-121">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="d9e7e-121">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9e7e-122">Связи</span><span class="sxs-lookup"><span data-stu-id="d9e7e-122">Relationships</span></span>
<span data-ttu-id="d9e7e-123">Нет</span><span class="sxs-lookup"><span data-stu-id="d9e7e-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9e7e-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9e7e-124">JSON Representation</span></span>
<span data-ttu-id="d9e7e-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9e7e-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
  "folderName": "String",
  "folderIdentifier": "String",
  "items": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
      "label": "String",
      "link": "String"
    }
  ]
}
```




