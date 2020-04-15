---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0b610cbfa4ba7296a9b8427b9bb49f7b4493f773
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474126"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="2c443-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="2c443-103">androidMobileAppIdentifier resource type</span></span>

<span data-ttu-id="2c443-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c443-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c443-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2c443-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c443-106">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="2c443-106">The identifier for an Android app.</span></span>


<span data-ttu-id="2c443-107">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="2c443-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2c443-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c443-108">Properties</span></span>
|<span data-ttu-id="2c443-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c443-109">Property</span></span>|<span data-ttu-id="2c443-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2c443-110">Type</span></span>|<span data-ttu-id="2c443-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2c443-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c443-112">packageId</span><span class="sxs-lookup"><span data-stu-id="2c443-112">packageId</span></span>|<span data-ttu-id="2c443-113">String</span><span class="sxs-lookup"><span data-stu-id="2c443-113">String</span></span>|<span data-ttu-id="2c443-114">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="2c443-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c443-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="2c443-115">Relationships</span></span>
<span data-ttu-id="2c443-116">Нет</span><span class="sxs-lookup"><span data-stu-id="2c443-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c443-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2c443-117">JSON Representation</span></span>
<span data-ttu-id="2c443-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c443-118">Here is a JSON representation of the resource.</span></span>
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







