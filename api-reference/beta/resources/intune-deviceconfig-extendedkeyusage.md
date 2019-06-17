---
title: Тип ресурса Екстендедкэйусаже
description: Настраиваемое определение расширенного использования ключа
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9eb9a02c8f403bf4ee29fc28622ab06f592c870b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34982520"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="e8278-103">Тип ресурса Екстендедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="e8278-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="e8278-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8278-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8278-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8278-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8278-106">Настраиваемое определение расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="e8278-106">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="e8278-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e8278-107">Properties</span></span>
|<span data-ttu-id="e8278-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8278-108">Property</span></span>|<span data-ttu-id="e8278-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e8278-109">Type</span></span>|<span data-ttu-id="e8278-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e8278-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8278-111">name</span><span class="sxs-lookup"><span data-stu-id="e8278-111">name</span></span>|<span data-ttu-id="e8278-112">String</span><span class="sxs-lookup"><span data-stu-id="e8278-112">String</span></span>|<span data-ttu-id="e8278-113">Имя расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="e8278-113">Extended Key Usage Name</span></span>|
|<span data-ttu-id="e8278-114">Обжектидентифиер</span><span class="sxs-lookup"><span data-stu-id="e8278-114">objectIdentifier</span></span>|<span data-ttu-id="e8278-115">String</span><span class="sxs-lookup"><span data-stu-id="e8278-115">String</span></span>|<span data-ttu-id="e8278-116">Идентификатор объекта расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="e8278-116">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8278-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="e8278-117">Relationships</span></span>
<span data-ttu-id="e8278-118">Нет</span><span class="sxs-lookup"><span data-stu-id="e8278-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8278-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e8278-119">JSON Representation</span></span>
<span data-ttu-id="e8278-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8278-120">Here is a JSON representation of the resource.</span></span>
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





