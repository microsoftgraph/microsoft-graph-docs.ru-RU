---
title: Тип ресурса iosMobileAppIdentifier
description: Идентификатор приложения для iOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f836d6869cae062e0ce8aabe87dc5c1ce9c8c03a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684661"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="74cf1-103">Тип ресурса iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="74cf1-103">iosMobileAppIdentifier resource type</span></span>

<span data-ttu-id="74cf1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74cf1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74cf1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74cf1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74cf1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="74cf1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74cf1-107">Идентификатор приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="74cf1-107">The identifier for an iOS app.</span></span>


<span data-ttu-id="74cf1-108">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="74cf1-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="74cf1-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="74cf1-109">Properties</span></span>
|<span data-ttu-id="74cf1-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="74cf1-110">Property</span></span>|<span data-ttu-id="74cf1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="74cf1-111">Type</span></span>|<span data-ttu-id="74cf1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="74cf1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74cf1-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="74cf1-113">bundleId</span></span>|<span data-ttu-id="74cf1-114">String</span><span class="sxs-lookup"><span data-stu-id="74cf1-114">String</span></span>|<span data-ttu-id="74cf1-115">Идентификатор приложения, указанный в магазине приложений.</span><span class="sxs-lookup"><span data-stu-id="74cf1-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74cf1-116">Связи</span><span class="sxs-lookup"><span data-stu-id="74cf1-116">Relationships</span></span>
<span data-ttu-id="74cf1-117">Нет</span><span class="sxs-lookup"><span data-stu-id="74cf1-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="74cf1-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74cf1-118">JSON Representation</span></span>
<span data-ttu-id="74cf1-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74cf1-119">Here is a JSON representation of the resource.</span></span>
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





