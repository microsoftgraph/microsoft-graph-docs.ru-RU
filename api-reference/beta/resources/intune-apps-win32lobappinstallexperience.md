---
title: Тип ресурса win32LobAppInstallExperience
description: Содержит свойства интерфейса установки приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cc79e79c3922982f58a39b1f835b936e62d5c400
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949586"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="dfb78-103">Тип ресурса win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="dfb78-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="dfb78-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfb78-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfb78-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dfb78-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfb78-106">Содержит свойства интерфейса установки приложения Win32</span><span class="sxs-lookup"><span data-stu-id="dfb78-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="dfb78-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dfb78-107">Properties</span></span>
|<span data-ttu-id="dfb78-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="dfb78-108">Property</span></span>|<span data-ttu-id="dfb78-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dfb78-109">Type</span></span>|<span data-ttu-id="dfb78-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dfb78-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfb78-111">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="dfb78-111">runAsAccount</span></span>|[<span data-ttu-id="dfb78-112">Рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="dfb78-112">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="dfb78-113">Указывает тип контекста выполнения, в котором работает приложение.</span><span class="sxs-lookup"><span data-stu-id="dfb78-113">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="dfb78-114">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="dfb78-114">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfb78-115">Связи</span><span class="sxs-lookup"><span data-stu-id="dfb78-115">Relationships</span></span>
<span data-ttu-id="dfb78-116">Нет</span><span class="sxs-lookup"><span data-stu-id="dfb78-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfb78-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dfb78-117">JSON Representation</span></span>
<span data-ttu-id="dfb78-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dfb78-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "runAsAccount": "String"
}
```




