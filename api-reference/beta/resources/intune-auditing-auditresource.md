---
title: Тип ресурса auditResource
description: Класс, содержащий свойства ресурса аудита.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bba8aa9cfe10d17cefdcfe28d25c4d8c2dfa429f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412480"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="0c7ff-103">Тип ресурса auditResource</span><span class="sxs-lookup"><span data-stu-id="0c7ff-103">auditResource resource type</span></span>

> <span data-ttu-id="0c7ff-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0c7ff-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c7ff-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c7ff-107">Класс, содержащий свойства ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-107">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="0c7ff-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c7ff-108">Properties</span></span>
|<span data-ttu-id="0c7ff-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c7ff-109">Property</span></span>|<span data-ttu-id="0c7ff-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0c7ff-110">Type</span></span>|<span data-ttu-id="0c7ff-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0c7ff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c7ff-112">displayName</span><span class="sxs-lookup"><span data-stu-id="0c7ff-112">displayName</span></span>|<span data-ttu-id="0c7ff-113">String</span><span class="sxs-lookup"><span data-stu-id="0c7ff-113">String</span></span>|<span data-ttu-id="0c7ff-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-114">Display name.</span></span>|
|<span data-ttu-id="0c7ff-115">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="0c7ff-115">modifiedProperties</span></span>|<span data-ttu-id="0c7ff-116">Коллекция [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="0c7ff-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="0c7ff-117">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-117">List of modified properties.</span></span>|
|<span data-ttu-id="0c7ff-118">type</span><span class="sxs-lookup"><span data-stu-id="0c7ff-118">type</span></span>|<span data-ttu-id="0c7ff-119">String</span><span class="sxs-lookup"><span data-stu-id="0c7ff-119">String</span></span>|<span data-ttu-id="0c7ff-120">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-120">Audit resource's type.</span></span>|
|<span data-ttu-id="0c7ff-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="0c7ff-121">resourceId</span></span>|<span data-ttu-id="0c7ff-122">String</span><span class="sxs-lookup"><span data-stu-id="0c7ff-122">String</span></span>|<span data-ttu-id="0c7ff-123">ИД ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c7ff-124">Связи</span><span class="sxs-lookup"><span data-stu-id="0c7ff-124">Relationships</span></span>
<span data-ttu-id="0c7ff-125">Нет</span><span class="sxs-lookup"><span data-stu-id="0c7ff-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c7ff-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c7ff-126">JSON Representation</span></span>
<span data-ttu-id="0c7ff-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c7ff-127">Here is a JSON representation of the resource.</span></span>
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




