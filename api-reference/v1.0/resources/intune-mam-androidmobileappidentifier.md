---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b4ba6cc892030489f73690362b4d5d30359d750a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530223"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="462f3-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="462f3-103">androidMobileAppIdentifier resource type</span></span>

<span data-ttu-id="462f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="462f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="462f3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="462f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="462f3-106">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="462f3-106">The identifier for an Android app.</span></span>


<span data-ttu-id="462f3-107">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="462f3-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="462f3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="462f3-108">Properties</span></span>
|<span data-ttu-id="462f3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="462f3-109">Property</span></span>|<span data-ttu-id="462f3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="462f3-110">Type</span></span>|<span data-ttu-id="462f3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="462f3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="462f3-112">packageId</span><span class="sxs-lookup"><span data-stu-id="462f3-112">packageId</span></span>|<span data-ttu-id="462f3-113">String</span><span class="sxs-lookup"><span data-stu-id="462f3-113">String</span></span>|<span data-ttu-id="462f3-114">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="462f3-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="462f3-115">Связи</span><span class="sxs-lookup"><span data-stu-id="462f3-115">Relationships</span></span>
<span data-ttu-id="462f3-116">Нет</span><span class="sxs-lookup"><span data-stu-id="462f3-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="462f3-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="462f3-117">JSON Representation</span></span>
<span data-ttu-id="462f3-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="462f3-118">Here is a JSON representation of the resource.</span></span>
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




