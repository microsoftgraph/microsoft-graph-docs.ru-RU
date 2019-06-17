---
title: Тип ресурса win32LobAppReturnCode
description: Содержит свойства кода возврата для приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 34bda91a0374c57ef4f5ca6e51bc006c80592361
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975779"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="32318-103">Тип ресурса win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="32318-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="32318-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32318-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32318-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32318-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32318-106">Содержит свойства кода возврата для приложения Win32</span><span class="sxs-lookup"><span data-stu-id="32318-106">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="32318-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="32318-107">Properties</span></span>
|<span data-ttu-id="32318-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="32318-108">Property</span></span>|<span data-ttu-id="32318-109">Тип</span><span class="sxs-lookup"><span data-stu-id="32318-109">Type</span></span>|<span data-ttu-id="32318-110">Описание</span><span class="sxs-lookup"><span data-stu-id="32318-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32318-111">Ретурнкоде</span><span class="sxs-lookup"><span data-stu-id="32318-111">returnCode</span></span>|<span data-ttu-id="32318-112">Int32</span><span class="sxs-lookup"><span data-stu-id="32318-112">Int32</span></span>|<span data-ttu-id="32318-113">Возвращаемый код.</span><span class="sxs-lookup"><span data-stu-id="32318-113">Return code.</span></span>|
|<span data-ttu-id="32318-114">type</span><span class="sxs-lookup"><span data-stu-id="32318-114">type</span></span>|[<span data-ttu-id="32318-115">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="32318-115">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="32318-116">Тип кода возврата.</span><span class="sxs-lookup"><span data-stu-id="32318-116">The type of return code.</span></span> <span data-ttu-id="32318-117">Возможные значения: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="32318-117">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32318-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="32318-118">Relationships</span></span>
<span data-ttu-id="32318-119">Нет</span><span class="sxs-lookup"><span data-stu-id="32318-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32318-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="32318-120">JSON Representation</span></span>
<span data-ttu-id="32318-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32318-121">Here is a JSON representation of the resource.</span></span>
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





