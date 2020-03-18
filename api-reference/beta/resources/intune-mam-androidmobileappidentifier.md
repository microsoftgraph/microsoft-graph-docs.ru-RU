---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bc998a09d30d94b42c6c118a51dc028b8251e134
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42782666"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="aabbe-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="aabbe-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="aabbe-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aabbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aabbe-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aabbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aabbe-106">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="aabbe-106">The identifier for an Android app.</span></span>


<span data-ttu-id="aabbe-107">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="aabbe-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aabbe-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="aabbe-108">Properties</span></span>
|<span data-ttu-id="aabbe-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="aabbe-109">Property</span></span>|<span data-ttu-id="aabbe-110">Тип</span><span class="sxs-lookup"><span data-stu-id="aabbe-110">Type</span></span>|<span data-ttu-id="aabbe-111">Описание</span><span class="sxs-lookup"><span data-stu-id="aabbe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aabbe-112">packageId</span><span class="sxs-lookup"><span data-stu-id="aabbe-112">packageId</span></span>|<span data-ttu-id="aabbe-113">String</span><span class="sxs-lookup"><span data-stu-id="aabbe-113">String</span></span>|<span data-ttu-id="aabbe-114">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="aabbe-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aabbe-115">Связи</span><span class="sxs-lookup"><span data-stu-id="aabbe-115">Relationships</span></span>
<span data-ttu-id="aabbe-116">Нет</span><span class="sxs-lookup"><span data-stu-id="aabbe-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aabbe-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aabbe-117">JSON Representation</span></span>
<span data-ttu-id="aabbe-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aabbe-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMobileAppIdentifier",
  "packageId": "String"
}
```



