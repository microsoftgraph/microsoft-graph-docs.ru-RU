---
title: Тип ресурса Андроидманажедстореаппассигнментсеттингс
description: Содержит свойства, используемые при назначении мобильного приложения с управляемым хранилищем Android группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f07b1dc3535e624302b3d2ad2bfd047c286604b8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723787"
---
# <a name="androidmanagedstoreappassignmentsettings-resource-type"></a><span data-ttu-id="1be6b-103">Тип ресурса Андроидманажедстореаппассигнментсеттингс</span><span class="sxs-lookup"><span data-stu-id="1be6b-103">androidManagedStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="1be6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1be6b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1be6b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1be6b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1be6b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1be6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1be6b-107">Содержит свойства, используемые при назначении мобильного приложения с управляемым хранилищем Android группе.</span><span class="sxs-lookup"><span data-stu-id="1be6b-107">Contains properties used to assign an Android Managed Store mobile app to a group.</span></span>


<span data-ttu-id="1be6b-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="1be6b-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1be6b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1be6b-109">Properties</span></span>
|<span data-ttu-id="1be6b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1be6b-110">Property</span></span>|<span data-ttu-id="1be6b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1be6b-111">Type</span></span>|<span data-ttu-id="1be6b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1be6b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1be6b-113">андроидманажедстореапптраккидс</span><span class="sxs-lookup"><span data-stu-id="1be6b-113">androidManagedStoreAppTrackIds</span></span>|<span data-ttu-id="1be6b-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1be6b-114">String collection</span></span>|<span data-ttu-id="1be6b-115">Идентификаторы отслеживания, которые необходимо включить для этого назначения приложения.</span><span class="sxs-lookup"><span data-stu-id="1be6b-115">The track IDs to enable for this app assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1be6b-116">Связи</span><span class="sxs-lookup"><span data-stu-id="1be6b-116">Relationships</span></span>
<span data-ttu-id="1be6b-117">Нет</span><span class="sxs-lookup"><span data-stu-id="1be6b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1be6b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1be6b-118">JSON Representation</span></span>
<span data-ttu-id="1be6b-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1be6b-119">Here is a JSON representation of the resource.</span></span>
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





