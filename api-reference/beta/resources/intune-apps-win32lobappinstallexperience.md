---
title: Тип ресурса win32LobAppInstallExperience
description: Содержит свойства интерфейса установки для приложения Win32
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9eeadf7bc97f53278ef59fe06795bc7120d5bc2c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986301"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="d30a6-103">Тип ресурса win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="d30a6-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="d30a6-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d30a6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d30a6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d30a6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d30a6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d30a6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d30a6-107">Содержит свойства интерфейса установки для приложения Win32</span><span class="sxs-lookup"><span data-stu-id="d30a6-107">Contains installation experience properties for a Win32 App</span></span>
## <a name="properties"></a><span data-ttu-id="d30a6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d30a6-108">Properties</span></span>
|<span data-ttu-id="d30a6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d30a6-109">Property</span></span>|<span data-ttu-id="d30a6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d30a6-110">Type</span></span>|<span data-ttu-id="d30a6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d30a6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d30a6-112">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="d30a6-112">runAsAccount</span></span>|[<span data-ttu-id="d30a6-113">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="d30a6-113">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="d30a6-114">Указывает тип контекста выполнения, в котором работает приложение в.</span><span class="sxs-lookup"><span data-stu-id="d30a6-114">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="d30a6-115">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="d30a6-115">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d30a6-116">Связи</span><span class="sxs-lookup"><span data-stu-id="d30a6-116">Relationships</span></span>
<span data-ttu-id="d30a6-117">Нет</span><span class="sxs-lookup"><span data-stu-id="d30a6-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d30a6-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d30a6-118">JSON Representation</span></span>
<span data-ttu-id="d30a6-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d30a6-119">Here is a JSON representation of the resource.</span></span>
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





