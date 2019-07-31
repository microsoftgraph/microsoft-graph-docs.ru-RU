---
title: Тип ресурса win32LobAppReturnCode
description: Содержит свойства кода возврата для приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1ea4c0138aa6d2cf90ac111a91f7e0acc145d64c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012214"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="b0690-103">Тип ресурса win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="b0690-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="b0690-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0690-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0690-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0690-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0690-106">Содержит свойства кода возврата для приложения Win32</span><span class="sxs-lookup"><span data-stu-id="b0690-106">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="b0690-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0690-107">Properties</span></span>
|<span data-ttu-id="b0690-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0690-108">Property</span></span>|<span data-ttu-id="b0690-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b0690-109">Type</span></span>|<span data-ttu-id="b0690-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b0690-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0690-111">Ретурнкоде</span><span class="sxs-lookup"><span data-stu-id="b0690-111">returnCode</span></span>|<span data-ttu-id="b0690-112">Int32</span><span class="sxs-lookup"><span data-stu-id="b0690-112">Int32</span></span>|<span data-ttu-id="b0690-113">Возвращаемый код.</span><span class="sxs-lookup"><span data-stu-id="b0690-113">Return code.</span></span>|
|<span data-ttu-id="b0690-114">type</span><span class="sxs-lookup"><span data-stu-id="b0690-114">type</span></span>|[<span data-ttu-id="b0690-115">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="b0690-115">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="b0690-116">Тип кода возврата.</span><span class="sxs-lookup"><span data-stu-id="b0690-116">The type of return code.</span></span> <span data-ttu-id="b0690-117">Возможные значения: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="b0690-117">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0690-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="b0690-118">Relationships</span></span>
<span data-ttu-id="b0690-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b0690-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0690-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0690-120">JSON Representation</span></span>
<span data-ttu-id="b0690-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0690-121">Here is a JSON representation of the resource.</span></span>
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





