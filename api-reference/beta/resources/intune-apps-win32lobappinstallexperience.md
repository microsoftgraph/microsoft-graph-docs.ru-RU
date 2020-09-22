---
title: Тип ресурса win32LobAppInstallExperience
description: Содержит свойства интерфейса установки приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b18675a00a9d0e9540bcc57208900dfb925ab72a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033778"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="74706-103">Тип ресурса win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="74706-103">win32LobAppInstallExperience resource type</span></span>

<span data-ttu-id="74706-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74706-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74706-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74706-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74706-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="74706-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74706-107">Содержит свойства интерфейса установки приложения Win32</span><span class="sxs-lookup"><span data-stu-id="74706-107">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="74706-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="74706-108">Properties</span></span>
|<span data-ttu-id="74706-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="74706-109">Property</span></span>|<span data-ttu-id="74706-110">Тип</span><span class="sxs-lookup"><span data-stu-id="74706-110">Type</span></span>|<span data-ttu-id="74706-111">Описание</span><span class="sxs-lookup"><span data-stu-id="74706-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74706-112">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="74706-112">runAsAccount</span></span>|[<span data-ttu-id="74706-113">рунасаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="74706-113">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="74706-114">Указывает тип контекста выполнения, в котором работает приложение.</span><span class="sxs-lookup"><span data-stu-id="74706-114">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="74706-115">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="74706-115">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="74706-116">девицерестартбехавиор</span><span class="sxs-lookup"><span data-stu-id="74706-116">deviceRestartBehavior</span></span>|[<span data-ttu-id="74706-117">win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="74706-117">win32LobAppRestartBehavior</span></span>](../resources/intune-apps-win32lobapprestartbehavior.md)|<span data-ttu-id="74706-118">Поведение устройства перезапускается.</span><span class="sxs-lookup"><span data-stu-id="74706-118">Device restart behavior.</span></span> <span data-ttu-id="74706-119">Возможные значения: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span><span class="sxs-lookup"><span data-stu-id="74706-119">Possible values are: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74706-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="74706-120">Relationships</span></span>
<span data-ttu-id="74706-121">Нет</span><span class="sxs-lookup"><span data-stu-id="74706-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="74706-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74706-122">JSON Representation</span></span>
<span data-ttu-id="74706-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74706-123">Here is a JSON representation of the resource.</span></span>
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






