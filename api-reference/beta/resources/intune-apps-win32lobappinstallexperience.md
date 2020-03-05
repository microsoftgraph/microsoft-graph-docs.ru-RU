---
title: Тип ресурса win32LobAppInstallExperience
description: Содержит свойства интерфейса установки приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 893f473f7543d93572800776d5511371f7cfbf4b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490702"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="d6bd8-103">Тип ресурса win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="d6bd8-103">win32LobAppInstallExperience resource type</span></span>

<span data-ttu-id="d6bd8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d6bd8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6bd8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6bd8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6bd8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6bd8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6bd8-107">Содержит свойства интерфейса установки приложения Win32</span><span class="sxs-lookup"><span data-stu-id="d6bd8-107">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="d6bd8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6bd8-108">Properties</span></span>
|<span data-ttu-id="d6bd8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6bd8-109">Property</span></span>|<span data-ttu-id="d6bd8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d6bd8-110">Type</span></span>|<span data-ttu-id="d6bd8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d6bd8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6bd8-112">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="d6bd8-112">runAsAccount</span></span>|[<span data-ttu-id="d6bd8-113">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="d6bd8-113">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="d6bd8-114">Указывает тип контекста выполнения, в котором работает приложение.</span><span class="sxs-lookup"><span data-stu-id="d6bd8-114">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="d6bd8-115">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="d6bd8-115">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="d6bd8-116">девицерестартбехавиор</span><span class="sxs-lookup"><span data-stu-id="d6bd8-116">deviceRestartBehavior</span></span>|[<span data-ttu-id="d6bd8-117">win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="d6bd8-117">win32LobAppRestartBehavior</span></span>](../resources/intune-apps-win32lobapprestartbehavior.md)|<span data-ttu-id="d6bd8-118">Поведение устройства перезапускается.</span><span class="sxs-lookup"><span data-stu-id="d6bd8-118">Device restart behavior.</span></span> <span data-ttu-id="d6bd8-119">Возможные значения: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span><span class="sxs-lookup"><span data-stu-id="d6bd8-119">Possible values are: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6bd8-120">Связи</span><span class="sxs-lookup"><span data-stu-id="d6bd8-120">Relationships</span></span>
<span data-ttu-id="d6bd8-121">Нет</span><span class="sxs-lookup"><span data-stu-id="d6bd8-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6bd8-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6bd8-122">JSON Representation</span></span>
<span data-ttu-id="d6bd8-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6bd8-123">Here is a JSON representation of the resource.</span></span>
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



