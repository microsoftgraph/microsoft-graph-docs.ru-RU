---
title: Тип ресурса Екстендедкэйусаже
description: Настраиваемое определение расширенного использования ключа
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 19cf790f692d624d926485fdc26feed1f69c73b7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791774"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="5177d-103">Тип ресурса Екстендедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="5177d-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="5177d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5177d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5177d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5177d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5177d-106">Настраиваемое определение расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="5177d-106">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="5177d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5177d-107">Properties</span></span>
|<span data-ttu-id="5177d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5177d-108">Property</span></span>|<span data-ttu-id="5177d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5177d-109">Type</span></span>|<span data-ttu-id="5177d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5177d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5177d-111">name</span><span class="sxs-lookup"><span data-stu-id="5177d-111">name</span></span>|<span data-ttu-id="5177d-112">String</span><span class="sxs-lookup"><span data-stu-id="5177d-112">String</span></span>|<span data-ttu-id="5177d-113">Имя расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="5177d-113">Extended Key Usage Name</span></span>|
|<span data-ttu-id="5177d-114">обжектидентифиер</span><span class="sxs-lookup"><span data-stu-id="5177d-114">objectIdentifier</span></span>|<span data-ttu-id="5177d-115">String</span><span class="sxs-lookup"><span data-stu-id="5177d-115">String</span></span>|<span data-ttu-id="5177d-116">Идентификатор объекта расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="5177d-116">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="5177d-117">Связи</span><span class="sxs-lookup"><span data-stu-id="5177d-117">Relationships</span></span>
<span data-ttu-id="5177d-118">Нет</span><span class="sxs-lookup"><span data-stu-id="5177d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5177d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5177d-119">JSON Representation</span></span>
<span data-ttu-id="5177d-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5177d-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```



