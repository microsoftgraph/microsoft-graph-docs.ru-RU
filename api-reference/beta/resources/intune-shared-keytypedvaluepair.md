---
title: Тип ресурса Кэйтипедвалуепаир
description: Значение типа "ключ — значение" со строковым ключом и типизированным значением.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 392988272257bdaf7fc3e5b8bafd6d7ca652547d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955627"
---
# <a name="keytypedvaluepair-resource-type"></a><span data-ttu-id="ce848-103">Тип ресурса Кэйтипедвалуепаир</span><span class="sxs-lookup"><span data-stu-id="ce848-103">keyTypedValuePair resource type</span></span>

> <span data-ttu-id="ce848-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce848-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce848-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce848-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce848-106">Значение типа "ключ — значение" со строковым ключом и типизированным значением.</span><span class="sxs-lookup"><span data-stu-id="ce848-106">A key-value pair with a string key and a typed value.</span></span>

## <a name="properties"></a><span data-ttu-id="ce848-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce848-107">Properties</span></span>
|<span data-ttu-id="ce848-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce848-108">Property</span></span>|<span data-ttu-id="ce848-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ce848-109">Type</span></span>|<span data-ttu-id="ce848-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ce848-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce848-111">key</span><span class="sxs-lookup"><span data-stu-id="ce848-111">key</span></span>|<span data-ttu-id="ce848-112">Строка</span><span class="sxs-lookup"><span data-stu-id="ce848-112">String</span></span>|<span data-ttu-id="ce848-113">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="ce848-113">The string key of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce848-114">Связи</span><span class="sxs-lookup"><span data-stu-id="ce848-114">Relationships</span></span>
<span data-ttu-id="ce848-115">Нет</span><span class="sxs-lookup"><span data-stu-id="ce848-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce848-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce848-116">JSON Representation</span></span>
<span data-ttu-id="ce848-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce848-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyTypedValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyTypedValuePair",
  "key": "String"
}
```



