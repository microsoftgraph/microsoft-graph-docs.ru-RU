---
title: Тип ресурса microsoftStoreForBusinessAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dbfb271e8cfb0d019a0e127d1ad81ee033544a17
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "43457892"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="ea16d-103">Тип ресурса microsoftStoreForBusinessAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="ea16d-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

<span data-ttu-id="ea16d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea16d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea16d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea16d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea16d-106">Содержит свойства, используемые при назначении мобильного приложения Microsoft Store для бизнеса группе.</span><span class="sxs-lookup"><span data-stu-id="ea16d-106">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="ea16d-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="ea16d-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ea16d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea16d-108">Properties</span></span>
|<span data-ttu-id="ea16d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea16d-109">Property</span></span>|<span data-ttu-id="ea16d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ea16d-110">Type</span></span>|<span data-ttu-id="ea16d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ea16d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea16d-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="ea16d-112">useDeviceContext</span></span>|<span data-ttu-id="ea16d-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea16d-113">Boolean</span></span>|<span data-ttu-id="ea16d-114">Указывает, следует ли использовать контекст работы устройства для мобильного приложения Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="ea16d-114">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea16d-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="ea16d-115">Relationships</span></span>
<span data-ttu-id="ea16d-116">Нет</span><span class="sxs-lookup"><span data-stu-id="ea16d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea16d-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea16d-117">JSON Representation</span></span>
<span data-ttu-id="ea16d-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea16d-118">Here is a JSON representation of the resource.</span></span>
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







