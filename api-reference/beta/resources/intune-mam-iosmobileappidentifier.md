---
title: Тип ресурса iosMobileAppIdentifier
description: Идентификатор приложения для iOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b106811c802571edfd4da28134ea99883869c129
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030467"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="bdf11-103">Тип ресурса iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="bdf11-103">iosMobileAppIdentifier resource type</span></span>

<span data-ttu-id="bdf11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdf11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bdf11-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdf11-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdf11-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bdf11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdf11-107">Идентификатор приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="bdf11-107">The identifier for an iOS app.</span></span>


<span data-ttu-id="bdf11-108">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="bdf11-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bdf11-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="bdf11-109">Properties</span></span>
|<span data-ttu-id="bdf11-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="bdf11-110">Property</span></span>|<span data-ttu-id="bdf11-111">Тип</span><span class="sxs-lookup"><span data-stu-id="bdf11-111">Type</span></span>|<span data-ttu-id="bdf11-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bdf11-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdf11-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="bdf11-113">bundleId</span></span>|<span data-ttu-id="bdf11-114">String</span><span class="sxs-lookup"><span data-stu-id="bdf11-114">String</span></span>|<span data-ttu-id="bdf11-115">Идентификатор приложения, указанный в магазине приложений.</span><span class="sxs-lookup"><span data-stu-id="bdf11-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdf11-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="bdf11-116">Relationships</span></span>
<span data-ttu-id="bdf11-117">Нет</span><span class="sxs-lookup"><span data-stu-id="bdf11-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bdf11-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bdf11-118">JSON Representation</span></span>
<span data-ttu-id="bdf11-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bdf11-119">Here is a JSON representation of the resource.</span></span>
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






