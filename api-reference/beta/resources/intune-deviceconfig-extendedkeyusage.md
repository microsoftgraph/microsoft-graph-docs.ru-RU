---
title: Тип ресурса Екстендедкэйусаже
description: Настраиваемое определение расширенного использования ключа
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5fbcaaf764a0b079df77d81d07e53094a8035e07
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001340"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="e94e8-103">Тип ресурса Екстендедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="e94e8-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="e94e8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e94e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e94e8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e94e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e94e8-106">Настраиваемое определение расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="e94e8-106">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="e94e8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e94e8-107">Properties</span></span>
|<span data-ttu-id="e94e8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e94e8-108">Property</span></span>|<span data-ttu-id="e94e8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e94e8-109">Type</span></span>|<span data-ttu-id="e94e8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e94e8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e94e8-111">name</span><span class="sxs-lookup"><span data-stu-id="e94e8-111">name</span></span>|<span data-ttu-id="e94e8-112">String</span><span class="sxs-lookup"><span data-stu-id="e94e8-112">String</span></span>|<span data-ttu-id="e94e8-113">Имя расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="e94e8-113">Extended Key Usage Name</span></span>|
|<span data-ttu-id="e94e8-114">Обжектидентифиер</span><span class="sxs-lookup"><span data-stu-id="e94e8-114">objectIdentifier</span></span>|<span data-ttu-id="e94e8-115">String</span><span class="sxs-lookup"><span data-stu-id="e94e8-115">String</span></span>|<span data-ttu-id="e94e8-116">Идентификатор объекта расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="e94e8-116">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="e94e8-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="e94e8-117">Relationships</span></span>
<span data-ttu-id="e94e8-118">Нет</span><span class="sxs-lookup"><span data-stu-id="e94e8-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e94e8-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e94e8-119">JSON Representation</span></span>
<span data-ttu-id="e94e8-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e94e8-120">Here is a JSON representation of the resource.</span></span>
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





