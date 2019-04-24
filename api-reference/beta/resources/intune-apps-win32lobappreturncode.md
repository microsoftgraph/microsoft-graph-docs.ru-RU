---
title: Тип ресурса win32LobAppReturnCode
description: Содержит свойства кода возврата для приложения Win32
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c05d695b05a001e6854e254bf065d6fb41ba773
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461089"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="831f2-103">Тип ресурса win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="831f2-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="831f2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="831f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="831f2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="831f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="831f2-106">Содержит свойства кода возврата для приложения Win32</span><span class="sxs-lookup"><span data-stu-id="831f2-106">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="831f2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="831f2-107">Properties</span></span>
|<span data-ttu-id="831f2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="831f2-108">Property</span></span>|<span data-ttu-id="831f2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="831f2-109">Type</span></span>|<span data-ttu-id="831f2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="831f2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="831f2-111">Ретурнкоде</span><span class="sxs-lookup"><span data-stu-id="831f2-111">returnCode</span></span>|<span data-ttu-id="831f2-112">Int32</span><span class="sxs-lookup"><span data-stu-id="831f2-112">Int32</span></span>|<span data-ttu-id="831f2-113">Возвращаемый код.</span><span class="sxs-lookup"><span data-stu-id="831f2-113">Return code.</span></span>|
|<span data-ttu-id="831f2-114">type</span><span class="sxs-lookup"><span data-stu-id="831f2-114">type</span></span>|[<span data-ttu-id="831f2-115">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="831f2-115">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="831f2-116">Тип кода возврата.</span><span class="sxs-lookup"><span data-stu-id="831f2-116">The type of return code.</span></span> <span data-ttu-id="831f2-117">Возможные значения: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="831f2-117">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="831f2-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="831f2-118">Relationships</span></span>
<span data-ttu-id="831f2-119">Нет</span><span class="sxs-lookup"><span data-stu-id="831f2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="831f2-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="831f2-120">JSON Representation</span></span>
<span data-ttu-id="831f2-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="831f2-121">Here is a JSON representation of the resource.</span></span>
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





