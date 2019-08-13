---
title: Тип ресурса win32LobAppInstallExperience
description: Содержит свойства интерфейса установки приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8cb0efbec4044bb63b9c8069e12bf934662ca587
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335671"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="6703b-103">Тип ресурса win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="6703b-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="6703b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6703b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6703b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6703b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6703b-106">Содержит свойства интерфейса установки приложения Win32</span><span class="sxs-lookup"><span data-stu-id="6703b-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="6703b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6703b-107">Properties</span></span>
|<span data-ttu-id="6703b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6703b-108">Property</span></span>|<span data-ttu-id="6703b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6703b-109">Type</span></span>|<span data-ttu-id="6703b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6703b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6703b-111">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="6703b-111">runAsAccount</span></span>|[<span data-ttu-id="6703b-112">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="6703b-112">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="6703b-113">Указывает тип контекста выполнения, в котором работает приложение.</span><span class="sxs-lookup"><span data-stu-id="6703b-113">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="6703b-114">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="6703b-114">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6703b-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="6703b-115">Relationships</span></span>
<span data-ttu-id="6703b-116">Нет</span><span class="sxs-lookup"><span data-stu-id="6703b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6703b-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6703b-117">JSON Representation</span></span>
<span data-ttu-id="6703b-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6703b-118">Here is a JSON representation of the resource.</span></span>
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



