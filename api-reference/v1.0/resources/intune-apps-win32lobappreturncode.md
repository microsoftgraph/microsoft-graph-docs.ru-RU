---
title: тип ресурса win32LobAppReturnCode
description: Содержит свойства кода возврата для приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 117ab8bd12cf8113efcbe42aa4f2ab7174e50ac3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759102"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="b8e4c-103">тип ресурса win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="b8e4c-103">win32LobAppReturnCode resource type</span></span>

<span data-ttu-id="b8e4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8e4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8e4c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8e4c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8e4c-106">Содержит свойства кода возврата для приложения Win32</span><span class="sxs-lookup"><span data-stu-id="b8e4c-106">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="b8e4c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8e4c-107">Properties</span></span>
|<span data-ttu-id="b8e4c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8e4c-108">Property</span></span>|<span data-ttu-id="b8e4c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b8e4c-109">Type</span></span>|<span data-ttu-id="b8e4c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b8e4c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8e4c-111">returnCode</span><span class="sxs-lookup"><span data-stu-id="b8e4c-111">returnCode</span></span>|<span data-ttu-id="b8e4c-112">Int32</span><span class="sxs-lookup"><span data-stu-id="b8e4c-112">Int32</span></span>|<span data-ttu-id="b8e4c-113">Код возврата.</span><span class="sxs-lookup"><span data-stu-id="b8e4c-113">Return code.</span></span>|
|<span data-ttu-id="b8e4c-114">type</span><span class="sxs-lookup"><span data-stu-id="b8e4c-114">type</span></span>|[<span data-ttu-id="b8e4c-115">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="b8e4c-115">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="b8e4c-116">Тип кода возврата.</span><span class="sxs-lookup"><span data-stu-id="b8e4c-116">The type of return code.</span></span> <span data-ttu-id="b8e4c-117">Возможные значения: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="b8e4c-117">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8e4c-118">Связи</span><span class="sxs-lookup"><span data-stu-id="b8e4c-118">Relationships</span></span>
<span data-ttu-id="b8e4c-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b8e4c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8e4c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8e4c-120">JSON Representation</span></span>
<span data-ttu-id="b8e4c-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8e4c-121">Here is a JSON representation of the resource.</span></span>
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




