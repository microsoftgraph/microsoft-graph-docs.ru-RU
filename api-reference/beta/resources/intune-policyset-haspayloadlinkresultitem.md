---
title: Тип ресурса Хаспайлоадлинкресултитем
description: Класс, содержащий результат действия Хаспайлоадлинкс.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3194dc0e7c1f154dcb61ab4f4731111a87fefe9d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458412"
---
# <a name="haspayloadlinkresultitem-resource-type"></a><span data-ttu-id="e1543-103">Тип ресурса Хаспайлоадлинкресултитем</span><span class="sxs-lookup"><span data-stu-id="e1543-103">hasPayloadLinkResultItem resource type</span></span>

<span data-ttu-id="e1543-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1543-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1543-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1543-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1543-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e1543-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1543-107">Класс, содержащий результат действия Хаспайлоадлинкс.</span><span class="sxs-lookup"><span data-stu-id="e1543-107">A class containing the result of HasPayloadLinks action.</span></span>

## <a name="properties"></a><span data-ttu-id="e1543-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1543-108">Properties</span></span>
|<span data-ttu-id="e1543-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1543-109">Property</span></span>|<span data-ttu-id="e1543-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e1543-110">Type</span></span>|<span data-ttu-id="e1543-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e1543-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1543-112">пайлоадид</span><span class="sxs-lookup"><span data-stu-id="e1543-112">payloadId</span></span>|<span data-ttu-id="e1543-113">String</span><span class="sxs-lookup"><span data-stu-id="e1543-113">String</span></span>|<span data-ttu-id="e1543-114">Ключ полезных данных в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="e1543-114">Key of the Payload, In the format of Guid.</span></span>|
|<span data-ttu-id="e1543-115">хаслинк</span><span class="sxs-lookup"><span data-stu-id="e1543-115">hasLink</span></span>|<span data-ttu-id="e1543-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1543-116">Boolean</span></span>|<span data-ttu-id="e1543-117">Указывает, содержит ли полезная нагрузка какую бы то ни было ссылку.</span><span class="sxs-lookup"><span data-stu-id="e1543-117">Indicate whether a payload has any link or not.</span></span>|
|<span data-ttu-id="e1543-118">error</span><span class="sxs-lookup"><span data-stu-id="e1543-118">error</span></span>|<span data-ttu-id="e1543-119">String</span><span class="sxs-lookup"><span data-stu-id="e1543-119">String</span></span>|<span data-ttu-id="e1543-120">Сведения об исключении указывают на успешность проверки этого элемента. Пустая строка без ошибки.</span><span class="sxs-lookup"><span data-stu-id="e1543-120">Exception information indicates if check for this item was successful or not.Empty string for no error.</span></span>|
|<span data-ttu-id="e1543-121">sources</span><span class="sxs-lookup"><span data-stu-id="e1543-121">sources</span></span>|<span data-ttu-id="e1543-122">Коллекция [девицеандаппманажементассигнментсаурце](../resources/intune-shared-deviceandappmanagementassignmentsource.md)</span><span class="sxs-lookup"><span data-stu-id="e1543-122">[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md) collection</span></span>|<span data-ttu-id="e1543-123">Причина, по которой получена ссылка.</span><span class="sxs-lookup"><span data-stu-id="e1543-123">The reason where the link comes from.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1543-124">Связи</span><span class="sxs-lookup"><span data-stu-id="e1543-124">Relationships</span></span>
<span data-ttu-id="e1543-125">Нет</span><span class="sxs-lookup"><span data-stu-id="e1543-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1543-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1543-126">JSON Representation</span></span>
<span data-ttu-id="e1543-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1543-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hasPayloadLinkResultItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hasPayloadLinkResultItem",
  "payloadId": "String",
  "hasLink": true,
  "error": "String",
  "sources": [
    "String"
  ]
}
```



