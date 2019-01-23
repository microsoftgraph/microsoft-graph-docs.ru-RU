---
title: Тип ресурса win32LobAppReturnCode
description: Содержит код возврата свойства для приложения Win32
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e6357d0ac6aab87e236e02d60454d1b45aa98fe1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404360"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="a50b1-103">Тип ресурса win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="a50b1-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="a50b1-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a50b1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a50b1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a50b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a50b1-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a50b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a50b1-107">Содержит код возврата свойства для приложения Win32</span><span class="sxs-lookup"><span data-stu-id="a50b1-107">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="a50b1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a50b1-108">Properties</span></span>
|<span data-ttu-id="a50b1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a50b1-109">Property</span></span>|<span data-ttu-id="a50b1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a50b1-110">Type</span></span>|<span data-ttu-id="a50b1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a50b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a50b1-112">код возврата</span><span class="sxs-lookup"><span data-stu-id="a50b1-112">returnCode</span></span>|<span data-ttu-id="a50b1-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a50b1-113">Int32</span></span>|<span data-ttu-id="a50b1-114">Код возврата.</span><span class="sxs-lookup"><span data-stu-id="a50b1-114">Return code.</span></span>|
|<span data-ttu-id="a50b1-115">type</span><span class="sxs-lookup"><span data-stu-id="a50b1-115">type</span></span>|[<span data-ttu-id="a50b1-116">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="a50b1-116">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="a50b1-117">Тип возвращаемого кода.</span><span class="sxs-lookup"><span data-stu-id="a50b1-117">The type of return code.</span></span> <span data-ttu-id="a50b1-118">Возможные значения: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="a50b1-118">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a50b1-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="a50b1-119">Relationships</span></span>
<span data-ttu-id="a50b1-120">Нет</span><span class="sxs-lookup"><span data-stu-id="a50b1-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a50b1-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a50b1-121">JSON Representation</span></span>
<span data-ttu-id="a50b1-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a50b1-122">Here is a JSON representation of the resource.</span></span>
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




