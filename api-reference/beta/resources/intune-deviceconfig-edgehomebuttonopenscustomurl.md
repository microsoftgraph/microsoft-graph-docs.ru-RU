---
title: Тип ресурса Еджехомебуттонопенскустомурл
description: Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2dad4baba5fd55b99efd6b2b7ebadf1973d6c9c8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551717"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="9dd88-103">Тип ресурса Еджехомебуттонопенскустомурл</span><span class="sxs-lookup"><span data-stu-id="9dd88-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="9dd88-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dd88-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9dd88-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9dd88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9dd88-106">Отображение кнопки "домой"; Нажатие кнопки "домой" загружает определенный URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="9dd88-106">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="9dd88-107">НаСледуется от [еджехомебуттонконфигуратион](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9dd88-107">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9dd88-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9dd88-108">Properties</span></span>
|<span data-ttu-id="9dd88-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9dd88-109">Property</span></span>|<span data-ttu-id="9dd88-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9dd88-110">Type</span></span>|<span data-ttu-id="9dd88-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9dd88-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9dd88-112">Хомебуттонкустомурл</span><span class="sxs-lookup"><span data-stu-id="9dd88-112">homeButtonCustomURL</span></span>|<span data-ttu-id="9dd88-113">String</span><span class="sxs-lookup"><span data-stu-id="9dd88-113">String</span></span>|<span data-ttu-id="9dd88-114">Заданный URL-адрес для загрузки.</span><span class="sxs-lookup"><span data-stu-id="9dd88-114">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9dd88-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="9dd88-115">Relationships</span></span>
<span data-ttu-id="9dd88-116">Нет</span><span class="sxs-lookup"><span data-stu-id="9dd88-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9dd88-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9dd88-117">JSON Representation</span></span>
<span data-ttu-id="9dd88-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9dd88-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeHomeButtonOpensCustomURL"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeHomeButtonOpensCustomURL",
  "homeButtonCustomURL": "String"
}
```





