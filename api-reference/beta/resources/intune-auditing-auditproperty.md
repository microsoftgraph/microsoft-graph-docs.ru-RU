---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f864f41a2068d6455dccb0a539c14e7e4b9dc6d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558344"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="3607f-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="3607f-103">auditProperty resource type</span></span>

> <span data-ttu-id="3607f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3607f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3607f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3607f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3607f-106">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="3607f-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="3607f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3607f-107">Properties</span></span>
|<span data-ttu-id="3607f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3607f-108">Property</span></span>|<span data-ttu-id="3607f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3607f-109">Type</span></span>|<span data-ttu-id="3607f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3607f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3607f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="3607f-111">displayName</span></span>|<span data-ttu-id="3607f-112">String</span><span class="sxs-lookup"><span data-stu-id="3607f-112">String</span></span>|<span data-ttu-id="3607f-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="3607f-113">Display name.</span></span>|
|<span data-ttu-id="3607f-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="3607f-114">oldValue</span></span>|<span data-ttu-id="3607f-115">String</span><span class="sxs-lookup"><span data-stu-id="3607f-115">String</span></span>|<span data-ttu-id="3607f-116">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="3607f-116">Old value.</span></span>|
|<span data-ttu-id="3607f-117">newValue</span><span class="sxs-lookup"><span data-stu-id="3607f-117">newValue</span></span>|<span data-ttu-id="3607f-118">String</span><span class="sxs-lookup"><span data-stu-id="3607f-118">String</span></span>|<span data-ttu-id="3607f-119">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="3607f-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3607f-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="3607f-120">Relationships</span></span>
<span data-ttu-id="3607f-121">Нет</span><span class="sxs-lookup"><span data-stu-id="3607f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3607f-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3607f-122">JSON Representation</span></span>
<span data-ttu-id="3607f-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3607f-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```





