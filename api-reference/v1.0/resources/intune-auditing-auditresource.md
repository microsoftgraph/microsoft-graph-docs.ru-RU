---
title: Тип ресурса auditResource
description: Класс, содержащий свойства ресурса аудита.
ms.openlocfilehash: 452df4cb27dba5de04022c6ba7be08471286d866
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027397"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="44756-103">Тип ресурса auditResource</span><span class="sxs-lookup"><span data-stu-id="44756-103">auditResource resource type</span></span>

> <span data-ttu-id="44756-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="44756-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44756-105">Класс, содержащий свойства ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="44756-105">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="44756-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="44756-106">Properties</span></span>
|<span data-ttu-id="44756-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="44756-107">Property</span></span>|<span data-ttu-id="44756-108">Тип</span><span class="sxs-lookup"><span data-stu-id="44756-108">Type</span></span>|<span data-ttu-id="44756-109">Описание</span><span class="sxs-lookup"><span data-stu-id="44756-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44756-110">displayName</span><span class="sxs-lookup"><span data-stu-id="44756-110">displayName</span></span>|<span data-ttu-id="44756-111">String</span><span class="sxs-lookup"><span data-stu-id="44756-111">String</span></span>|<span data-ttu-id="44756-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="44756-112">Display name.</span></span>|
|<span data-ttu-id="44756-113">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="44756-113">modifiedProperties</span></span>|<span data-ttu-id="44756-114">Коллекция [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="44756-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="44756-115">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="44756-115">List of modified properties.</span></span>|
|<span data-ttu-id="44756-116">type</span><span class="sxs-lookup"><span data-stu-id="44756-116">type</span></span>|<span data-ttu-id="44756-117">String</span><span class="sxs-lookup"><span data-stu-id="44756-117">String</span></span>|<span data-ttu-id="44756-118">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="44756-118">Audit resource's type.</span></span>|
|<span data-ttu-id="44756-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="44756-119">resourceId</span></span>|<span data-ttu-id="44756-120">String</span><span class="sxs-lookup"><span data-stu-id="44756-120">String</span></span>|<span data-ttu-id="44756-121">ИД ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="44756-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44756-122">Связи</span><span class="sxs-lookup"><span data-stu-id="44756-122">Relationships</span></span>
<span data-ttu-id="44756-123">Нет</span><span class="sxs-lookup"><span data-stu-id="44756-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="44756-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44756-124">JSON Representation</span></span>
<span data-ttu-id="44756-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44756-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```



