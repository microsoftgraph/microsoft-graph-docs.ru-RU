---
title: Тип ресурса Кэйтипедвалуепаир
description: Значение типа "ключ — значение" со строковым ключом и типизированным значением.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c0d86243be0a9c40137d194727a762272e7f53dc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269037"
---
# <a name="keytypedvaluepair-resource-type"></a><span data-ttu-id="fb854-103">Тип ресурса Кэйтипедвалуепаир</span><span class="sxs-lookup"><span data-stu-id="fb854-103">keyTypedValuePair resource type</span></span>

<span data-ttu-id="fb854-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb854-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb854-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb854-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb854-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb854-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb854-107">Значение типа "ключ — значение" со строковым ключом и типизированным значением.</span><span class="sxs-lookup"><span data-stu-id="fb854-107">A key-value pair with a string key and a typed value.</span></span>

## <a name="properties"></a><span data-ttu-id="fb854-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb854-108">Properties</span></span>
|<span data-ttu-id="fb854-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb854-109">Property</span></span>|<span data-ttu-id="fb854-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fb854-110">Type</span></span>|<span data-ttu-id="fb854-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fb854-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb854-112">key</span><span class="sxs-lookup"><span data-stu-id="fb854-112">key</span></span>|<span data-ttu-id="fb854-113">String</span><span class="sxs-lookup"><span data-stu-id="fb854-113">String</span></span>|<span data-ttu-id="fb854-114">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="fb854-114">The string key of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb854-115">Связи</span><span class="sxs-lookup"><span data-stu-id="fb854-115">Relationships</span></span>
<span data-ttu-id="fb854-116">Нет</span><span class="sxs-lookup"><span data-stu-id="fb854-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb854-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb854-117">JSON Representation</span></span>
<span data-ttu-id="fb854-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb854-118">Here is a JSON representation of the resource.</span></span>
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




