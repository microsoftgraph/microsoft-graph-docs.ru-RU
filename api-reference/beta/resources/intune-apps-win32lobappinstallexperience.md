---
title: Тип ресурса win32LobAppInstallExperience
description: Содержит свойства интерфейса установки приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aaf3c6dd99b36e33a8af3a8eb4687e1942779937
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538555"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="88a22-103">Тип ресурса win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="88a22-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="88a22-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88a22-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88a22-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88a22-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88a22-106">Содержит свойства интерфейса установки приложения Win32</span><span class="sxs-lookup"><span data-stu-id="88a22-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="88a22-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="88a22-107">Properties</span></span>
|<span data-ttu-id="88a22-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="88a22-108">Property</span></span>|<span data-ttu-id="88a22-109">Тип</span><span class="sxs-lookup"><span data-stu-id="88a22-109">Type</span></span>|<span data-ttu-id="88a22-110">Описание</span><span class="sxs-lookup"><span data-stu-id="88a22-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88a22-111">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="88a22-111">runAsAccount</span></span>|[<span data-ttu-id="88a22-112">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="88a22-112">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="88a22-113">Указывает тип контекста выполнения, в котором работает приложение.</span><span class="sxs-lookup"><span data-stu-id="88a22-113">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="88a22-114">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="88a22-114">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="88a22-115">девицерестартбехавиор</span><span class="sxs-lookup"><span data-stu-id="88a22-115">deviceRestartBehavior</span></span>|[<span data-ttu-id="88a22-116">win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="88a22-116">win32LobAppRestartBehavior</span></span>](../resources/intune-apps-win32lobapprestartbehavior.md)|<span data-ttu-id="88a22-117">Поведение устройства перезапускается.</span><span class="sxs-lookup"><span data-stu-id="88a22-117">Device restart behavior.</span></span> <span data-ttu-id="88a22-118">Возможные значения: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span><span class="sxs-lookup"><span data-stu-id="88a22-118">Possible values are: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88a22-119">Связи</span><span class="sxs-lookup"><span data-stu-id="88a22-119">Relationships</span></span>
<span data-ttu-id="88a22-120">Нет</span><span class="sxs-lookup"><span data-stu-id="88a22-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88a22-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88a22-121">JSON Representation</span></span>
<span data-ttu-id="88a22-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88a22-122">Here is a JSON representation of the resource.</span></span>
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



