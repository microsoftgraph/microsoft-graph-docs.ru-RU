---
title: Тип ресурса iosMobileAppIdentifier
description: Идентификатор приложения для iOS.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 088f5507051676d587334966b91d4d4d1e8a135c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468564"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="61b9a-103">Тип ресурса iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="61b9a-103">iosMobileAppIdentifier resource type</span></span>

<span data-ttu-id="61b9a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61b9a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61b9a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="61b9a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61b9a-106">Идентификатор приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="61b9a-106">The identifier for an iOS app.</span></span>


<span data-ttu-id="61b9a-107">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="61b9a-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="61b9a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="61b9a-108">Properties</span></span>
|<span data-ttu-id="61b9a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="61b9a-109">Property</span></span>|<span data-ttu-id="61b9a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="61b9a-110">Type</span></span>|<span data-ttu-id="61b9a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="61b9a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61b9a-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="61b9a-112">bundleId</span></span>|<span data-ttu-id="61b9a-113">String</span><span class="sxs-lookup"><span data-stu-id="61b9a-113">String</span></span>|<span data-ttu-id="61b9a-114">Идентификатор приложения, указанный в магазине приложений.</span><span class="sxs-lookup"><span data-stu-id="61b9a-114">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61b9a-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="61b9a-115">Relationships</span></span>
<span data-ttu-id="61b9a-116">Нет</span><span class="sxs-lookup"><span data-stu-id="61b9a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61b9a-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="61b9a-117">JSON Representation</span></span>
<span data-ttu-id="61b9a-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61b9a-118">Here is a JSON representation of the resource.</span></span>
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







