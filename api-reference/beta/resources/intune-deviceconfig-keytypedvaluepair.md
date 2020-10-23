---
title: Тип ресурса Кэйтипедвалуепаир
description: Значение типа "ключ — значение" со строковым ключом и типизированным значением.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da689e16e795910e9ab24f3e95647bd07a6e535e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697884"
---
# <a name="keytypedvaluepair-resource-type"></a><span data-ttu-id="15ee0-103">Тип ресурса Кэйтипедвалуепаир</span><span class="sxs-lookup"><span data-stu-id="15ee0-103">keyTypedValuePair resource type</span></span>

<span data-ttu-id="15ee0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15ee0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15ee0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15ee0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15ee0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15ee0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15ee0-107">Значение типа "ключ — значение" со строковым ключом и типизированным значением.</span><span class="sxs-lookup"><span data-stu-id="15ee0-107">A key-value pair with a string key and a typed value.</span></span>

## <a name="properties"></a><span data-ttu-id="15ee0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="15ee0-108">Properties</span></span>
|<span data-ttu-id="15ee0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="15ee0-109">Property</span></span>|<span data-ttu-id="15ee0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="15ee0-110">Type</span></span>|<span data-ttu-id="15ee0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="15ee0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15ee0-112">key</span><span class="sxs-lookup"><span data-stu-id="15ee0-112">key</span></span>|<span data-ttu-id="15ee0-113">Строка</span><span class="sxs-lookup"><span data-stu-id="15ee0-113">String</span></span>|<span data-ttu-id="15ee0-114">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="15ee0-114">The string key of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15ee0-115">Связи</span><span class="sxs-lookup"><span data-stu-id="15ee0-115">Relationships</span></span>
<span data-ttu-id="15ee0-116">Нет</span><span class="sxs-lookup"><span data-stu-id="15ee0-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15ee0-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15ee0-117">JSON Representation</span></span>
<span data-ttu-id="15ee0-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15ee0-118">Here is a JSON representation of the resource.</span></span>
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





