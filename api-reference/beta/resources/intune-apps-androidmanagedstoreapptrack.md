---
title: Тип ресурса Андроидманажедстореапптракк
description: Содержит сведения о записях для приложений управляемого хранилища Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ab4009dfb8fc6cfd40ae49529e07a6a6932d7c4d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690275"
---
# <a name="androidmanagedstoreapptrack-resource-type"></a><span data-ttu-id="51916-103">Тип ресурса Андроидманажедстореапптракк</span><span class="sxs-lookup"><span data-stu-id="51916-103">androidManagedStoreAppTrack resource type</span></span>

<span data-ttu-id="51916-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51916-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51916-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51916-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51916-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51916-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51916-107">Содержит сведения о записях для приложений управляемого хранилища Android.</span><span class="sxs-lookup"><span data-stu-id="51916-107">Contains track information for Android Managed Store apps.</span></span>

## <a name="properties"></a><span data-ttu-id="51916-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="51916-108">Properties</span></span>
|<span data-ttu-id="51916-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="51916-109">Property</span></span>|<span data-ttu-id="51916-110">Тип</span><span class="sxs-lookup"><span data-stu-id="51916-110">Type</span></span>|<span data-ttu-id="51916-111">Описание</span><span class="sxs-lookup"><span data-stu-id="51916-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51916-112">траккид</span><span class="sxs-lookup"><span data-stu-id="51916-112">trackId</span></span>|<span data-ttu-id="51916-113">Строка</span><span class="sxs-lookup"><span data-stu-id="51916-113">String</span></span>|<span data-ttu-id="51916-114">Уникальный идентификатор записи.</span><span class="sxs-lookup"><span data-stu-id="51916-114">Unique track identifier.</span></span>|
|<span data-ttu-id="51916-115">траккалиас</span><span class="sxs-lookup"><span data-stu-id="51916-115">trackAlias</span></span>|<span data-ttu-id="51916-116">Строка</span><span class="sxs-lookup"><span data-stu-id="51916-116">String</span></span>|<span data-ttu-id="51916-117">Понятное имя для отслеживания.</span><span class="sxs-lookup"><span data-stu-id="51916-117">Friendly name for track.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51916-118">Связи</span><span class="sxs-lookup"><span data-stu-id="51916-118">Relationships</span></span>
<span data-ttu-id="51916-119">Нет</span><span class="sxs-lookup"><span data-stu-id="51916-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="51916-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51916-120">JSON Representation</span></span>
<span data-ttu-id="51916-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51916-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppTrack"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppTrack",
  "trackId": "String",
  "trackAlias": "String"
}
```





