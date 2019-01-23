---
title: Тип ресурса win32LobAppInstallExperience
description: Содержит свойства интерфейса установки для приложения Win32
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 240000dfceaa2ef4e973167cbd3b5a743d346892
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406691"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="9073f-103">Тип ресурса win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="9073f-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="9073f-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9073f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9073f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9073f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9073f-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9073f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9073f-107">Содержит свойства интерфейса установки для приложения Win32</span><span class="sxs-lookup"><span data-stu-id="9073f-107">Contains installation experience properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="9073f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9073f-108">Properties</span></span>
|<span data-ttu-id="9073f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9073f-109">Property</span></span>|<span data-ttu-id="9073f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9073f-110">Type</span></span>|<span data-ttu-id="9073f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9073f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9073f-112">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="9073f-112">runAsAccount</span></span>|[<span data-ttu-id="9073f-113">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="9073f-113">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="9073f-114">Указывает тип контекста выполнения, в котором работает приложение в.</span><span class="sxs-lookup"><span data-stu-id="9073f-114">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="9073f-115">Возможные значения: `system`, `user`.</span><span class="sxs-lookup"><span data-stu-id="9073f-115">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9073f-116">Связи</span><span class="sxs-lookup"><span data-stu-id="9073f-116">Relationships</span></span>
<span data-ttu-id="9073f-117">Нет</span><span class="sxs-lookup"><span data-stu-id="9073f-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9073f-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9073f-118">JSON Representation</span></span>
<span data-ttu-id="9073f-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9073f-119">Here is a JSON representation of the resource.</span></span>
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




