---
title: Тип ресурса Макоссистемекстенсион
description: Представляет определенное расширение системы macOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8cea7fb3cb7c0c95fb0ad5174b171bc1993aa1fb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294027"
---
# <a name="macossystemextension-resource-type"></a><span data-ttu-id="63871-103">Тип ресурса Макоссистемекстенсион</span><span class="sxs-lookup"><span data-stu-id="63871-103">macOSSystemExtension resource type</span></span>

<span data-ttu-id="63871-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63871-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63871-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63871-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63871-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63871-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63871-107">Представляет определенное расширение системы macOS.</span><span class="sxs-lookup"><span data-stu-id="63871-107">Represents a specific macOS system extension.</span></span>

## <a name="properties"></a><span data-ttu-id="63871-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="63871-108">Properties</span></span>
|<span data-ttu-id="63871-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="63871-109">Property</span></span>|<span data-ttu-id="63871-110">Тип</span><span class="sxs-lookup"><span data-stu-id="63871-110">Type</span></span>|<span data-ttu-id="63871-111">Описание</span><span class="sxs-lookup"><span data-stu-id="63871-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63871-112">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="63871-112">teamIdentifier</span></span>|<span data-ttu-id="63871-113">String</span><span class="sxs-lookup"><span data-stu-id="63871-113">String</span></span>|<span data-ttu-id="63871-114">Получает или задает идентификатор группы, использованный для подписи расширения системы.</span><span class="sxs-lookup"><span data-stu-id="63871-114">Gets or sets the team identifier that was used to sign the system extension.</span></span>|
|<span data-ttu-id="63871-115">bundleId</span><span class="sxs-lookup"><span data-stu-id="63871-115">bundleId</span></span>|<span data-ttu-id="63871-116">String</span><span class="sxs-lookup"><span data-stu-id="63871-116">String</span></span>|<span data-ttu-id="63871-117">Получает или задает идентификатор пакета расширения системы.</span><span class="sxs-lookup"><span data-stu-id="63871-117">Gets or sets the bundle identifier of the system extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63871-118">Связи</span><span class="sxs-lookup"><span data-stu-id="63871-118">Relationships</span></span>
<span data-ttu-id="63871-119">Нет</span><span class="sxs-lookup"><span data-stu-id="63871-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63871-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="63871-120">JSON Representation</span></span>
<span data-ttu-id="63871-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63871-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSSystemExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSystemExtension",
  "teamIdentifier": "String",
  "bundleId": "String"
}
```




