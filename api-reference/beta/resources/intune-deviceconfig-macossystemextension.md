---
title: Тип ресурса Макоссистемекстенсион
description: Представляет определенное расширение системы macOS.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bab537a60d213e2e1976c8f902ce7a8b0dbc3027
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44179406"
---
# <a name="macossystemextension-resource-type"></a><span data-ttu-id="08a31-103">Тип ресурса Макоссистемекстенсион</span><span class="sxs-lookup"><span data-stu-id="08a31-103">macOSSystemExtension resource type</span></span>

<span data-ttu-id="08a31-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08a31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08a31-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08a31-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08a31-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08a31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08a31-107">Представляет определенное расширение системы macOS.</span><span class="sxs-lookup"><span data-stu-id="08a31-107">Represents a specific macOS system extension.</span></span>

## <a name="properties"></a><span data-ttu-id="08a31-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="08a31-108">Properties</span></span>
|<span data-ttu-id="08a31-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="08a31-109">Property</span></span>|<span data-ttu-id="08a31-110">Тип</span><span class="sxs-lookup"><span data-stu-id="08a31-110">Type</span></span>|<span data-ttu-id="08a31-111">Описание</span><span class="sxs-lookup"><span data-stu-id="08a31-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08a31-112">теамидентифиер</span><span class="sxs-lookup"><span data-stu-id="08a31-112">teamIdentifier</span></span>|<span data-ttu-id="08a31-113">Строка</span><span class="sxs-lookup"><span data-stu-id="08a31-113">String</span></span>|<span data-ttu-id="08a31-114">Получает или задает идентификатор группы, использованный для подписи расширения системы.</span><span class="sxs-lookup"><span data-stu-id="08a31-114">Gets or sets the team identifier that was used to sign the system extension.</span></span>|
|<span data-ttu-id="08a31-115">bundleId</span><span class="sxs-lookup"><span data-stu-id="08a31-115">bundleId</span></span>|<span data-ttu-id="08a31-116">String</span><span class="sxs-lookup"><span data-stu-id="08a31-116">String</span></span>|<span data-ttu-id="08a31-117">Получает или задает идентификатор пакета расширения системы.</span><span class="sxs-lookup"><span data-stu-id="08a31-117">Gets or sets the bundle identifier of the system extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08a31-118">Связи</span><span class="sxs-lookup"><span data-stu-id="08a31-118">Relationships</span></span>
<span data-ttu-id="08a31-119">Нет</span><span class="sxs-lookup"><span data-stu-id="08a31-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08a31-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08a31-120">JSON Representation</span></span>
<span data-ttu-id="08a31-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08a31-121">Here is a JSON representation of the resource.</span></span>
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



