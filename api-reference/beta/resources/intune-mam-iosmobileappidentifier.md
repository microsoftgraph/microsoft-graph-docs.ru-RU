---
title: Тип ресурса iosMobileAppIdentifier
description: Идентификатор приложения для iOS.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 10744d417738baf6f0d83a287a5e518fa6e55b60
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42782365"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="edaa3-103">Тип ресурса iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="edaa3-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="edaa3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edaa3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edaa3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="edaa3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edaa3-106">Идентификатор приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="edaa3-106">The identifier for an iOS app.</span></span>


<span data-ttu-id="edaa3-107">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="edaa3-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="edaa3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="edaa3-108">Properties</span></span>
|<span data-ttu-id="edaa3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="edaa3-109">Property</span></span>|<span data-ttu-id="edaa3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="edaa3-110">Type</span></span>|<span data-ttu-id="edaa3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="edaa3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edaa3-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="edaa3-112">bundleId</span></span>|<span data-ttu-id="edaa3-113">String</span><span class="sxs-lookup"><span data-stu-id="edaa3-113">String</span></span>|<span data-ttu-id="edaa3-114">Идентификатор приложения, указанный в магазине приложений.</span><span class="sxs-lookup"><span data-stu-id="edaa3-114">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="edaa3-115">Связи</span><span class="sxs-lookup"><span data-stu-id="edaa3-115">Relationships</span></span>
<span data-ttu-id="edaa3-116">Нет</span><span class="sxs-lookup"><span data-stu-id="edaa3-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="edaa3-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="edaa3-117">JSON Representation</span></span>
<span data-ttu-id="edaa3-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edaa3-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppIdentifier",
  "bundleId": "String"
}
```



