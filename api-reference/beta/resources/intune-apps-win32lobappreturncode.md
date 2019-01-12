---
title: Тип ресурса win32LobAppReturnCode
description: Содержит код возврата свойства для приложения Win32
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0728ee3c029331b37369172373ef1400dde37991
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927865"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="e28f1-103">Тип ресурса win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="e28f1-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="e28f1-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e28f1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e28f1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e28f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e28f1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e28f1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e28f1-107">Содержит код возврата свойства для приложения Win32</span><span class="sxs-lookup"><span data-stu-id="e28f1-107">Contains return code properties for a Win32 App</span></span>
## <a name="properties"></a><span data-ttu-id="e28f1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e28f1-108">Properties</span></span>
|<span data-ttu-id="e28f1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e28f1-109">Property</span></span>|<span data-ttu-id="e28f1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e28f1-110">Type</span></span>|<span data-ttu-id="e28f1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e28f1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e28f1-112">код возврата</span><span class="sxs-lookup"><span data-stu-id="e28f1-112">returnCode</span></span>|<span data-ttu-id="e28f1-113">Int32</span><span class="sxs-lookup"><span data-stu-id="e28f1-113">Int32</span></span>|<span data-ttu-id="e28f1-114">Код возврата.</span><span class="sxs-lookup"><span data-stu-id="e28f1-114">Return code.</span></span>|
|<span data-ttu-id="e28f1-115">type</span><span class="sxs-lookup"><span data-stu-id="e28f1-115">type</span></span>|[<span data-ttu-id="e28f1-116">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="e28f1-116">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="e28f1-117">Тип возвращаемого кода.</span><span class="sxs-lookup"><span data-stu-id="e28f1-117">The type of return code.</span></span> <span data-ttu-id="e28f1-118">Возможные значения: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="e28f1-118">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e28f1-119">Связи</span><span class="sxs-lookup"><span data-stu-id="e28f1-119">Relationships</span></span>
<span data-ttu-id="e28f1-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e28f1-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e28f1-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e28f1-121">JSON Representation</span></span>
<span data-ttu-id="e28f1-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e28f1-122">Here is a JSON representation of the resource.</span></span>
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





