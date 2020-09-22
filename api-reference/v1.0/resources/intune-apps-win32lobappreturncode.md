---
title: Тип ресурса win32LobAppReturnCode
description: Содержит свойства кода возврата для приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e9b64542a7c3679e31b23ee63bcdcf9713bccc92
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036760"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="61596-103">Тип ресурса win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="61596-103">win32LobAppReturnCode resource type</span></span>

<span data-ttu-id="61596-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61596-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61596-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="61596-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61596-106">Содержит свойства кода возврата для приложения Win32</span><span class="sxs-lookup"><span data-stu-id="61596-106">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="61596-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="61596-107">Properties</span></span>
|<span data-ttu-id="61596-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="61596-108">Property</span></span>|<span data-ttu-id="61596-109">Тип</span><span class="sxs-lookup"><span data-stu-id="61596-109">Type</span></span>|<span data-ttu-id="61596-110">Описание</span><span class="sxs-lookup"><span data-stu-id="61596-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61596-111">ретурнкоде</span><span class="sxs-lookup"><span data-stu-id="61596-111">returnCode</span></span>|<span data-ttu-id="61596-112">Int32</span><span class="sxs-lookup"><span data-stu-id="61596-112">Int32</span></span>|<span data-ttu-id="61596-113">Возвращаемый код.</span><span class="sxs-lookup"><span data-stu-id="61596-113">Return code.</span></span>|
|<span data-ttu-id="61596-114">type</span><span class="sxs-lookup"><span data-stu-id="61596-114">type</span></span>|[<span data-ttu-id="61596-115">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="61596-115">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="61596-116">Тип кода возврата.</span><span class="sxs-lookup"><span data-stu-id="61596-116">The type of return code.</span></span> <span data-ttu-id="61596-117">Возможные значения: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="61596-117">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61596-118">Связи</span><span class="sxs-lookup"><span data-stu-id="61596-118">Relationships</span></span>
<span data-ttu-id="61596-119">Нет</span><span class="sxs-lookup"><span data-stu-id="61596-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61596-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="61596-120">JSON Representation</span></span>
<span data-ttu-id="61596-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61596-121">Here is a JSON representation of the resource.</span></span>
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





