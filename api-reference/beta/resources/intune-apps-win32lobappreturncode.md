---
title: Тип ресурса win32LobAppReturnCode
description: Содержит свойства кода возврата для приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a37236064abb2e792e9227b8f76f32e1fd3ff9d9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949481"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="b9e64-103">Тип ресурса win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="b9e64-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="b9e64-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9e64-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9e64-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b9e64-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9e64-106">Содержит свойства кода возврата для приложения Win32</span><span class="sxs-lookup"><span data-stu-id="b9e64-106">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="b9e64-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9e64-107">Properties</span></span>
|<span data-ttu-id="b9e64-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9e64-108">Property</span></span>|<span data-ttu-id="b9e64-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b9e64-109">Type</span></span>|<span data-ttu-id="b9e64-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b9e64-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9e64-111">Ретурнкоде</span><span class="sxs-lookup"><span data-stu-id="b9e64-111">returnCode</span></span>|<span data-ttu-id="b9e64-112">Int32</span><span class="sxs-lookup"><span data-stu-id="b9e64-112">Int32</span></span>|<span data-ttu-id="b9e64-113">Возвращаемый код.</span><span class="sxs-lookup"><span data-stu-id="b9e64-113">Return code.</span></span>|
|<span data-ttu-id="b9e64-114">type</span><span class="sxs-lookup"><span data-stu-id="b9e64-114">type</span></span>|[<span data-ttu-id="b9e64-115">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="b9e64-115">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="b9e64-116">Тип кода возврата.</span><span class="sxs-lookup"><span data-stu-id="b9e64-116">The type of return code.</span></span> <span data-ttu-id="b9e64-117">Возможные значения: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="b9e64-117">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9e64-118">Связи</span><span class="sxs-lookup"><span data-stu-id="b9e64-118">Relationships</span></span>
<span data-ttu-id="b9e64-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b9e64-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9e64-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b9e64-120">JSON Representation</span></span>
<span data-ttu-id="b9e64-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9e64-121">Here is a JSON representation of the resource.</span></span>
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




