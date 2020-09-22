---
title: Тип ресурса Макосаппливентрецеивер
description: Представляет процесс, который может принимать уведомления о событиях Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db781ad536e8fe918257f74d87fa104f4b2a23f1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055451"
---
# <a name="macosappleeventreceiver-resource-type"></a><span data-ttu-id="0231b-103">Тип ресурса Макосаппливентрецеивер</span><span class="sxs-lookup"><span data-stu-id="0231b-103">macOSAppleEventReceiver resource type</span></span>

<span data-ttu-id="0231b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0231b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0231b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0231b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0231b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0231b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0231b-107">Представляет процесс, который может принимать уведомления о событиях Apple.</span><span class="sxs-lookup"><span data-stu-id="0231b-107">Represents a process that can receive an Apple Event notification.</span></span>

## <a name="properties"></a><span data-ttu-id="0231b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0231b-108">Properties</span></span>
|<span data-ttu-id="0231b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0231b-109">Property</span></span>|<span data-ttu-id="0231b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0231b-110">Type</span></span>|<span data-ttu-id="0231b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0231b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0231b-112">кодерекуиремент</span><span class="sxs-lookup"><span data-stu-id="0231b-112">codeRequirement</span></span>|<span data-ttu-id="0231b-113">String</span><span class="sxs-lookup"><span data-stu-id="0231b-113">String</span></span>|<span data-ttu-id="0231b-114">Требования к коду для приложения или двоичных файлов, которые получают событие Apple.</span><span class="sxs-lookup"><span data-stu-id="0231b-114">Code requirement for the app or binary that receives the Apple Event.</span></span>|
|<span data-ttu-id="0231b-115">идентификатор</span><span class="sxs-lookup"><span data-stu-id="0231b-115">identifier</span></span>|<span data-ttu-id="0231b-116">String</span><span class="sxs-lookup"><span data-stu-id="0231b-116">String</span></span>|<span data-ttu-id="0231b-117">Идентификатор пакета приложения или пути к файлу процесса или исполняемого файла, который получает событие Apple.</span><span class="sxs-lookup"><span data-stu-id="0231b-117">Bundle ID of the app or file path of the process or executable that receives the Apple Event.</span></span>|
|<span data-ttu-id="0231b-118">identifierType</span><span class="sxs-lookup"><span data-stu-id="0231b-118">identifierType</span></span>|[<span data-ttu-id="0231b-119">macOSProcessIdentifierType</span><span class="sxs-lookup"><span data-stu-id="0231b-119">macOSProcessIdentifierType</span></span>](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|<span data-ttu-id="0231b-120">Используйте идентификатор пакета для приложения или пути для процесса или исполняемого файла, который получает событие Apple.</span><span class="sxs-lookup"><span data-stu-id="0231b-120">Use bundle ID for an app or path for a process or executable that receives the Apple Event.</span></span> <span data-ttu-id="0231b-121">Возможные значения: `bundleID`, `path`.</span><span class="sxs-lookup"><span data-stu-id="0231b-121">Possible values are: `bundleID`, `path`.</span></span>|
|<span data-ttu-id="0231b-122">разрешенных</span><span class="sxs-lookup"><span data-stu-id="0231b-122">allowed</span></span>|<span data-ttu-id="0231b-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="0231b-123">Boolean</span></span>|<span data-ttu-id="0231b-124">Разрешить или запретить получение событий Apple для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="0231b-124">Allow or block this app from receiving Apple events.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0231b-125">Связи</span><span class="sxs-lookup"><span data-stu-id="0231b-125">Relationships</span></span>
<span data-ttu-id="0231b-126">Нет</span><span class="sxs-lookup"><span data-stu-id="0231b-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0231b-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0231b-127">JSON Representation</span></span>
<span data-ttu-id="0231b-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0231b-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAppleEventReceiver"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAppleEventReceiver",
  "codeRequirement": "String",
  "identifier": "String",
  "identifierType": "String",
  "allowed": true
}
```






