---
title: Тип ресурса androidMobileAppIdentifier
description: Идентификатор приложения для Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3d34ff19e37a3453458621fb0876cb1a04b55308
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978015"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="e5518-103">Тип ресурса androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="e5518-103">androidMobileAppIdentifier resource type</span></span>

<span data-ttu-id="e5518-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5518-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5518-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5518-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5518-106">Идентификатор приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="e5518-106">The identifier for an Android app.</span></span>


<span data-ttu-id="e5518-107">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="e5518-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e5518-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5518-108">Properties</span></span>
|<span data-ttu-id="e5518-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5518-109">Property</span></span>|<span data-ttu-id="e5518-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e5518-110">Type</span></span>|<span data-ttu-id="e5518-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e5518-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5518-112">packageId</span><span class="sxs-lookup"><span data-stu-id="e5518-112">packageId</span></span>|<span data-ttu-id="e5518-113">String</span><span class="sxs-lookup"><span data-stu-id="e5518-113">String</span></span>|<span data-ttu-id="e5518-114">Идентификатор приложения, указанный в магазине Google Play.</span><span class="sxs-lookup"><span data-stu-id="e5518-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5518-115">Связи</span><span class="sxs-lookup"><span data-stu-id="e5518-115">Relationships</span></span>
<span data-ttu-id="e5518-116">Нет</span><span class="sxs-lookup"><span data-stu-id="e5518-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5518-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e5518-117">JSON Representation</span></span>
<span data-ttu-id="e5518-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5518-118">Here is a JSON representation of the resource.</span></span>
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









