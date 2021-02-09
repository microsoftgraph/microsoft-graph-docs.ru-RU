---
title: Тип ресурса windowsAppIdentifier
description: Идентификатор приложения для Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fd94a5cbd893c4f65dd726191f7a40198ca7750d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160697"
---
# <a name="windowsappidentifier-resource-type"></a><span data-ttu-id="b0b21-103">Тип ресурса windowsAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b0b21-103">windowsAppIdentifier resource type</span></span>

<span data-ttu-id="b0b21-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0b21-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0b21-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0b21-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0b21-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0b21-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0b21-107">Идентификатор приложения для Windows.</span><span class="sxs-lookup"><span data-stu-id="b0b21-107">The identifier for a Windows app.</span></span>


<span data-ttu-id="b0b21-108">Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="b0b21-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b0b21-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0b21-109">Properties</span></span>
|<span data-ttu-id="b0b21-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0b21-110">Property</span></span>|<span data-ttu-id="b0b21-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b0b21-111">Type</span></span>|<span data-ttu-id="b0b21-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b0b21-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0b21-113">windowsAppId</span><span class="sxs-lookup"><span data-stu-id="b0b21-113">windowsAppId</span></span>|<span data-ttu-id="b0b21-114">String</span><span class="sxs-lookup"><span data-stu-id="b0b21-114">String</span></span>|<span data-ttu-id="b0b21-115">Идентификатор приложения, указанный в магазине приложений.</span><span class="sxs-lookup"><span data-stu-id="b0b21-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0b21-116">Связи</span><span class="sxs-lookup"><span data-stu-id="b0b21-116">Relationships</span></span>
<span data-ttu-id="b0b21-117">Нет</span><span class="sxs-lookup"><span data-stu-id="b0b21-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0b21-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0b21-118">JSON Representation</span></span>
<span data-ttu-id="b0b21-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0b21-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAppIdentifier",
  "windowsAppId": "String"
}
```




