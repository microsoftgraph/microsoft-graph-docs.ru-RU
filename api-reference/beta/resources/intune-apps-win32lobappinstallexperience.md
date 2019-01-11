---
title: Тип ресурса win32LobAppInstallExperience
description: Содержит свойства интерфейса установки для приложения Win32
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 74e7dd5b036d42d85e49935f454f3050f604827b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866908"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="c4d2a-103">Тип ресурса win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="c4d2a-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="c4d2a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c4d2a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4d2a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4d2a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c4d2a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c4d2a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c4d2a-107">Содержит свойства интерфейса установки для приложения Win32</span><span class="sxs-lookup"><span data-stu-id="c4d2a-107">Contains installation experience properties for a Win32 App</span></span>
## <a name="properties"></a><span data-ttu-id="c4d2a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4d2a-108">Properties</span></span>
|<span data-ttu-id="c4d2a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4d2a-109">Property</span></span>|<span data-ttu-id="c4d2a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c4d2a-110">Type</span></span>|<span data-ttu-id="c4d2a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c4d2a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4d2a-112">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="c4d2a-112">runAsAccount</span></span>|[<span data-ttu-id="c4d2a-113">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="c4d2a-113">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="c4d2a-114">Указывает тип контекста выполнения, в котором работает приложение в.</span><span class="sxs-lookup"><span data-stu-id="c4d2a-114">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="c4d2a-115">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="c4d2a-115">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4d2a-116">Связи</span><span class="sxs-lookup"><span data-stu-id="c4d2a-116">Relationships</span></span>
<span data-ttu-id="c4d2a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="c4d2a-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c4d2a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4d2a-118">JSON Representation</span></span>
<span data-ttu-id="c4d2a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4d2a-119">Here is a JSON representation of the resource.</span></span>
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





