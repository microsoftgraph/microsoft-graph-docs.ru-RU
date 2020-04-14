---
title: Тип ресурса iosMobileAppIdentifier
description: Идентификатор приложения для iOS.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 88dd590887954334ce9a419f8140a41c8fdd5647
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43374103"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="a060d-103">Тип ресурса iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="a060d-103">iosMobileAppIdentifier resource type</span></span>

<span data-ttu-id="a060d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a060d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a060d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a060d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a060d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a060d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a060d-107">Идентификатор приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="a060d-107">The identifier for an iOS app.</span></span>


<span data-ttu-id="a060d-108">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="a060d-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a060d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a060d-109">Properties</span></span>
|<span data-ttu-id="a060d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a060d-110">Property</span></span>|<span data-ttu-id="a060d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a060d-111">Type</span></span>|<span data-ttu-id="a060d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a060d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a060d-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="a060d-113">bundleId</span></span>|<span data-ttu-id="a060d-114">String</span><span class="sxs-lookup"><span data-stu-id="a060d-114">String</span></span>|<span data-ttu-id="a060d-115">Идентификатор приложения, указанный в магазине приложений.</span><span class="sxs-lookup"><span data-stu-id="a060d-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a060d-116">Связи</span><span class="sxs-lookup"><span data-stu-id="a060d-116">Relationships</span></span>
<span data-ttu-id="a060d-117">Нет</span><span class="sxs-lookup"><span data-stu-id="a060d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a060d-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a060d-118">JSON Representation</span></span>
<span data-ttu-id="a060d-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a060d-119">Here is a JSON representation of the resource.</span></span>
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



