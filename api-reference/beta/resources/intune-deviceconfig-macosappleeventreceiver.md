---
title: Тип ресурса Макосаппливентрецеивер
description: Представляет процесс, который может принимать уведомления о событиях Apple.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 16064b1f7311f8ab384d7905a6f4cfa2f09ccc09
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177354"
---
# <a name="macosappleeventreceiver-resource-type"></a><span data-ttu-id="fd320-103">Тип ресурса Макосаппливентрецеивер</span><span class="sxs-lookup"><span data-stu-id="fd320-103">macOSAppleEventReceiver resource type</span></span>

<span data-ttu-id="fd320-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd320-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd320-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd320-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd320-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fd320-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd320-107">Представляет процесс, который может принимать уведомления о событиях Apple.</span><span class="sxs-lookup"><span data-stu-id="fd320-107">Represents a process that can receive an Apple Event notification.</span></span>

## <a name="properties"></a><span data-ttu-id="fd320-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd320-108">Properties</span></span>
|<span data-ttu-id="fd320-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd320-109">Property</span></span>|<span data-ttu-id="fd320-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fd320-110">Type</span></span>|<span data-ttu-id="fd320-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fd320-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd320-112">кодерекуиремент</span><span class="sxs-lookup"><span data-stu-id="fd320-112">codeRequirement</span></span>|<span data-ttu-id="fd320-113">Строка</span><span class="sxs-lookup"><span data-stu-id="fd320-113">String</span></span>|<span data-ttu-id="fd320-114">Требования к коду для приложения или двоичных файлов, которые получают событие Apple.</span><span class="sxs-lookup"><span data-stu-id="fd320-114">Code requirement for the app or binary that receives the Apple Event.</span></span>|
|<span data-ttu-id="fd320-115">идентификатор</span><span class="sxs-lookup"><span data-stu-id="fd320-115">identifier</span></span>|<span data-ttu-id="fd320-116">Строка</span><span class="sxs-lookup"><span data-stu-id="fd320-116">String</span></span>|<span data-ttu-id="fd320-117">Идентификатор пакета приложения или пути к файлу процесса или исполняемого файла, который получает событие Apple.</span><span class="sxs-lookup"><span data-stu-id="fd320-117">Bundle ID of the app or file path of the process or executable that receives the Apple Event.</span></span>|
|<span data-ttu-id="fd320-118">identifierType</span><span class="sxs-lookup"><span data-stu-id="fd320-118">identifierType</span></span>|[<span data-ttu-id="fd320-119">макоспроцессидентифиертипе</span><span class="sxs-lookup"><span data-stu-id="fd320-119">macOSProcessIdentifierType</span></span>](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|<span data-ttu-id="fd320-120">Используйте идентификатор пакета для приложения или пути для процесса или исполняемого файла, который получает событие Apple.</span><span class="sxs-lookup"><span data-stu-id="fd320-120">Use bundle ID for an app or path for a process or executable that receives the Apple Event.</span></span> <span data-ttu-id="fd320-121">Возможные значения: `bundleID`, `path`.</span><span class="sxs-lookup"><span data-stu-id="fd320-121">Possible values are: `bundleID`, `path`.</span></span>|
|<span data-ttu-id="fd320-122">разрешенных</span><span class="sxs-lookup"><span data-stu-id="fd320-122">allowed</span></span>|<span data-ttu-id="fd320-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd320-123">Boolean</span></span>|<span data-ttu-id="fd320-124">Разрешить или запретить получение событий Apple для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="fd320-124">Allow or block this app from receiving Apple events.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd320-125">Связи</span><span class="sxs-lookup"><span data-stu-id="fd320-125">Relationships</span></span>
<span data-ttu-id="fd320-126">Нет</span><span class="sxs-lookup"><span data-stu-id="fd320-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd320-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fd320-127">JSON Representation</span></span>
<span data-ttu-id="fd320-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd320-128">Here is a JSON representation of the resource.</span></span>
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



