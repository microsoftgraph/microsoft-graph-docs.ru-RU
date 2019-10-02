---
title: Тип ресурса iosMobileAppIdentifier
description: Идентификатор приложения для iOS.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c85d0f1a2bedffe8525c2012487646c4364ec2ff
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356501"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="caf2e-103">Тип ресурса iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="caf2e-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="caf2e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="caf2e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="caf2e-105">Идентификатор приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="caf2e-105">The identifier for an iOS app.</span></span>


<span data-ttu-id="caf2e-106">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="caf2e-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="caf2e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="caf2e-107">Properties</span></span>
|<span data-ttu-id="caf2e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="caf2e-108">Property</span></span>|<span data-ttu-id="caf2e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="caf2e-109">Type</span></span>|<span data-ttu-id="caf2e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="caf2e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caf2e-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="caf2e-111">bundleId</span></span>|<span data-ttu-id="caf2e-112">String</span><span class="sxs-lookup"><span data-stu-id="caf2e-112">String</span></span>|<span data-ttu-id="caf2e-113">Идентификатор приложения, указанный в магазине приложений.</span><span class="sxs-lookup"><span data-stu-id="caf2e-113">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="caf2e-114">Связи</span><span class="sxs-lookup"><span data-stu-id="caf2e-114">Relationships</span></span>
<span data-ttu-id="caf2e-115">Нет</span><span class="sxs-lookup"><span data-stu-id="caf2e-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="caf2e-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="caf2e-116">JSON Representation</span></span>
<span data-ttu-id="caf2e-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="caf2e-117">Here is a JSON representation of the resource.</span></span>
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




