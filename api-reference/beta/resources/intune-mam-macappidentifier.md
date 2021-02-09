---
title: Тип ресурса macAppIdentifier
description: Идентификатор приложения для Mac.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b4ee44dc2fe288d7a1605660ef95dc7d88f600fb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160961"
---
# <a name="macappidentifier-resource-type"></a><span data-ttu-id="dbc76-103">Тип ресурса macAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="dbc76-103">macAppIdentifier resource type</span></span>

<span data-ttu-id="dbc76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbc76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dbc76-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbc76-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dbc76-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dbc76-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbc76-107">Идентификатор приложения для Mac.</span><span class="sxs-lookup"><span data-stu-id="dbc76-107">The identifier for a Mac app.</span></span>


<span data-ttu-id="dbc76-108">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="dbc76-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dbc76-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="dbc76-109">Properties</span></span>
|<span data-ttu-id="dbc76-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="dbc76-110">Property</span></span>|<span data-ttu-id="dbc76-111">Тип</span><span class="sxs-lookup"><span data-stu-id="dbc76-111">Type</span></span>|<span data-ttu-id="dbc76-112">Описание</span><span class="sxs-lookup"><span data-stu-id="dbc76-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbc76-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="dbc76-113">bundleId</span></span>|<span data-ttu-id="dbc76-114">String</span><span class="sxs-lookup"><span data-stu-id="dbc76-114">String</span></span>|<span data-ttu-id="dbc76-115">Идентификатор приложения, указанный в магазине приложений.</span><span class="sxs-lookup"><span data-stu-id="dbc76-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dbc76-116">Связи</span><span class="sxs-lookup"><span data-stu-id="dbc76-116">Relationships</span></span>
<span data-ttu-id="dbc76-117">Нет</span><span class="sxs-lookup"><span data-stu-id="dbc76-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dbc76-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dbc76-118">JSON Representation</span></span>
<span data-ttu-id="dbc76-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dbc76-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macAppIdentifier",
  "bundleId": "String"
}
```




