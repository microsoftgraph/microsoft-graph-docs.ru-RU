---
title: Тип ресурса win32LobAppInstallExperience
description: Содержит свойства интерфейса установки приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 468afea165645c2fc6a728e5a171b1ef37e9e338
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080167"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="de91b-103">Тип ресурса win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="de91b-103">win32LobAppInstallExperience resource type</span></span>

<span data-ttu-id="de91b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de91b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de91b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de91b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de91b-106">Содержит свойства интерфейса установки приложения Win32</span><span class="sxs-lookup"><span data-stu-id="de91b-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="de91b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="de91b-107">Properties</span></span>
|<span data-ttu-id="de91b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="de91b-108">Property</span></span>|<span data-ttu-id="de91b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="de91b-109">Type</span></span>|<span data-ttu-id="de91b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="de91b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de91b-111">девицерестартбехавиор</span><span class="sxs-lookup"><span data-stu-id="de91b-111">deviceRestartBehavior</span></span>|[<span data-ttu-id="de91b-112">win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="de91b-112">win32LobAppRestartBehavior</span></span>](../resources/intune-apps-win32lobapprestartbehavior.md)|<span data-ttu-id="de91b-113">Поведение устройства перезапускается.</span><span class="sxs-lookup"><span data-stu-id="de91b-113">Device restart behavior.</span></span> <span data-ttu-id="de91b-114">Возможные значения: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span><span class="sxs-lookup"><span data-stu-id="de91b-114">Possible values are: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de91b-115">Связи</span><span class="sxs-lookup"><span data-stu-id="de91b-115">Relationships</span></span>
<span data-ttu-id="de91b-116">Нет</span><span class="sxs-lookup"><span data-stu-id="de91b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de91b-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="de91b-117">JSON Representation</span></span>
<span data-ttu-id="de91b-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de91b-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "deviceRestartBehavior": "String"
}
```





