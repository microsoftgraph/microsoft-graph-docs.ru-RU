---
title: Тип ресурса Андроидманажедстореаппассигнментсеттингс
description: Содержит свойства, используемые при назначении мобильного приложения с управляемым хранилищем Android группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 383c272efc420cba893208e806a29df55f5429f6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073679"
---
# <a name="androidmanagedstoreappassignmentsettings-resource-type"></a><span data-ttu-id="b58cb-103">Тип ресурса Андроидманажедстореаппассигнментсеттингс</span><span class="sxs-lookup"><span data-stu-id="b58cb-103">androidManagedStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="b58cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b58cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b58cb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b58cb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b58cb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b58cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b58cb-107">Содержит свойства, используемые при назначении мобильного приложения с управляемым хранилищем Android группе.</span><span class="sxs-lookup"><span data-stu-id="b58cb-107">Contains properties used to assign an Android Managed Store mobile app to a group.</span></span>


<span data-ttu-id="b58cb-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="b58cb-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b58cb-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b58cb-109">Properties</span></span>
|<span data-ttu-id="b58cb-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b58cb-110">Property</span></span>|<span data-ttu-id="b58cb-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b58cb-111">Type</span></span>|<span data-ttu-id="b58cb-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b58cb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b58cb-113">андроидманажедстореапптраккидс</span><span class="sxs-lookup"><span data-stu-id="b58cb-113">androidManagedStoreAppTrackIds</span></span>|<span data-ttu-id="b58cb-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b58cb-114">String collection</span></span>|<span data-ttu-id="b58cb-115">Идентификаторы отслеживания, которые необходимо включить для этого назначения приложения.</span><span class="sxs-lookup"><span data-stu-id="b58cb-115">The track IDs to enable for this app assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b58cb-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="b58cb-116">Relationships</span></span>
<span data-ttu-id="b58cb-117">Нет</span><span class="sxs-lookup"><span data-stu-id="b58cb-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b58cb-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b58cb-118">JSON Representation</span></span>
<span data-ttu-id="b58cb-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b58cb-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppAssignmentSettings",
  "androidManagedStoreAppTrackIds": [
    "String"
  ]
}
```






