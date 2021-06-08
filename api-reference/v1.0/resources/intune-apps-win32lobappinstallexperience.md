---
title: тип ресурса win32LobAppInstallExperience
description: Содержит свойства работы с установкой для приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5a1f844683368d898be7a3acdc1dacbcaffa99ff
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760302"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="b2421-103">тип ресурса win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="b2421-103">win32LobAppInstallExperience resource type</span></span>

<span data-ttu-id="b2421-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2421-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2421-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2421-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2421-106">Содержит свойства работы с установкой для приложения Win32</span><span class="sxs-lookup"><span data-stu-id="b2421-106">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="b2421-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2421-107">Properties</span></span>
|<span data-ttu-id="b2421-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2421-108">Property</span></span>|<span data-ttu-id="b2421-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b2421-109">Type</span></span>|<span data-ttu-id="b2421-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b2421-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2421-111">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="b2421-111">runAsAccount</span></span>|[<span data-ttu-id="b2421-112">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="b2421-112">runAsAccountType</span></span>](../resources/intune-apps-runasaccounttype.md)|<span data-ttu-id="b2421-113">Указывает тип контекста выполнения, в котором выполняется приложение.</span><span class="sxs-lookup"><span data-stu-id="b2421-113">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="b2421-114">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="b2421-114">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="b2421-115">deviceRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="b2421-115">deviceRestartBehavior</span></span>|[<span data-ttu-id="b2421-116">win32LobAppRestartBehavior</span><span class="sxs-lookup"><span data-stu-id="b2421-116">win32LobAppRestartBehavior</span></span>](../resources/intune-apps-win32lobapprestartbehavior.md)|<span data-ttu-id="b2421-117">Поведение перезагрузки устройства.</span><span class="sxs-lookup"><span data-stu-id="b2421-117">Device restart behavior.</span></span> <span data-ttu-id="b2421-118">Возможные значения: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span><span class="sxs-lookup"><span data-stu-id="b2421-118">Possible values are: `basedOnReturnCode`, `allow`, `suppress`, `force`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2421-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b2421-119">Relationships</span></span>
<span data-ttu-id="b2421-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b2421-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2421-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2421-121">JSON Representation</span></span>
<span data-ttu-id="b2421-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2421-122">Here is a JSON representation of the resource.</span></span>
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




