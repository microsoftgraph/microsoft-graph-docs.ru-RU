---
title: Тип ресурса win32LobAppReturnCode
description: Содержит свойства кода возврата для приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e7429433f4e1a382d0a5f4ba0dab6028bf27d283
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070977"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="5c201-103">Тип ресурса win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="5c201-103">win32LobAppReturnCode resource type</span></span>

<span data-ttu-id="5c201-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c201-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c201-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c201-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c201-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c201-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c201-107">Содержит свойства кода возврата для приложения Win32</span><span class="sxs-lookup"><span data-stu-id="5c201-107">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="5c201-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c201-108">Properties</span></span>
|<span data-ttu-id="5c201-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c201-109">Property</span></span>|<span data-ttu-id="5c201-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5c201-110">Type</span></span>|<span data-ttu-id="5c201-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5c201-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c201-112">ретурнкоде</span><span class="sxs-lookup"><span data-stu-id="5c201-112">returnCode</span></span>|<span data-ttu-id="5c201-113">Int32</span><span class="sxs-lookup"><span data-stu-id="5c201-113">Int32</span></span>|<span data-ttu-id="5c201-114">Возвращаемый код.</span><span class="sxs-lookup"><span data-stu-id="5c201-114">Return code.</span></span>|
|<span data-ttu-id="5c201-115">type</span><span class="sxs-lookup"><span data-stu-id="5c201-115">type</span></span>|[<span data-ttu-id="5c201-116">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="5c201-116">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="5c201-117">Тип кода возврата.</span><span class="sxs-lookup"><span data-stu-id="5c201-117">The type of return code.</span></span> <span data-ttu-id="5c201-118">Возможные значения: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="5c201-118">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c201-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="5c201-119">Relationships</span></span>
<span data-ttu-id="5c201-120">Нет</span><span class="sxs-lookup"><span data-stu-id="5c201-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c201-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5c201-121">JSON Representation</span></span>
<span data-ttu-id="5c201-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c201-122">Here is a JSON representation of the resource.</span></span>
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






