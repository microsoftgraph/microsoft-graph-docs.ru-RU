---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9000c2989dc9b8e41c1f9aa36a05c29fc7a86cfe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010911"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="d86ba-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d86ba-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="d86ba-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d86ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d86ba-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d86ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d86ba-106">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="d86ba-106">The identifier for an Android app.</span></span>


<span data-ttu-id="d86ba-107">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="d86ba-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d86ba-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d86ba-108">Properties</span></span>
|<span data-ttu-id="d86ba-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d86ba-109">Property</span></span>|<span data-ttu-id="d86ba-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d86ba-110">Type</span></span>|<span data-ttu-id="d86ba-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d86ba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d86ba-112">packageId</span><span class="sxs-lookup"><span data-stu-id="d86ba-112">packageId</span></span>|<span data-ttu-id="d86ba-113">String</span><span class="sxs-lookup"><span data-stu-id="d86ba-113">String</span></span>|<span data-ttu-id="d86ba-114">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="d86ba-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d86ba-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="d86ba-115">Relationships</span></span>
<span data-ttu-id="d86ba-116">Нет</span><span class="sxs-lookup"><span data-stu-id="d86ba-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d86ba-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d86ba-117">JSON Representation</span></span>
<span data-ttu-id="d86ba-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d86ba-118">Here is a JSON representation of the resource.</span></span>
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





