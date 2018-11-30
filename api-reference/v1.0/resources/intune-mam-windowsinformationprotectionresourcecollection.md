---
title: Тип ресурса windowsInformationProtectionResourceCollection
description: Коллекция ресурсов Windows Information Protection
ms.openlocfilehash: fd350f85acb962267f92352e6298dc50c44949ed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026068"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="745be-103">Тип ресурса windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="745be-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="745be-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="745be-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="745be-105">Коллекция ресурсов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="745be-105">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="745be-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="745be-106">Properties</span></span>
|<span data-ttu-id="745be-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="745be-107">Property</span></span>|<span data-ttu-id="745be-108">Тип</span><span class="sxs-lookup"><span data-stu-id="745be-108">Type</span></span>|<span data-ttu-id="745be-109">Описание</span><span class="sxs-lookup"><span data-stu-id="745be-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="745be-110">displayName</span><span class="sxs-lookup"><span data-stu-id="745be-110">displayName</span></span>|<span data-ttu-id="745be-111">Строка</span><span class="sxs-lookup"><span data-stu-id="745be-111">String</span></span>|<span data-ttu-id="745be-112">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="745be-112">Display name</span></span>|
|<span data-ttu-id="745be-113">resources</span><span class="sxs-lookup"><span data-stu-id="745be-113">resources</span></span>|<span data-ttu-id="745be-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="745be-114">String collection</span></span>|<span data-ttu-id="745be-115">Коллекция ресурсов</span><span class="sxs-lookup"><span data-stu-id="745be-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="745be-116">Связи</span><span class="sxs-lookup"><span data-stu-id="745be-116">Relationships</span></span>
<span data-ttu-id="745be-117">Нет</span><span class="sxs-lookup"><span data-stu-id="745be-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="745be-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="745be-118">JSON Representation</span></span>
<span data-ttu-id="745be-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="745be-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```



