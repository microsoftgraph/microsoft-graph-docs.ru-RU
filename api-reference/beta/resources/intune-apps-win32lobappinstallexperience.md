---
title: Тип ресурса win32LobAppInstallExperience
description: Содержит свойства интерфейса установки приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9af7042dd9a95ffde1a447b9d047db003415ad4b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987306"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="108ac-103">Тип ресурса win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="108ac-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="108ac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="108ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="108ac-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="108ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="108ac-106">Содержит свойства интерфейса установки приложения Win32</span><span class="sxs-lookup"><span data-stu-id="108ac-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="108ac-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="108ac-107">Properties</span></span>
|<span data-ttu-id="108ac-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="108ac-108">Property</span></span>|<span data-ttu-id="108ac-109">Тип</span><span class="sxs-lookup"><span data-stu-id="108ac-109">Type</span></span>|<span data-ttu-id="108ac-110">Описание</span><span class="sxs-lookup"><span data-stu-id="108ac-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="108ac-111">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="108ac-111">runAsAccount</span></span>|[<span data-ttu-id="108ac-112">Рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="108ac-112">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="108ac-113">Указывает тип контекста выполнения, в котором работает приложение.</span><span class="sxs-lookup"><span data-stu-id="108ac-113">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="108ac-114">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="108ac-114">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="108ac-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="108ac-115">Relationships</span></span>
<span data-ttu-id="108ac-116">Нет</span><span class="sxs-lookup"><span data-stu-id="108ac-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="108ac-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="108ac-117">JSON Representation</span></span>
<span data-ttu-id="108ac-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="108ac-118">Here is a JSON representation of the resource.</span></span>
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





