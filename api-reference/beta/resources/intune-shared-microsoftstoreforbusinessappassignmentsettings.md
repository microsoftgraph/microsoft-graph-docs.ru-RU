---
title: Тип ресурса microsoftStoreForBusinessAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de6faaf42df24ae89f8d0dd514e1beb4d1b6cb25
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070781"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="a195a-103">Тип ресурса microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="a195a-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

<span data-ttu-id="a195a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a195a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a195a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a195a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a195a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a195a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a195a-107">Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.</span><span class="sxs-lookup"><span data-stu-id="a195a-107">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="a195a-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a195a-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a195a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a195a-109">Properties</span></span>
|<span data-ttu-id="a195a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a195a-110">Property</span></span>|<span data-ttu-id="a195a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a195a-111">Type</span></span>|<span data-ttu-id="a195a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a195a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a195a-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="a195a-113">useDeviceContext</span></span>|<span data-ttu-id="a195a-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="a195a-114">Boolean</span></span>|<span data-ttu-id="a195a-115">Указывает, следует ли использовать контекст работы устройства для мобильного приложения Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="a195a-115">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a195a-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="a195a-116">Relationships</span></span>
<span data-ttu-id="a195a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="a195a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a195a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a195a-118">JSON Representation</span></span>
<span data-ttu-id="a195a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a195a-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings",
  "useDeviceContext": true
}
```






