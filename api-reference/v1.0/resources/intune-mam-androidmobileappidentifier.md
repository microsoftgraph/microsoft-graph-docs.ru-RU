---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a26d5ec654749b23a78052d1e9a392857462b8c5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030571"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="ea896-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ea896-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="ea896-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea896-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea896-105">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="ea896-105">The identifier for an Android app.</span></span>


<span data-ttu-id="ea896-106">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="ea896-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ea896-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea896-107">Properties</span></span>
|<span data-ttu-id="ea896-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea896-108">Property</span></span>|<span data-ttu-id="ea896-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ea896-109">Type</span></span>|<span data-ttu-id="ea896-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ea896-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea896-111">packageId</span><span class="sxs-lookup"><span data-stu-id="ea896-111">packageId</span></span>|<span data-ttu-id="ea896-112">String</span><span class="sxs-lookup"><span data-stu-id="ea896-112">String</span></span>|<span data-ttu-id="ea896-113">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="ea896-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea896-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="ea896-114">Relationships</span></span>
<span data-ttu-id="ea896-115">Нет</span><span class="sxs-lookup"><span data-stu-id="ea896-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea896-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea896-116">JSON Representation</span></span>
<span data-ttu-id="ea896-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea896-117">Here is a JSON representation of the resource.</span></span>
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



