---
title: Тип ресурса auditResource
description: Класс, содержащий свойства ресурса аудита.
author: tfitzmac
ms.openlocfilehash: c60c76f899fabfbced271e6ec38043337b8b3851
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339867"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="e4b8e-103">Тип ресурса auditResource</span><span class="sxs-lookup"><span data-stu-id="e4b8e-103">auditResource resource type</span></span>

> <span data-ttu-id="e4b8e-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e4b8e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4b8e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4b8e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4b8e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e4b8e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4b8e-107">Класс, содержащий свойства ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="e4b8e-107">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="e4b8e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4b8e-108">Properties</span></span>
|<span data-ttu-id="e4b8e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4b8e-109">Property</span></span>|<span data-ttu-id="e4b8e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e4b8e-110">Type</span></span>|<span data-ttu-id="e4b8e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e4b8e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4b8e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e4b8e-112">displayName</span></span>|<span data-ttu-id="e4b8e-113">String</span><span class="sxs-lookup"><span data-stu-id="e4b8e-113">String</span></span>|<span data-ttu-id="e4b8e-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="e4b8e-114">Display name.</span></span>|
|<span data-ttu-id="e4b8e-115">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="e4b8e-115">modifiedProperties</span></span>|<span data-ttu-id="e4b8e-116">Коллекция [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="e4b8e-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="e4b8e-117">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="e4b8e-117">List of modified properties.</span></span>|
|<span data-ttu-id="e4b8e-118">type</span><span class="sxs-lookup"><span data-stu-id="e4b8e-118">type</span></span>|<span data-ttu-id="e4b8e-119">String</span><span class="sxs-lookup"><span data-stu-id="e4b8e-119">String</span></span>|<span data-ttu-id="e4b8e-120">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="e4b8e-120">Audit resource's type.</span></span>|
|<span data-ttu-id="e4b8e-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="e4b8e-121">resourceId</span></span>|<span data-ttu-id="e4b8e-122">String</span><span class="sxs-lookup"><span data-stu-id="e4b8e-122">String</span></span>|<span data-ttu-id="e4b8e-123">ИД ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="e4b8e-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4b8e-124">Связи</span><span class="sxs-lookup"><span data-stu-id="e4b8e-124">Relationships</span></span>
<span data-ttu-id="e4b8e-125">Нет</span><span class="sxs-lookup"><span data-stu-id="e4b8e-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e4b8e-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4b8e-126">JSON Representation</span></span>
<span data-ttu-id="e4b8e-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4b8e-127">Here is a JSON representation of the resource.</span></span>
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





