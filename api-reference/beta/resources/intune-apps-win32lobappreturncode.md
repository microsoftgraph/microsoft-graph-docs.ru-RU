---
title: Тип ресурса win32LobAppReturnCode
description: Содержит свойства кода возврата для приложения Win32
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5e1c312fd7a43c6f685d80211849e9a9280917b8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797551"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="47df4-103">Тип ресурса win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="47df4-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="47df4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47df4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47df4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47df4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47df4-106">Содержит свойства кода возврата для приложения Win32</span><span class="sxs-lookup"><span data-stu-id="47df4-106">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="47df4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="47df4-107">Properties</span></span>
|<span data-ttu-id="47df4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="47df4-108">Property</span></span>|<span data-ttu-id="47df4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="47df4-109">Type</span></span>|<span data-ttu-id="47df4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="47df4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47df4-111">ретурнкоде</span><span class="sxs-lookup"><span data-stu-id="47df4-111">returnCode</span></span>|<span data-ttu-id="47df4-112">Int32</span><span class="sxs-lookup"><span data-stu-id="47df4-112">Int32</span></span>|<span data-ttu-id="47df4-113">Возвращаемый код.</span><span class="sxs-lookup"><span data-stu-id="47df4-113">Return code.</span></span>|
|<span data-ttu-id="47df4-114">type</span><span class="sxs-lookup"><span data-stu-id="47df4-114">type</span></span>|[<span data-ttu-id="47df4-115">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="47df4-115">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="47df4-116">Тип кода возврата.</span><span class="sxs-lookup"><span data-stu-id="47df4-116">The type of return code.</span></span> <span data-ttu-id="47df4-117">Возможные значения: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="47df4-117">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47df4-118">Связи</span><span class="sxs-lookup"><span data-stu-id="47df4-118">Relationships</span></span>
<span data-ttu-id="47df4-119">Нет</span><span class="sxs-lookup"><span data-stu-id="47df4-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47df4-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47df4-120">JSON Representation</span></span>
<span data-ttu-id="47df4-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47df4-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppReturnCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppReturnCode",
  "returnCode": 1024,
  "type": "String"
}
```



