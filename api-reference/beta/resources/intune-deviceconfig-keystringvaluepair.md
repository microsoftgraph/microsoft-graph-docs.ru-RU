---
title: Тип ресурса Кэйстрингвалуепаир
description: Значение типа "ключ — значение" со строковым ключом и строковым значением.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5492724d400c52638706c24df9826bf8725e00f2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269065"
---
# <a name="keystringvaluepair-resource-type"></a><span data-ttu-id="4845c-103">Тип ресурса Кэйстрингвалуепаир</span><span class="sxs-lookup"><span data-stu-id="4845c-103">keyStringValuePair resource type</span></span>

<span data-ttu-id="4845c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4845c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4845c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4845c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4845c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4845c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4845c-107">Значение типа "ключ — значение" со строковым ключом и строковым значением.</span><span class="sxs-lookup"><span data-stu-id="4845c-107">A key-value pair with a string key and a string value.</span></span>


<span data-ttu-id="4845c-108">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4845c-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4845c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4845c-109">Properties</span></span>
|<span data-ttu-id="4845c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4845c-110">Property</span></span>|<span data-ttu-id="4845c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4845c-111">Type</span></span>|<span data-ttu-id="4845c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4845c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4845c-113">key</span><span class="sxs-lookup"><span data-stu-id="4845c-113">key</span></span>|<span data-ttu-id="4845c-114">String</span><span class="sxs-lookup"><span data-stu-id="4845c-114">String</span></span>|<span data-ttu-id="4845c-115">Строковый ключ для типа "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="4845c-115">The string key of the key-value pair.</span></span> <span data-ttu-id="4845c-116">Наследуется от [кэйтипедвалуепаир](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4845c-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="4845c-117">value</span><span class="sxs-lookup"><span data-stu-id="4845c-117">value</span></span>|<span data-ttu-id="4845c-118">String</span><span class="sxs-lookup"><span data-stu-id="4845c-118">String</span></span>|<span data-ttu-id="4845c-119">Строковое значение для параметра "ключ — значение".</span><span class="sxs-lookup"><span data-stu-id="4845c-119">The string value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4845c-120">Связи</span><span class="sxs-lookup"><span data-stu-id="4845c-120">Relationships</span></span>
<span data-ttu-id="4845c-121">Нет</span><span class="sxs-lookup"><span data-stu-id="4845c-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4845c-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4845c-122">JSON Representation</span></span>
<span data-ttu-id="4845c-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4845c-123">Here is a JSON representation of the resource.</span></span>
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




