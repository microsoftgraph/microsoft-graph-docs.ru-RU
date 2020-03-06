---
title: Тип ресурса iosMobileAppIdentifier
description: Идентификатор приложения для iOS.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b485d5b0ba526971a29e98d764aa459e870fd725
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533207"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="3271c-103">Тип ресурса iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="3271c-103">iosMobileAppIdentifier resource type</span></span>

<span data-ttu-id="3271c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3271c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3271c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3271c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3271c-106">Идентификатор приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="3271c-106">The identifier for an iOS app.</span></span>


<span data-ttu-id="3271c-107">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="3271c-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3271c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3271c-108">Properties</span></span>
|<span data-ttu-id="3271c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3271c-109">Property</span></span>|<span data-ttu-id="3271c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3271c-110">Type</span></span>|<span data-ttu-id="3271c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3271c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3271c-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="3271c-112">bundleId</span></span>|<span data-ttu-id="3271c-113">String</span><span class="sxs-lookup"><span data-stu-id="3271c-113">String</span></span>|<span data-ttu-id="3271c-114">Идентификатор приложения, указанный в магазине приложений.</span><span class="sxs-lookup"><span data-stu-id="3271c-114">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3271c-115">Связи</span><span class="sxs-lookup"><span data-stu-id="3271c-115">Relationships</span></span>
<span data-ttu-id="3271c-116">Нет</span><span class="sxs-lookup"><span data-stu-id="3271c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3271c-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3271c-117">JSON Representation</span></span>
<span data-ttu-id="3271c-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3271c-118">Here is a JSON representation of the resource.</span></span>
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




