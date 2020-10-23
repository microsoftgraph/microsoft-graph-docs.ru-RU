---
title: Тип ресурса win32LobAppReturnCode
description: Содержит свойства кода возврата для приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8049ef7a7678d7d5283d45d2236dc364f2df4669
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706172"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="5f180-103">Тип ресурса win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="5f180-103">win32LobAppReturnCode resource type</span></span>

<span data-ttu-id="5f180-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f180-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f180-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f180-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f180-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f180-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f180-107">Содержит свойства кода возврата для приложения Win32</span><span class="sxs-lookup"><span data-stu-id="5f180-107">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="5f180-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f180-108">Properties</span></span>
|<span data-ttu-id="5f180-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f180-109">Property</span></span>|<span data-ttu-id="5f180-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5f180-110">Type</span></span>|<span data-ttu-id="5f180-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5f180-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f180-112">ретурнкоде</span><span class="sxs-lookup"><span data-stu-id="5f180-112">returnCode</span></span>|<span data-ttu-id="5f180-113">Int32</span><span class="sxs-lookup"><span data-stu-id="5f180-113">Int32</span></span>|<span data-ttu-id="5f180-114">Возвращаемый код.</span><span class="sxs-lookup"><span data-stu-id="5f180-114">Return code.</span></span>|
|<span data-ttu-id="5f180-115">type</span><span class="sxs-lookup"><span data-stu-id="5f180-115">type</span></span>|[<span data-ttu-id="5f180-116">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="5f180-116">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="5f180-117">Тип кода возврата.</span><span class="sxs-lookup"><span data-stu-id="5f180-117">The type of return code.</span></span> <span data-ttu-id="5f180-118">Возможные значения: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="5f180-118">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f180-119">Связи</span><span class="sxs-lookup"><span data-stu-id="5f180-119">Relationships</span></span>
<span data-ttu-id="5f180-120">Нет</span><span class="sxs-lookup"><span data-stu-id="5f180-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f180-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f180-121">JSON Representation</span></span>
<span data-ttu-id="5f180-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f180-122">Here is a JSON representation of the resource.</span></span>
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





