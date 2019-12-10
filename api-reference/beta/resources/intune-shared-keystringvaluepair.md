---
title: Тип ресурса Кэйстрингвалуепаир
description: Значение типа "ключ — значение" со строковым ключом и строковым значением.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7c62ec2cf1fbe5a78534bdb5f6ff9b1e73e37c9f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39924523"
---
# <a name="keystringvaluepair-resource-type"></a><span data-ttu-id="cada0-103">Тип ресурса Кэйстрингвалуепаир</span><span class="sxs-lookup"><span data-stu-id="cada0-103">keyStringValuePair resource type</span></span>

> <span data-ttu-id="cada0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cada0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cada0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cada0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cada0-106">Значение типа "ключ — значение" со строковым ключом и строковым значением.</span><span class="sxs-lookup"><span data-stu-id="cada0-106">A key-value pair with a string key and a string value.</span></span>


<span data-ttu-id="cada0-107">Наследуется от [кэйтипедвалуепаир](../resources/intune-shared-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="cada0-107">Inherits from [keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cada0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cada0-108">Properties</span></span>
|<span data-ttu-id="cada0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cada0-109">Property</span></span>|<span data-ttu-id="cada0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cada0-110">Type</span></span>|<span data-ttu-id="cada0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cada0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cada0-112">key</span><span class="sxs-lookup"><span data-stu-id="cada0-112">key</span></span>|<span data-ttu-id="cada0-113">Строка</span><span class="sxs-lookup"><span data-stu-id="cada0-113">String</span></span>|<span data-ttu-id="cada0-114">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="cada0-114">The string key of the key-value pair.</span></span> <span data-ttu-id="cada0-115">Наследуется от [кэйтипедвалуепаир](../resources/intune-shared-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="cada0-115">Inherited from [keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="cada0-116">value</span><span class="sxs-lookup"><span data-stu-id="cada0-116">value</span></span>|<span data-ttu-id="cada0-117">String</span><span class="sxs-lookup"><span data-stu-id="cada0-117">String</span></span>|<span data-ttu-id="cada0-118">Строковое значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="cada0-118">The string value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cada0-119">Связи</span><span class="sxs-lookup"><span data-stu-id="cada0-119">Relationships</span></span>
<span data-ttu-id="cada0-120">Нет</span><span class="sxs-lookup"><span data-stu-id="cada0-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cada0-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cada0-121">JSON Representation</span></span>
<span data-ttu-id="cada0-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cada0-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyStringValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyStringValuePair",
  "key": "String",
  "value": "String"
}
```



