---
title: Тип ресурса win32LobAppReturnCode
description: Содержит свойства кода возврата для приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 38111feb284407a028e222beb3894d6359ed72c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490282"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="72617-103">Тип ресурса win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="72617-103">win32LobAppReturnCode resource type</span></span>

<span data-ttu-id="72617-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="72617-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72617-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72617-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72617-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72617-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72617-107">Содержит свойства кода возврата для приложения Win32</span><span class="sxs-lookup"><span data-stu-id="72617-107">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="72617-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="72617-108">Properties</span></span>
|<span data-ttu-id="72617-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="72617-109">Property</span></span>|<span data-ttu-id="72617-110">Тип</span><span class="sxs-lookup"><span data-stu-id="72617-110">Type</span></span>|<span data-ttu-id="72617-111">Описание</span><span class="sxs-lookup"><span data-stu-id="72617-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72617-112">ретурнкоде</span><span class="sxs-lookup"><span data-stu-id="72617-112">returnCode</span></span>|<span data-ttu-id="72617-113">Int32</span><span class="sxs-lookup"><span data-stu-id="72617-113">Int32</span></span>|<span data-ttu-id="72617-114">Возвращаемый код.</span><span class="sxs-lookup"><span data-stu-id="72617-114">Return code.</span></span>|
|<span data-ttu-id="72617-115">type</span><span class="sxs-lookup"><span data-stu-id="72617-115">type</span></span>|[<span data-ttu-id="72617-116">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="72617-116">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="72617-117">Тип кода возврата.</span><span class="sxs-lookup"><span data-stu-id="72617-117">The type of return code.</span></span> <span data-ttu-id="72617-118">Возможные значения: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="72617-118">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72617-119">Связи</span><span class="sxs-lookup"><span data-stu-id="72617-119">Relationships</span></span>
<span data-ttu-id="72617-120">Нет</span><span class="sxs-lookup"><span data-stu-id="72617-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72617-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72617-121">JSON Representation</span></span>
<span data-ttu-id="72617-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72617-122">Here is a JSON representation of the resource.</span></span>
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



