---
title: Тип ресурса win32LobAppInstallExperience
description: Содержит свойства интерфейса установки приложения Win32
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1a8f6fcecd995857b337f6d91b09e2ce7361defb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797630"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="5fc01-103">Тип ресурса win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="5fc01-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="5fc01-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fc01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5fc01-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5fc01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fc01-106">Содержит свойства интерфейса установки приложения Win32</span><span class="sxs-lookup"><span data-stu-id="5fc01-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="5fc01-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5fc01-107">Properties</span></span>
|<span data-ttu-id="5fc01-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5fc01-108">Property</span></span>|<span data-ttu-id="5fc01-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5fc01-109">Type</span></span>|<span data-ttu-id="5fc01-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5fc01-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fc01-111">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="5fc01-111">runAsAccount</span></span>|[<span data-ttu-id="5fc01-112">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="5fc01-112">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="5fc01-113">Указывает тип контекста выполнения, в котором работает приложение.</span><span class="sxs-lookup"><span data-stu-id="5fc01-113">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="5fc01-114">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="5fc01-114">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="5fc01-115">девицерестартбехавиор</span><span class="sxs-lookup"><span data-stu-id="5fc01-115">deviceRestartBehavior</span></span>|[<span data-ttu-id="5fc01-116">win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="5fc01-116">win32LobAppRestartBehavior</span></span>](../resources/intune-apps-win32lobapprestartbehavior.md)|<span data-ttu-id="5fc01-117">Поведение устройства перезапускается.</span><span class="sxs-lookup"><span data-stu-id="5fc01-117">Device restart behavior.</span></span> <span data-ttu-id="5fc01-118">Возможные значения: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span><span class="sxs-lookup"><span data-stu-id="5fc01-118">Possible values are: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5fc01-119">Связи</span><span class="sxs-lookup"><span data-stu-id="5fc01-119">Relationships</span></span>
<span data-ttu-id="5fc01-120">Нет</span><span class="sxs-lookup"><span data-stu-id="5fc01-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5fc01-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5fc01-121">JSON Representation</span></span>
<span data-ttu-id="5fc01-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5fc01-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "runAsAccount": "String",
  "deviceRestartBehavior": "String"
}
```



