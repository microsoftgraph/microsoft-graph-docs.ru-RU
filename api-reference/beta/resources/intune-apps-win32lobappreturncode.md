---
title: Тип ресурса win32LobAppReturnCode
description: Содержит код возврата свойства для приложения Win32
author: tfitzmac
ms.openlocfilehash: 1ac6b01240e25d1a0163148e61851d6e9405aa44
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346237"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="35e6e-103">Тип ресурса win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="35e6e-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="35e6e-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="35e6e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35e6e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35e6e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35e6e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="35e6e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35e6e-107">Содержит код возврата свойства для приложения Win32</span><span class="sxs-lookup"><span data-stu-id="35e6e-107">Contains return code properties for a Win32 App</span></span>
## <a name="properties"></a><span data-ttu-id="35e6e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="35e6e-108">Properties</span></span>
|<span data-ttu-id="35e6e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="35e6e-109">Property</span></span>|<span data-ttu-id="35e6e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="35e6e-110">Type</span></span>|<span data-ttu-id="35e6e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="35e6e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35e6e-112">код возврата</span><span class="sxs-lookup"><span data-stu-id="35e6e-112">returnCode</span></span>|<span data-ttu-id="35e6e-113">Int32</span><span class="sxs-lookup"><span data-stu-id="35e6e-113">Int32</span></span>|<span data-ttu-id="35e6e-114">Код возврата.</span><span class="sxs-lookup"><span data-stu-id="35e6e-114">Return code.</span></span>|
|<span data-ttu-id="35e6e-115">type</span><span class="sxs-lookup"><span data-stu-id="35e6e-115">type</span></span>|[<span data-ttu-id="35e6e-116">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="35e6e-116">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="35e6e-117">Тип возвращаемого кода.</span><span class="sxs-lookup"><span data-stu-id="35e6e-117">The type of return code.</span></span> <span data-ttu-id="35e6e-118">Возможные значения: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="35e6e-118">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35e6e-119">Связи</span><span class="sxs-lookup"><span data-stu-id="35e6e-119">Relationships</span></span>
<span data-ttu-id="35e6e-120">Нет</span><span class="sxs-lookup"><span data-stu-id="35e6e-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="35e6e-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35e6e-121">JSON Representation</span></span>
<span data-ttu-id="35e6e-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35e6e-122">Here is a JSON representation of the resource.</span></span>
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





