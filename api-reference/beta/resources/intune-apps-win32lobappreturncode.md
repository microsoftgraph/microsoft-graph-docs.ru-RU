---
title: Тип ресурса win32LobAppReturnCode
description: Содержит свойства кода возврата для приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 84b2798956ec2b88b4c4dea212fb614f26ff1eff
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335489"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="a7e75-103">Тип ресурса win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="a7e75-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="a7e75-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7e75-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7e75-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7e75-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7e75-106">Содержит свойства кода возврата для приложения Win32</span><span class="sxs-lookup"><span data-stu-id="a7e75-106">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="a7e75-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7e75-107">Properties</span></span>
|<span data-ttu-id="a7e75-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7e75-108">Property</span></span>|<span data-ttu-id="a7e75-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a7e75-109">Type</span></span>|<span data-ttu-id="a7e75-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a7e75-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7e75-111">ретурнкоде</span><span class="sxs-lookup"><span data-stu-id="a7e75-111">returnCode</span></span>|<span data-ttu-id="a7e75-112">Int32</span><span class="sxs-lookup"><span data-stu-id="a7e75-112">Int32</span></span>|<span data-ttu-id="a7e75-113">Возвращаемый код.</span><span class="sxs-lookup"><span data-stu-id="a7e75-113">Return code.</span></span>|
|<span data-ttu-id="a7e75-114">type</span><span class="sxs-lookup"><span data-stu-id="a7e75-114">type</span></span>|[<span data-ttu-id="a7e75-115">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="a7e75-115">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="a7e75-116">Тип кода возврата.</span><span class="sxs-lookup"><span data-stu-id="a7e75-116">The type of return code.</span></span> <span data-ttu-id="a7e75-117">Возможные значения: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="a7e75-117">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7e75-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="a7e75-118">Relationships</span></span>
<span data-ttu-id="a7e75-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a7e75-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7e75-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7e75-120">JSON Representation</span></span>
<span data-ttu-id="a7e75-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7e75-121">Here is a JSON representation of the resource.</span></span>
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



