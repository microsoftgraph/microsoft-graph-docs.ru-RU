---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8ab50278d26e7de3eb90ad64f5ae84d7cfe674f6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332318"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="b0db8-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b0db8-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="b0db8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0db8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0db8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0db8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0db8-106">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="b0db8-106">The identifier for an Android app.</span></span>


<span data-ttu-id="b0db8-107">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="b0db8-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b0db8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0db8-108">Properties</span></span>
|<span data-ttu-id="b0db8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0db8-109">Property</span></span>|<span data-ttu-id="b0db8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b0db8-110">Type</span></span>|<span data-ttu-id="b0db8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b0db8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0db8-112">packageId</span><span class="sxs-lookup"><span data-stu-id="b0db8-112">packageId</span></span>|<span data-ttu-id="b0db8-113">String</span><span class="sxs-lookup"><span data-stu-id="b0db8-113">String</span></span>|<span data-ttu-id="b0db8-114">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="b0db8-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0db8-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="b0db8-115">Relationships</span></span>
<span data-ttu-id="b0db8-116">Нет</span><span class="sxs-lookup"><span data-stu-id="b0db8-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0db8-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0db8-117">JSON Representation</span></span>
<span data-ttu-id="b0db8-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0db8-118">Here is a JSON representation of the resource.</span></span>
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



