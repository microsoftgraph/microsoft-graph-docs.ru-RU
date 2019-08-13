---
title: Тип ресурса iosMobileAppIdentifier
description: Идентификатор приложения для iOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c4b3de2dd5dd25e5995e7a1d30ad4314bb34efa5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332220"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="e43d6-103">Тип ресурса iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="e43d6-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="e43d6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e43d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e43d6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e43d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e43d6-106">Идентификатор приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="e43d6-106">The identifier for an iOS app.</span></span>


<span data-ttu-id="e43d6-107">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="e43d6-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e43d6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e43d6-108">Properties</span></span>
|<span data-ttu-id="e43d6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e43d6-109">Property</span></span>|<span data-ttu-id="e43d6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e43d6-110">Type</span></span>|<span data-ttu-id="e43d6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e43d6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e43d6-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="e43d6-112">bundleId</span></span>|<span data-ttu-id="e43d6-113">String</span><span class="sxs-lookup"><span data-stu-id="e43d6-113">String</span></span>|<span data-ttu-id="e43d6-114">Идентификатор приложения, указанный в магазине приложений.</span><span class="sxs-lookup"><span data-stu-id="e43d6-114">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e43d6-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="e43d6-115">Relationships</span></span>
<span data-ttu-id="e43d6-116">Нет</span><span class="sxs-lookup"><span data-stu-id="e43d6-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e43d6-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e43d6-117">JSON Representation</span></span>
<span data-ttu-id="e43d6-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e43d6-118">Here is a JSON representation of the resource.</span></span>
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



